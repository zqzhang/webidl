# WebIDL

Research on WebIDL fragments in specifications and web engines.

My initial thought is to create an IDL index for all the web platform
specifications that [Crosswalk Project](https://crosswalk-project.org/) cares
about, and to get a whole view of Web APIs it supports.

To my knowledge, Blink web engine that the Crosswalk Project relies on has some
issues of its IDL fragments conforming to the W3C standard WebIDL. Thus we
cannot leverage
[idlharness.js](https://github.com/w3c/testharness.js/blob/master/idlharness.js)
based test cases in Crosswalk Project testing.

Searching `webidl` in GitHub, I find some great repositories:

* [heycam/webidl](https://github.com/heycam/webidl): primary repository in which
  the [Web IDL specification](https://heycam.github.io/webidl/) is developed.
* [darobin/webidl2.js](https://github.com/darobin/webidl2.js): WebIDL parser.
* [extensibleweb/webidl.js](https://github.com/extensibleweb/webidl.js): an
  implementation of WebIDL in ECMAScript.
* [othree/webidl](https://github.com/othree/webidl): WebIDL files from Mozilla.
* [dontcallmedom/webidl-checker](https://github.com/dontcallmedom/webidl-checker):
  source code for the
  [W3C on-line WebIDL checker](http://www.w3.org/2009/07/webidl-check?), a tool
  verify the correctness of WebIDL fragments embedded in HTML documents.

Then I realize it is better to figure out the difference of WebIDL usage between
specifications and web engines, moving forward from the IDL index.

# WebIDL Files

All webidl files are from the latest specifications and web engines source code
repositories.

* https://mxr.mozilla.org/mozilla-central/source/dom/webidl/