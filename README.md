README for myapp
==========================

The current errors are:

At startup (mvn spring-boot:run)
---------------------------------

`
WARN] com.mangofactory.swagger.plugin.SwaggerPluginAdapter - SwaggerSpringMvcPlugin have already been initialized!
`

Then, when accessing http://localhost:8080
------------------------------------------

On the JavaScript console

`
WebSocket connection to 'ws://localhost:8080/websocket/activity?X-Atmosphere-tracking-id=0&X-Atmosphere-Framework=2.2.5-javascript&X-Atmosphere-Transport=websocket&X-Atmosphere-TrackMessageSize=true&Content-Type=application/json&X-atmo-protocol=true' failed: Error during WebSocket handshake: Unexpected response code: 501

Websocket failed. Downgrading to Comet and resending
`

Login as admin and then going to the User Tracker
-------------------------------------------------

The list is empty at first

Swagger errors keep popping

`
WARN] com.mangofactory.swagger.plugin.SwaggerPluginAdapter - SwaggerSpringMvcPlugin have already been initialized!
`

also some

`
[ERROR] org.atmosphere.cpr.AsynchronousProcessor - Invalid request state. Websocket protocol not supported
`

in the JavaScript console

`
 Synchronous XMLHttpRequest on the main thread is deprecated because of its detrimental effects to the end user's experience. For more help, check http://xhr.spec.whatwg.org/.
 
 No suspended connection available. Make sure atmosphere.subscribe has been called and request.onOpen invoked before invoking this method atmosphere.js:3117 
 atmosphere.util.log atmosphere.js:3135 
 atmosphere.util.error atmosphere.js:2428 
 _push atmosphere.js:2806 
 atmosphere.AtmosphereRequest.push app.js:235 
 $rootScope.websocketRequest.sendMessage app.js:228 
 $rootScope.websocketRequest.onClose atmosphere.js:2689 
 _f atmosphere.js:2632 
 _invokeFunction atmosphere.js:2750 
 _invokeCallback atmosphere.js:2711 
 _invokeClose atmosphere.js:1814 
 atmosphere.AtmosphereRequest.ajaxRequest.onabort atmosphere.js:466 
 _clearStateatmosphere.js:1558 (anonymous function)
`

 After a long long time, content appear to the page.
