---
title: "Changing Project Name On Android Studio"
datePublished: Fri Dec 04 2020 15:12:01 GMT+0000 (Coordinated Universal Time)
cuid: ckiaf74ay009xqrs116s0490d
slug: changing-project-name-on-android-studio
tags: android-app-development, android-studio

---

Sometimes, the need to change a project name or directory in Android Studio arises; for this reason, I have decided to write an article on how to get that done. It is easy; there's absolutely nothing to worry about. Although I had already answered a question concerning this on StackOverflow, you might want to check that out ASAP.

## A quick way of doing this is by the following steps

* hit the shift key twice, a pop-up will show up, search for a file named "settings.gradle" when it opens, change the `rootProject.name = "Old-name"` to `rootProject.name = "new name"` then sync.
    
* hit the shift key twice, a pop up will show search for a file named `"string.xml"`, when it opens change `<string "app_name">old-name</string>` to `<string "app_name">new-name</string>`
    
* close android studio
    
* locate androidStudioProject directory on your machine, open it and find the project by its old name, rename it to the new name.
    
* open Android Studio goto File &gt; Open &gt; "new name". open it from there
    

#### This is currently working on Android Studio 4.1.1

I hope this works for you, do well to upvote my answer on [StackOverFlow](https://stackoverflow.com/a/64935048/12002890) if it works :)