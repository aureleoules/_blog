---
title: Introduction to AngularJS
---
## What is Angular ?

AngularJS is a <b>powerful open source JavaScript framework</b> for web applications. It was originally developed in 2009 by Misko Hevery and Adam Abrons. It is now maintained by Google.

##Advantages

- AngularJS allows you to use <b>MVC</b> (Model View Controller), which means you can do a website with one single page, usually the <code>index.html</code> file.
- AngularJS uses <b>dependency injection</b>.
- Write <b>less</b> code!
- AngularJS can run on <b>every</b> web browsers (Even Internet Explorer!).

##Features

- ###<u>MVC</u>:
It splits an application intro different parts (<b>Model</b>, <b>View</b>, and <b>Controller</b>) to create a <b>Single Page</b> web Application.
- ###<u>Data Binding</u>:
<b>Sync</b> data between the <b>model</b> and the <b>view</b>.
- ###<u>Scope</u>:
It's an <b>object</b> that refers to the application model. The link between <b>controller</b> and <b>view</b>.
- ###<b><u>Controllers</u>:
Functions bound to a specific <b>scope<b>.
- ###<u>View</u>:
What the user <b>sees</b> (the DOM).
- ###<u>Services</u>:
These are substitutable objects that are wired together using <b>dependency injection</b>. AngularJS come with <b>several built-in services</b> for example $http to make a XMLHttpRequests.
- ###<u>Filters</u>:
<b>Format</b> the value of an expression to display a <b>new</b> one. They can be used in <b>view templates</b>, <b>controllers</b> or <b>services</b>.
- ###<u>Directives</u>:
Directives are <b>markers on DOM elements</b> (such as elements, attributes, css, and more). These can be used to create <b>custom HTML tags</b> that serve as new, custom widgets. AngularJS has built-in directives (ngBind, ngModel...)
- ###<u>Templates</u>:
Templates are written with <b>HTML</b> that contains Angular-specific elements and attributes. Angular combines the template with information from the <b>model</b> and <b>controller</b> to render the dynamic <b>view</b> that a user sees in the browser.
- ###<u>Routing</u>:
Way to <b>switch</b> to different <b>views</b>.

##Components

The AngularJS framework is divided in 3 main parts:

- <b>ng-app</b>: It defines and links an AngularJS application to HTML.   
- <b>ng-model</b>: This directive binds the values of AngularJS application data to HTML input controls.
- <b>ng-bind</b>: This directive binds the AngularJS Application data to HTML tags.
