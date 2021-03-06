---
layout: post
title: Online Authenticator
category: programming
tags: [ php, battle.net, authenticator, project ]
published: true
---

A long time ago, when I was still playing World of Warcraft, I started using a Battle.Net Mobile Authenticator to secure my account. After some time, the burden of always having my phone with me when I wanted to play was too much and I decided to find another solution. Since the specification were known, some desktop implementation were written. I adapted one of them to publish my Authenticator code somewhere on the internet, accessible from anywhere as long as you had my password ;)

<!--more-->

When I stopped playing, I adapted this script to display the Authenticator of a friend. Sadly, when I moved my old dedicated server content to the new instance, I lost my modifications and I didn't found the time to made them again. My friend was forced to use his phone again !

Now that I had some time to think about it, I decided to write my [own PHP implementation](https://github.com/krtek4/php-bna) of the specification. My plan is to use this little project to create a website allowing everyone to host their authenticator online and be freed of the burden of carrying a device to access his account in a secure way.

For now, [Online Authenticator](http://authenticator.me) is still in beta. The Authenticator part is working, my friend is already using it, but other parts of the site need some polish ! I plan to release this little webapp before the end of October. If you want to help me, feel free to contact me so we can discuss an access to the beta...

By the time of the release, I'm planning to offer the possibility to generate new Authenticators or re-use the current one for those using an Android version. Sadly, I don't know a way to retrieve the necessary informations from the iPhone version, if you know something about that, I'm all ears.

I hope this project could benefit not only my friend... If you're interested or if you have ideas, let me know in the comments !

*UPDATE:* The [Online Authenticator](http://authenticator.me) is finally released. Go check it out ! The Authenticator is fully compatible with Blizzard's Battle.Net Mobile Authenticator. You can play World of Warcraft of Starcraft without any problem. A complete post about this is coming...
