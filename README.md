GAnalytics
=============================
A Google Analytics native extension for OpenFL
-----------------------------

This OpenFL native extension allows you to integrate Google Analytics ( v3.03 ) into your OpenFL application.
The supported compilation targets are [iOS](https://developers.google.com/analytics/devguides/collection/ios/v3) & [Android](https://developers.google.com/analytics/devguides/collection/android/v3/)

Installation
------------
There is an [include.nmml]() file and [ndll]() are compiled for:
* ios armv6
* ios armv7
* ios simulator
* android armv6

Recompiling
-----------
For recompiling the native extensions just use the sh files contained in the project folder.

Usage
-----
Just call the public methods on the HypGA class.

For iOS you need to link the Google Analytics class package to your XCode project.
Just drag & drop on your project the HypGA folder. ( [your_export_folder]/ios/[ProjectName]/HypGA )

Baisc reference
---------------

First start the session via :
<pre><code>HypGA.startSession( "YOUR-UA-CODE" );<code></pre>

Tracking a page view :
<pre><code>HypGA.trackPageView( "your-page-code");<code></pre>

Tracking an event :
<pre><code>HypGA.trackEvent( "event-cat" , "event-action","event-label",1);<code></pre>

For more advance methods just take a look a the HypGA class.
All the Google Analytics V2 methods are supported( timing, metric , social , dimension... )

This project was Originally forked from HypGA by Hyperfiction
--------------------
[hyperfiction.fr](http://hyperfiction.fr)

License
-------
This work is under BSD simplified License.
