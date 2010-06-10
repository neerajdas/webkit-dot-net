WebKit.NET README
*****************

WebKit.NET is a control library wrapper for WebKit written in C#.

The source code is licensed under a BSD open source license, see
LICENSE.txt for details.

This package contains two Visual C# 2008 in the following directories:

    WebKitBrowser - WebKit.NET control library.
    
    WebKitBrowserTest - A simple web browser that uses the WebKit.NET control
                        to display web pages.
                        
    webkit - WebKit libraries and dependencies (not included).
                        
The current releases are at a very early stage of development and are not
recommended for production level use yet.

Please send any questions or feedback to Peter Nelson at charn.opcode@gmail.com


Requirements for building
*************************

To build the source code provided in this release you must use either Visual
Studio 2008 or Visual C# Express 2008.  With a bit of work it should be
possible to get it to build under 2005 or Mono.


Requirements for using
**********************

This source package does not include WebKit or any of it's dependencies, which
are required to use WebKit.NET.  Currently, it has been tested with both the
Apple and Cairo ports of WebKit.  Many of the dependencies required by Apple's
port are non-redistributable, however they are included with Safari which is 
free to download.  If you wish to use WebKit.NET with the Apple port, you can
download a nightly build of WebKit from nightly.webkit.org.  The dependencies
for the nightly builds can be found in the Safari installation directory.

The Cairo build and it's dependencies are all freely redistributable, however
the port is not yet complete (for example, downloading files is unimplemented).
If you wish to use this build of WebKit, the WebKit.NET-x.x-bin-cairo package
contains everything that is needed.
