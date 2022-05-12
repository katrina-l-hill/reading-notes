# Class 13 - Local Storage

## The Past, Present & Future of Local Storage for Web Applications

### Diving In

- In native applications, an abstraction layer for storing and retrieving application-specific data is usually provided by the operating system.
- The values may be stored in different types of files on the computer, such as the registry, INI files, XML files, or other similar files.
- Cookies were invented in the early days of the internet and can be used to provide local storage for some data.
- The downsides of cookies are that they are included in every HTTP request, so this slows down web applications by constantly transmitting data over and over.  
- Another downside of cookies being included in every HTTP request is that it sends unencrypted data over the internet unless your whole web application is served over Secure Sockets Layer (SSL), which is a standard security technology for encrypting data.

### A Brief History of Local Storage Hacks before HTML 5

- Internet Explorer (IE) used to be the only web browser people could see.
- Microsoft invented IE to be the main browser people would use, and in order to do that, they invented DHTML Behaviors and userData.
- userData provided more storage to web pages by being able to store up to 64 KB of data per domain.
- Over the years, Adobe Flash, AMASS, Google Gears, dojox.storage, and Adobe AIR were all invented as ways to store browser data.
- These were all prototypes for HTML5.

### Introducing HTML5 Storage

- HTML5 Storage is like cookies in that it is a way  for webpages to store key/value pairs locally within the client web browser.
- Unlike cookies, the key/value pairs are not transmitted over the internet to the remote web server.
- HTML5 is implemented natively in web browsers, so it’s available even when third-party plug-ins are not.

### Using HTML5 Storage

- In HTML5 you store data based on a named key, then you retrieve the data by the same named key.
- You can type the data using strings, Booleans, integers, or floats, but the data is actually stored as a string, so you will need to write functions if you are storing or retrieving the data as anything other than a string.
- In order to track changes to the storage area, you will need to create storage events that are called on to make the changes.

### Limitations in Current Browsers

- The limitation for storage space at each origin is 5 megabytes. This storage is for strings, not data in its original format.  
- An exception of “QUOTA_EXCEEDED_ERR” will be thrown if you exceed the 5 megabytes limitation.
- As of this article, there is no browser that will support giving more storage space above 5 megabytes.
