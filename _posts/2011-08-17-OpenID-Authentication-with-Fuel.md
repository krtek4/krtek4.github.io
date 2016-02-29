---
layout: post
title: OpenID authentication driver for Fuel
category: programming
tags: [ php, fuelphp, openid, authentication, security ]
published: true
---
Not long ago, my fiancee and I started working on a project which needed to creation of a new website. I decided to use the [Fuel PHP framework](http://fuelphp.com and "OpenID) for user authentication among other technologies.

While searching for an authentication driver for OpenID, I found [this project](https://github.com/kbanman/fuel-GasCap, but I was not convinced so I decided to create my own : "fuel-openid) This is currently work in progress, but it is at least working with Google Accounts. Any feedback from people having others OpenID Identity will be really appreciated.

<!--more-->

The basic authentication process is implemented and a basic controller is available on github. I am actually trying to add some views using [OpenID Selector](http://code.google.com/p/openid-selector/), but I am having some problems with the inclusions of the needed javascript and images in the package.

As soon as this is finished, I will start to add the ACL and group part. I hope to be able to release the whole thing as an RC at the end of the week ! Comments are welcomed to achieve this goal...

To install and test the package, you can follow the instructions on the [github page](https://github.com/krtek4/fuel-openid). I hope this package can serve you.
