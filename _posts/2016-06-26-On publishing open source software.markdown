---
layout: post
title:  "On publishing open source software"
date:   2016-06-26 12:02:00
categories: [projects]
author: "Bruno Henriques"
tags:
- C#
- .Net
- Nuget
- Open-source
- Cocoapods
- iOS
- Wpf
- Log4Net
- Xml
- Swift

containscode: false
---

Hello,

Throughout the development of several projects I have been working on, for example, the Malaria-iOS, the Técnico Lisboa App and even, more recently my MSc thesis on Rapport, I have been noticing the potentiality of moving some of the developed code to a separate self-contained module that could be useful for other developers as well. For this purpose, I have been actively learning how to share my work with other developers.

My goals when publishing these modules are:

* Reduce the required boilerplate code to develop common use-cases (this also applies to any development environment);
* Ease the workload of other developers that encounter the same issues these modules aim to solve.

However it is not easy:

* Assuring that the code is not hanging my wires;
* Assure that what is accessibly publicly is well documented and easy to understand;
* Assure (for everybody) that the modules are stable and work as intended by developing unit tests;
* Be careful with version semantics;
* If you publish, you should provide a readme;
* If you publish, you should ideally provide a demo project;
* If you publish, you have to maintain the project (you should at least...).

As of this moment, I developed the following Cocoapods modules and Nuget Packages.

* [NetObjectToFileWritter](https://github.com/bphenriques/NetObjectToFileWritter) - Import/Export Xml and objects, useful for configuration files;
* [Log4NetWrapperLite](https://github.com/bphenriques/Log4NetWrapperLite) - Wraps some log4net use cases and provides mechanism to use it with a RichTextbox (stylish log);
* [HelpersForNet](https://github.com/bphenriques/HelpersForNet) - Just a set of useful C# extensions.
* [done-toolbar-swift](https://github.com/bphenriques/done-toolbar-swift) - Adds a conveninent and intuitive done button on every input view;
* [EKEventStoreWrapper](https://github.com/bphenriques/EKEventStoreWrapper) - In development. Wraps the mechanism to export and import events to the native iOS calendar;
* [PickerSwift](https://github.com/bphenriques/PickerSwift) - Wraps the UIPicker and reduces the boiler plate code to provide this inputs to the user;
* [CircleProgressView](https://github.com/bphenriques/CircleProgressView) - Circular progress view;
* [HorizontalProgressView](https://github.com/bphenriques/HorizontalProgressView) - Horizontal progress view.

I salute every developer who develops and maintains their public libraries. From the little experience I had, it's cumbersome to maintain modules. For example, after the Swift 2 release, Malaria-iOS was failing because I haven't updated the modules yet to the newer version of Swift. Unfortunatly, or fortunatly (I don't know), haven't been receiving feedback on the modules I have been developing. I believe, that NetObjectToFileWritter, the PickerSwift and EKEventStoreWrapper are really useful for the developers.

The current state of these projects are not perfect I am aware. Why? Because I think they should all have:

* A demo project (some of these projects already have!);
* Unit tests with a nice stamp on the repository readme.

For every developer who stambles upon my code, I hope that it delivers what you expect and if you ever feel frustrated with it please let me know. For me, it has been a enriching experience!


See ya!

Bruno Henriques