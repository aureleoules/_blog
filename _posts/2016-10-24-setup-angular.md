---
title: Setup AngularJS
---
##Download AngularJS  

There are multiple ways to download and use **AngularJS**.  

- You can use the [Google CDN](https://developers.google.com/speed/libraries/#angularjs) using:  

{% highlight html linenos %}

<!DOCTYPE HTML>
<html ng-app="myApp">
    <head>
        <title>AngularJS App</title>
        <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.5.8/angular.min.js"></script>
    </head>
    <body>
    ...
    </body>
</html>

{% endhighlight %}  
**Note** that only versions 1.0.1 and above are available on the **CDN**. If you need an earlier version (which you **shouldn't**) you can use the [https://code.angularjs.org/](https://code.angularjs.org/) URL, which was the previous recommended location for hosted code source. If you're still using the Angular server you should switch to the CDN version for even faster loading times.

- Using **Bower**:  
<code>bower install angular</code>  
Or use a **specific version** of Angular:  
<code>bower install angular#1.2.0</code>
- Using **GitHub**:  
<code>git clone -b master https://github.com/angular/angular.js.git</code>
- Using **NPM**:  
<code>npm install angular</code>  

##Quick example:  

Make a simple HTML page including the **AngularJS library and a JavaScript file** called <code>app.js</code> like:  

{% highlight html linenos %}
<!DOCTYPE HTML>
<html>
    <head>
        <title>Simple App</title>
        <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.5.8/angular.min.js"></script>
        <script src="app.js"></script>
    </head>
    <body>
    </body>
</html>
{% endhighlight %}  

**Then** add to the <code><html></code> tag: "**ng-app="myApp"**.  

In your <code>app.js</code> file, write the following:  

{% highlight javascript linenos %}
var app = angular.module('myApp', []);
app.controller('myCtrl', function($scope) {
    $scope.myText = "Hello World!";
});
{% endhighlight %}  
**Go back** to your html file and add to the <code><body></code> tag :  
<code>ng-controller="myCtrl"</code>.  
And in your body add a <code><h1>{% raw %}{{ myText }}{% endraw %}</h1></code>.  

It should looks like this:  
{% highlight html linenos %}
<!DOCTYPE HTML>
<html>
    <head>
        <title>Simple App</title>
        <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.5.8/angular.min.js"></script>
        <script src="app.js"></script>
    </head>
    <body ng-controller="myCtrl">
        <h1>{% raw %}{{ myText }}{% endraw %}</h1>
    </body>
</html>
{% endhighlight %}  

**Now** open your html file and admire a wonderful :  

#Hello World!
