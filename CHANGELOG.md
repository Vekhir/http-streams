* _v0.8.9_
    Ongoing maintenance continues, including support for GHC 9.2 and GHC 9.4

* _v0.8.6_  
	Internal modules are exposed. Mostly so the test suite would only
	depend on the library and not the code directly, but occasionally
	someone needed to poke at the internals. Usual warning against
	doing that applies. They are _not_ visible in the generated Haddock
	documentation.

* _v0.8.4_  
	Support GHC 8.0

* _v0.8.3_  
	A pure version of `buildRequest` is now available as `buildRequest1`.
	Support for connecting to Unix domain sockets has been added.

* _v0.7.0_  
	The Request, Response, Headers, and RequestBuilder types have been
	factored out and moved to **http-common**. They are still exported
	by **http-streams**.

* _v0.6.0_  
	Entity body lengths (both for Requests and Responses) now Int64.
	Library depends on **io-streams** 1.1.

* _v0.5.0_  
	Definition of Hostname and Port have been changed to ByteString
	and Word16, respectively.

* _v0.4.0_  
	Type signature of `buildRequest` changed, removing the Connection
	parameter. This allows you to construct Request objects before
	opening a connection to the web server if you wish.

* _v0.3.1_  
	Initial public release
