# cordova-api-fetch
An app built with Cordova-PhoneGap for fetching API, https or http request.

Please, cover my another cordova repository first, so it will be easy. <br>
https://github.com/ronycse778/cordova-phonegap-android-studio

For API server I use this repository <br>
https://github.com/ronycse778/laravel-simple-rest-api

Type ipconfig in CMD, to find pc ip. suppose(192.168.68.108) <br>
Clone the API server repository and follow processes and run with
<pre>php artisan serve --host=0.0.0.0</pre>
So, basically the server will run in <code>http://192.168.68.108:8000</code> <br>
If server is ok, it can be checked with the link <code>http://192.168.68.108:8000/api/v1/users</code> in browser. <br>
No login is required. <br>

As this link is http server so, a cordova advanced http plugin is required.
Install it in app project by
<pre>cordova plugin add cordova-plugin-advanced-http</pre>

To show bug, output or anything in android studio console add
<pre>cordova plugin add cordova-plugin-console</pre>

<b>After importing the project to android studio,</b> to bind this ip(192.168.68.108) <br>
1. Update your AndroidManifest.xml to use the network security configuration. <br>
<application <br>
        android:networkSecurityConfig="@xml/network_security_config" <br>
        ... > <br>
    </application> <br>
2. Create a file named network_security_config.xml in the res/xml directory of your project (create the xml directory if it doesn't exist). <br>
content of this xml not shown in here, so check it from snapshot from Data.Source folder

<b>To use this repository:</b> <br>
Clone it, unzip node_modules.zip, platforms.zip, plugins.zip <br>
Change ip address from www folder/index.html file. <br>
Check app ouput snapshot. <br>

Done
