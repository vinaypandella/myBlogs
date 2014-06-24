---
layout: post
title:  "Running Multiple Tomcat Instances using one source"
date:   2014-06-17 22:04:30
categories: Tomcat Server Coding Development Software
comments: true
excerpt:  multipletomcat
---

Here’s a brief on how to run more than one instance of Tomcat on a single machine.

Install Tomcat
--------------
Download Tomcat 5.5, 6.x, or 7.x and unzip it into an appropriate directory. Put it in /usr/local, so it ends up in a directory called /usr/local/apache-tomcat-5.5.17, and make a symlink named /usr/local/tomcat to that directory.

Make directories for each instance
----------------------------------

For each instance of Tomcat you’re going to run, you’ll need a directory that will be CATALINA_BASE. For example, you might make them /var/tomcat/serverA and /var/tomcat/serverB.

In each of these directories you need the following subdirectories: conf, logs, temp, webapps, and work.

Put a server.xml and web.xml file in the conf directory. You can get these from the conf directory of the directory where you put the tomcat installation files, although of course you should tighten up your server.xml a bit.

The webapps directory is where you’ll put the web applications you want to run on the particular instance of Tomcat.

Usually you can do this through DevOps code.

Configure the ports and/or addresses for each instance
------------------------------------------------------

Tomcat listens to at least two network ports, one for the shutdown command, and one or more for accepting requests. Two instances of Tomcat can’t listen to the same port number on the same IP address, so you will need to edit your server.xml files to change the ports they listen to.

The first port to look at is the shutdown port. This is used by the command line shutdown script (actually, but the Java code it runs) to tell the Tomcat instance to shut itself down. This port is defined at the top of the server.xml file for the instance.

{% highlight ruby linenos %}
<Server port="8001" shutdown="_SHUTDOWN_COMMAND_" debug="0">
{% endhighlight %}

Make sure each instance uses a different port value. The port value will normally need to be higher than 1024, and shouldn’t conflict with any other network service running on the same system.

Unlike the other ports Tomcat listens to, the shutdown port can’t be configured to listen to its port on a different IP address. It always listens on 127.0.0.1.

Startup
-------

Startup scripts are a whole other topic, but here’s the brief rundown. The main different from running a single Tomcat instance is you need to set CATALINA_BASE to the directory you set up for the particular instance you want to start (or stop). Here’s a typical startup routine:

{% highlight ruby linenos %}
JAVA_HOME=/usr/java
JAVA_OPTS="-Xmx800m -Xms800m"
CATALINA_HOME=/usr/local/tomcat
CATALINA_BASE=/var/tomcat/serverA
export JAVA_HOME JAVA_OPTS CATALINA_HOME CATALINA_BASE
$CATALINA_HOME/bin/catalina.sh start
{% endhighlight %}