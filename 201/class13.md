# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

This article starts with talking about the challenges that the early web applications suffered in the local storage area.

An early solution for that problem was cookies, but had several problems

+ Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

+ Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

+ Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

Then they give a brief about the history of local storage hacks before *HTML5* was introduced.  

After that, HTML5 storage was introduced or as it is called *Web Storage*.  

They then explain using HTML5 storage and how to track changes to the HTML5 storage area, and its limitations in current web browsers.  