# twpdfexport

Extension uses Selenium Chrome driver. It does not rely on JavaFX. IT can be used with any OpenJDK 11 and higher. 

You need to have ChromeDriver + Chrome browser (Chromium gost) installed for this extension to work.  

For AppKey to be passed as Header oposed to URL parameter LittleProxy is used. Upon service invocation (exportPDF) LittleProxy opens random port within the 50000-51000 range which is bound to all IPv4 interfaces on machine where ThingWorx is located (0.0.0.0). This process it transparent so from user point of view no changes are needed. 

Simply fill the URL with:
`http(s)://localhost:<TomcatPort>/Thingworx/Mashups/<yourMashup>`

Dont forget the AppKey with appropriate permissions set.

