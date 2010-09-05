The Bakery
==========

An experimental web application platform for [The Fireworks Project].
---------------------------------------------------------------------
The Bakery is a web application sandbox of sorts.  [The Fireworks Project] will
use it to try out new ideas for web applications, but you are free to use it
however you see fit.  The Bakery is designed to run on the [Google App Engine]
platform and we have no plans to port it to any other platform. However, the
lessons we learn from the experiments we run in The Bakery should carry over to
any platform we might want to use in the future.

Ultimately we intend to create a platform that will allow us to rapidly develop
and deploy complex web applications by joining together many components that
are much simpler and easier to understand. In addition, we want to move all of
the logic of the applications to the client, and leave the servers to handle
data storage only.

The problem is that we don't really know how we want to achieve all this
awesomeness. The goal of The Bakery is to allow us to take baby steps in the
directrion we want to go. More than anything, The Bakery will be a learning
tool that will allow us to perfect our craft and take over the World.


The Bakery has the tools we need to continue building applications for our
customers while experimenting with our ideas for modular design -- all on the
same platform. If this experiment goes according to plan we'll learn some
valuable lessons and apply them to a future platform in a galaxy not so far
away.

Architecture
------------
### Multitenancy
The Bakery is designed to be a multitenancy application server, which means
that a single instance of it may serve multiple client organizations known as
tenants. This architecture allows it to be a cost effective and highly
scalable application server for what we hope will be many high paying
customers.

### Datastore
The Bakery includes an HTTP API which is simply hooked directly into the GAE
datastore API. The HTTP datastore API allows JavaScript code on the client to
store and query data from the server.

### Libraries
The Bakery also maintains and dishes out JavaScript, HTML, and CSS libraries
that are commonly used by most of the applications that will run on it. This
includes jQuery, HTML and CSS for common interface widgets, jQuery UI, and
more.

Usage
-----

### Quick start.

#### Install Python
The Bakery is built to run on the GAE Python runtime, so you will need to
install Python 2.5 before going any further. If necessary, download and install
Python 2.5 for your platform from the [Python] web site. If you are using Linux
or Mac OS X 10.5 Leopard then give yourself a pat on the back, because Python
is probably already installed. To find out, open a terminal and type `python
--version` and hit enter. You should see something like `Python 2.5.2` diplayed
on the command line.

### Install The Bakery
Download the latest release of [The Bakery]. You'll get a zip file named
something like `thebakery_0.1.zip`. Move it to wherever you want it on your
computer and unpack it. A directory called `thebakery` will be created
automatically. It will contain all of the necessary files to start baking web
applications.

### Install the inspector. 
The first application you'll want to install into the bakery before you get
started is the *Bakery Inspector*. It will allow you to run tests on The Bakery
as well as your other apps to see if they are healthy for consumption.

To install any app, including the *Bakery Inspector* you need to have it located
someplace on you computer. There are a number of ways to achieve this, which we'll
go over later, but you can get the *Bakery Inspector* by downloading the latest
release from [The Bakery] download page. You'll get another zip file that looks
something like `bakeryinspecter_0.1.zip`. Move it to wherever you want it on your
computer and unpack it. A directory called `bakeryinspector` will be created
automatically. It will contain all of the necessary files to start inspecting
your Bakery apps.

### Run the inspector.
To run the inspector move to `thebakery` directory (where you installed The
Bakery) and type `./app run /path/to/bakeryinspector/` where
`/path/to/bakeryinspector` is the actual path to the location where you
installed the *Bakery Inspector*. Once it is running, set your web browser to
`http://localhost:8080/inspector/` and take it from there.

FOSS
----
Although The Bakery is *free and open source software* it is still in the early
stages of development. So, unless you are a glutton for hair pulling
frustration you might want to look around the source code a bit before trying
to use it. Better documentation will certainly help, and we will expand the
documentation as the project grows.

Copyright and License
---------------------
copyright: (c) 2010 by Fireworks Technology Projects Inc., see AUTHORS for more
details.

Unless otherwise indicated, all source code is licensed under the MIT license.
See MIT-LICENSE for details.

And, unless otherwise indicated, all content, including written copy and images
but not including source code, is licensed under a Creative Commons
Attribution-ShareAlike 3.0 Unported license. All derivatives of this content
must be attributed to
["The Fireworks Project"](http://www.fireworksproject.com/). See
[creativecommons.org/licenses/by-sa/3.0/](http://creativecommons.org/licenses/by-sa/3.0/)
for more details.


  [The Fireworks Project]: http://www.fireworksproject.com
  [Google App Engine]: http://appengine.google.com/
  [Python]: http://www.python.org/
  [The Bakery]: http://www.fireworksproject.com/projects/
