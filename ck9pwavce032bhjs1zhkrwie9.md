---
title: "Creating Your First android App in Kotlin for Complete beginners"
datePublished: Wed Jul 17 2019 20:30:00 GMT+0000 (Coordinated Universal Time)
cuid: ck9pwavce032bhjs1zhkrwie9
slug: creating-your-first-android-app-in-kotlin-for-complete-beginners

---



![creating your first Android app using kotlin.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586717475483/giQ7orAaO.jpeg)

# Build your First Android App with Kotlin
 Android is an  [Open Source Operating System](https://www.zdnet.com/article/what-are-open-source-operating-systems-everything-you-need-to-know/ "Meaning of: OSOS") it allows just any body to contribute and improve it Usability . The need for an Android Developer increases day by day due to the numbers of users operating on the Android device.
 

> 
*Android has been the best-selling OS worldwide on smartphones since 2011 and on tablets since 2013. As of May 2017, it has over two billion monthly active users, the largest installed base of any operating system, and as of January 2020, the Google Play Store features over 2.9 million apps.*
                  -Wikipedia

Making an android application is a thoughtful decision since your app will capture high range of users.

## Making an android application.

In other to create an android application, a developer has to have hands on the following tools


- Android Studio IDE and SDK 

- A prior knowledge in either Java/Kotlin programming language 

- Android Emulators


The above tools are the basic tools necessary to write an Android Application. 
Although, it may vary depending on the kind of android project you are creating.

## Android Studio IDE and SDK

Android Studio is an Integrated Development Environment (IDE) that is officially use for the development of android applications, built on JetBrains IntelliJ IDEA software. you don't have to be overwhelmed by the grammatical terms used, you can imagine *Android studio* as a normal **text editor** like : *notepad* , *Sublime text*, *visual studio code* etc with extra functionalities to help you manage your code effectively. The *Android Studio IDE* is available for download in the [Developers website](https://developer.android.com/studio "Click to download Android studio"). I will work you through downloading and installing of the *Android Studio IDE and SDK* later on in this article.

## A prior knowledge in either Java/Kotlin programming language 

Before a developer can create an android app he/she has to have a proper understanding of either *Java* or *Kotlin* programming language. In case you don't know what a programming language is, A *programming language* is a language that helps us carry out complex computer instructions in form of code, they are use to communicate to the machine  using almost normal human readable language.

The java programming language is an Object Oriented Programming language (OOP) which was formly the primary language supported by google for writing android applications but later on, Google announced that a programming language called *Kotlin* can also be used for programming *android applications*. In 2019, Google announced that *kotlin* is now the primary language for writing android application. 


> 
*On 7 May 2019, Google announced that the Kotlin programming language is now its preferred language for Android app developers. Since the release of Android Studio 3.0 in October 2017, Kotlin has been included as an alternative to the standard Java compiler.* -Wikipedia

%[https://youtu.be/ukm_RXxw4Yc]

Despite the fact that *kotlin* is now the primary language for *Android*, you can still use *Java* to write Android apps but, i will strongly advice you use *Kotlin* because, it's easier than java. Although, *Kotlin* is just full of Extension function and Extension properties from the standard *Java* library or we can just say *kotlin* is built on *Java's* Virtual Machine(JVM). 
The both language can be used at the same time in one project and Android Studio makes things easy because Android studio can convert code written in Java to *kotlin* and vise versa, just by simply copying a *Java* code to android studio, it will suggest converting the code to *Kotlin* and if permissions are granted the code will be successfully converted to *Kotlin*.  one of the cons of *java* is the billion dollar **NullPointerexception** which cause app to crash at run time, *Kotlin* handled the **NullPointerException** by making all types  in mutable( types cannot be nullable ) by default. The nitty-gritty of all this is that *Kotlin* helps to create android apps easier as opposed to *java*. 

In our own case we will be using **KOTLIN** 


## Android Emulator

In computing, an emulator is a hardware or software that enables one computer system (called the host) to behave like another computer system (called the guest). 
An Android Emulator is a software that is pre-installed in our *Android Studio*  which allows us test our finished apps. *Android Emulators* are simple software application that mirrors an actual android device with almost all the functionalities of a real android device. Although, not only Android Emulators can be used for app testing, our physical android device can also be used to test our application, All we have to do is to connect our physical android device to our computer using the Universal Serial Bus(USB). Before we can install our android apps in our physical *Android* device, we have to enable USB debugging from the Developers option in our *Android* device. i will work you through that later on in this article.

## App Description

We will be building your first Android app together, we will build a very simple Android calculator that carry out normal calculation functionalities like Add, Subtract , Multiply and Divide. After we are done with the project our new application should look like the image below.

![2020-05-02 14.47.15.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1588427488953/mE80AHGVN.jpeg)

Dowload the entire source code for this project [here](https://www.github.com/mubaracktahir/calculator "click to clone or download from git hub")
## Setting up Environment 

### **Step 1**
- Download *Android Studio IDE*
 **NB**  before you can download *Android Studio* your computer has to meet the following 
requirements 


![Screenshot (107).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586782160534/_QgvFXAkw.png)

if your computer meet the above requirements download *Android Studio* [here.](https://developer.android.com/studio  "click to download android studio")

Downloading *android studio* consumes a lot of data and time. So, you might want to connect to a *wifi*. Then sit back and relax with a cup of coffee while you wait for android studio to be successfully installed in your computer.
if android studio has been successfully installed, it will automatically open and your environment should look like this.

#### *The loading screen*

![Screenshot (108).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586804096004/6jdBItuvG.png)

If your loading screen looks different from mine don't panic we are still on the same environment, it just that you might either be using an older version of *android studio* or at the time you are reading this article another version of the android studio might have been built and released. So, for every new version of *android studio* the loading interface changes. 
   
#### The preceding screen after it loads


![Screenshot (110).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586805615021/PHzWpKBQ2.png)


In the above screen select the first option titled ** *start a new android studio project* **
after which you have selected that, a pop up window that looks like the below one will pop up prompting you to select a template.


![Screenshot (112).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586806115783/0Uo9oZEGF.png)
 


select ***empty activity*** and click ***next***.


In the next pop up window,put the name of the project as **Calculator**,make sure the **language**
is set as *Kotlin*. Then, leave every other things as it is and click **finish**.


![Screenshot (113).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586807208419/ao19vShr1.png)


your Final screen should look like this:


![Screenshot (114).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586807691688/30PSpLcBf.png)

this is where we write all our codes  and UI for the application.

cheers! we have finally set up our environment.

### **Step 2**

- Final step, starting  an Emulator.
 watch this video below created by [Vlad Voytenko](https://www.youtube.com/channel/UCq0BPYTmAz5x6qyQn-wHhcA) to understand how to create *Emulators* from within *android studio*
%[https://youtu.be/du8XaKw0jO0]

if you want to watch the above video in full screen click [here](https://youtu.be/du8XaKw0jO0)

Now that we have everything we need, **lets get coding!!!**

## Coding The UI
Its a good practice to always start with the User Interface(UI) part of a project. If you are wondering what a **UI** is, **UI** is the physical part of an application, it is the part that the user interacts with. A very good examble of *UI* is the one we have below

![2020-05-01 11.18.21.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1588427181138/BaSSPvwZZ.jpeg)

So, we will start by creating the *UI* of this app

In android, a folder called `res` is the folder where all the code that has to do with the UI are stored. In other to create our UI, we have to navigate to the `res` folder from within *android studio*, i will guide you through the processes involve in coiding the UI. First, let figure out a way to reach the `res` directory in our *andorid studio*. i will illustrate a step by step guide to reach the `res` directory in the disgram below.


![Screenshot (119).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982088537/bChhCT5ih.png)

![Screenshot (120).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982096699/bsDfxGCKW.png)

![Screenshot (121).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982151663/KdO7tTjDC.png)

![Screenshot (123).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982177622/RjHdS3bQ_.png)

![Screenshot (124).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982201587/iYG0FEjDD.png)

![Screenshot (126).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586982209052/6thXQpSyG.png)

In the `activity_main.xml`, copy and paste the below code in side. do make sure you clear the initial code in `activity_main.xml`

%[https://gist.github.com/d89ac4bd71b9e43805f0f28037e39094]

You will notice some errors after pasting the code, that because there are some files that we have to create that haven't been created.

Now lets create the files. Under our `res` directory in our `drawable` folder lets create a file called `button_click1.xml` and `button_click2.xml`, The work of these files are to add a **ripple effect** to our button when ever they are clicked. If you dont know what a *ripple effect* is, a *ripple effect*  is the circumstance in which one event instigates another event(s) , in a more friendly term it is the effect that happens on a button whenever they are clicked, they are in form of animation or coloration  that shows on a view or viewgroup(e.g button or Linearlayout *respectively*) when you click on them.


Lets locate the `drawable` directory which is located inside the `res` directory. Remember, the `res` directory is where all the code that as to do with our layout are stored.
You can do the job of scrolling up to see the illustration on how to locate the `res` directory. Afterwards, we can then find our `drawable` which is a sub directory in the `res` directory. 
follow the below navigation to find the `drawable` directory:

### `res` >  `drawable`

After which you have located the `drawable` directory **right click** and select **new**>**Drawable Resource File** a window will pop up prompting you to input *file name*, name the file "***button_click1***" as spelled then **hit enter or select Ok** to continue 

In the `button_click1.xml`, copy and paste the below code snippet into it. Make sure you clear the initial code in the `button_click1.xml` before pasting the below code.


%[https://gist.github.com/227e29767005a7f200996c94bb4c722c]


Now let's create the second `ripple` in similar procedure, name the file "***buttin_click2***" as spelled

In the `buttin_click2.xml`, copy and paste the below code snippet into it. Make sure you clear the initial code in the `buttin_click2.xml` before pasting the below code.

%[https://gist.github.com/bbad1371e05393e73ca30d4c73c72f11]


**We are almost done**, now that we have created the ripple effect for our views lets create another `drawable` resource which will serve as our **delete icon**. In similar way, create another `drawable resource file` and name the file "***clear***" as spelled in lowercase 

 In the `clear.xml`, copy and paste the below code snippet into it. Make sure you clear the initial code in the `buttin_clear.xml` before pasting the below code.

%[https://gist.github.com/16d9b8b524796abe4bb2d32422ad88d9]


#### Congratulations, we have completed 50% of our Application. 

if you try running the application, it will run but there wont be any effect when you click the buttons and that's because in **Android**, `.xml` files are use to create the UI of our `android applications` while `.kt` file which contains kotlin codes are use to specify the behavior of our UI more like what should happen when you click on a button or what should happen when u interact with any widget in the UI of an application All this are handled by the `Kotlin code`. 

Now that we know where our problem lies, lets wire our UI with  the kotlin code.

## Writing your First Kotlin Code 

Kotlin work almost like java, we will explore how to write your first kotlin on an online Kotlin compiler


```kotlin
fun main ( args : Array<String> ) {
    //the fun main is the main thread/method of a kotlin program just like java's PSVM ( public static void main ( String[] 
  // args )

   // this is the starting point of a kotlin code, any function that is not written or called in this block will not 
  //run
}
``` 
funny enough we wont be needing that to write `Android application`.

Click  [here](https://play.kotlinlang.org/#eyJ2ZXJzaW9uIjoiMS4zLjcyIiwicGxhdGZvcm0iOiJqYXZhIiwiYXJncyI6IiIsImpzQ29kZSI6IiIsIm5vbmVNYXJrZXJzIjp0cnVlLCJ0aGVtZSI6ImlkZWEiLCJjb2RlIjoiLyoqXG4gKiBcdGNyZWF0ZWQgYnkgTXViYXJhY2sgdGFoaXIgIG9uIDQvMzAvMjAyMC5cbiAqIFx0bXViYXJhY2sudGFoaXJyQGdhbWlsLmNvbVxuICogXG4gKiBcbiAqICBBIGRhdGEgY2xhc3MgaW4ga290bGluIG1vZFxuICogXG4gKiAgQSBEYXRhIENsYXNzIGlzIGxpa2UgYSByZWd1bGFyIGNsYXNzIGJ1dCB3aXRoXG4gKiAgc29tZSBhZGRpdGlvbmFsIGZ1bmN0aW9uYWxpdGllcy5cbiAqICBXaXRoIEtvdGxpbidzIGRhdGEgY2xhc3NlcywgeW91IGRvbid0IG5lZWQgdG8gXG4gKiAgd3JpdGUvZ2VuZXJhdGUgYWxsIHRoZSBsZW5ndGh5IGJvaWxlcnBsYXRlIFxuICogIGNvZGUgeW91cnNlbGYuXG4gKiAgTm8gbmVlZCBmb3IgR2V0dGVycyBhbmQgU2V0dGVyc1xuICogXG4gKi9cblxuXG5lbnVtIGNsYXNzIEdlbmRlcntcbiAgICBNQUxFLEZFTUFMRVxufVxuZW51bSBjbGFzcyBDb3VudHJ5e1xuICAgIE5pZ2VyaWEsQW1lcmljYSxFbmdsYW5kLFR1cmtleVxufVxuXG5lbnVtIGNsYXNzIEN1cnJlbmN5e1xuICAgIFxuICAgIE5BSVJBLERPTExBUixQT1VORFMsTElSQVxufVxuZGF0YSBjbGFzcyBQZXJzb24oXG4gICAgdmFsIG5hbWU6U3RyaW5nICwgXG4gICAgdmFsIGdlbmRlcjpHZW5kZXIgLCBcbiAgICB2YWwgbW9uZXk6RG91YmxlLCBcbiAgICAvKlxuICAgICAqIGluIGtvdGxpbiB5b3UgY2FuIGdpdmUgYSBkZWZhdWx0IHZhbHVlIHRvIHBhcmFtZXRlcnMgd2hpY2ggbWFrZXMgb3ZlcmxvYWRlZCBmdW5jdGlvbnMgcHJldHR5IGludGVyZXN0aW5nIFxuICAgICAqIFxuICAgICAqIHdoZW4gYSBkZWZhdWx0IHZhbHVlIGlzIHNwZWNpZmllZCBmb3IgYSBwYXJhbWV0ZXIgeW91IGNhbiBvbW1pdCBhc3NpZ25pbmcuXG4gICAgICogXG4gICAgICogKi8gICAgICAgICAgICAgIFxuICAgIHZhbCBjdXJyZW5jeTpDdXJyZW5jeSA9IEN1cnJlbmN5LkRPTExBUixcbiAgICB2YWwgY291bnRyeTpDb3VudHJ5XG4pXG5cbmZ1biBtYWluKGFyZ3M6QXJyYXk8U3RyaW5nPikge1xuICAgIFxuICAgIC8vIGNyZWF0aW5nIGFuIE9iamVjdCBpbiBrb3RsaW46ID4+PiBubyBuZWVkIGZvciB0aGUgbmV3IGtleXdvcmQgYW5kIGtvdGxpbiBpcyB2ZXJ5IGdvb2QgXG4gICAgLy8gaW4gdHlwZSBpbmZlcmVuY2UgaGVuY2UsIHRoZSBuZWVkIHRvIHNwZWNpZnkgZGF0YXR5cGVzIGFyZSBhbG1vc3Qgbm90IG5lY2Vzc2FyeVxuICAgIFxuICAgIFxuICAgdmFyIHBlcnNvbjEgPSBQZXJzb24oXCJNdWJhcmFjayB0YWhpclwiLEdlbmRlci5NQUxFLDkwMDAwMC4wLGNvdW50cnkgPSBDb3VudHJ5Lk5pZ2VyaWEpXG4gICBcbiAgIHZhciBwZXJzb24yID0gUGVyc29uKFwiRnVya2FuIEFza2luXCIsIEdlbmRlci5NQUxFLDcwMDAwMDAuMCxDdXJyZW5jeS5MSVJBLENvdW50cnkuVHVya2V5KVxuICAgXG4gICBcbiAgIC8qXG4gICAgKiBjb3B5aW5nIGFuIGV4aXN0aW5nIG9iamVjdCBhbmQgc3BlY2lmeWluZyB0aGUgY2hhbmdlcyB5b3Ugd2FudCBpbiBpdHMgcGFyYW1ldGVyXG4gICAgKiBcbiAgICAqICovXG4gICB2YXIgcGVyc29uMyA9IHBlcnNvbjEuY29weShuYW1lID0gXCJKb2huIFdpbGxzb25cIiwgY291bnRyeSA9IENvdW50cnkuQW1lcmljYSlcbiAgIHZhciBwZXJzb240ID0gcGVyc29uMS5jb3B5KG5hbWUgPSBcIkFiZHVsbWFqaWQgVXNtYW5cIiwgY3VycmVuY3kgPSBDdXJyZW5jeS5OQUlSQSwgbW9uZXkgPSA4MDAwMDAwLjApXG4gICB2YXIgcGVyc29ubGlzdCA9IGFycmF5T2YocGVyc29uMSxwZXJzb24yLHBlcnNvbjMscGVyc29uNClcbiAgIFxuICAgZm9yICggcGVyc29uIGluIHBlcnNvbmxpc3QgKSB7XG4gICAgICAgdmFyIHN5bWJvbCA9IGlmKHBlcnNvbi5jdXJyZW5jeSA9PSBDdXJyZW5jeS5ET0xMQVIpIFwiJFwiXG4gICAgICAgXHRcdFx0ZWxzZSBpZihwZXJzb24uY3VycmVuY3kgPT0gQ3VycmVuY3kuTkFJUkEpIFwiTlwiXG4gICAgICAgICAgICAgIFx0ZWxzZSBcInRcIlxuICAgICAgIFxuICAgICAgIHByaW50bG4oXCJNeSBuYW1lIGlzICR7cGVyc29uLm5hbWV9LCBJIGFtIGZyb20gJHtwZXJzb24uY291bnRyeX0uIE15IG5ldCB3b3J0aCBpcyAke3N5bWJvbCtwZXJzb24ubW9uZXl9XCIpXG4gICAgICAgcHJpbnRsbigpXG4gICB9XG4gICBcbiAgIFxuICAgXG4gICBcbn0ifQ==
) to explore the code i wrote for you to see how kotlin works!

 

 [Clic here for more examples on kotlin ](https://play.kotlinlang.org/byExample/01_introduction/01_Hello%20world)  

Lets write our Kotlin Code

the `kotlin code` in *android studio* are placed in a directory called `java`, which is located just at the top of the `res` directory in `android studio`  navigate to **java**>**com.example.calculator**>**MainActivity**

**right click** on the file called `MainActivity.kt` and select **new**>**Kotlin File/class** a window will pop up prompting you to input *file name*, name the file "***Calculator***" as spelled, in the list below choose "*class*" and  **hit enter ** to continue 

in `Calculator.kt`, copy and paste the below code snippet into it. Make sure you clear the initial code in the `Calculator.kt` before pasting the below code.

%[https://gist.github.com/17240dc2fe85d02d8e7b058d9a63f269]

In `MainActivity.kt`, copy and paste the below code snippet into it. Make sure you clear the initial code in the `MainActiviy.kt` before pasting the below code.

%[https://gist.github.com/898b3ff27f0d6962010aaa710b384218]

now run the project and test on an emulator.

# Hooray, we are Done!!!
![Alt Text](https://media.giphy.com/media/YTbZzCkRQCEJa/giphy.gif)

if yours isnt working fine, you can download the entire file for this project [here](https://github.com/mubaracktahir/calculator.git)  and open with **Android Studio IDE**



# Useful resources 


-  [Code laps](https://codelabs.developers.google.com/)
-   [Code architecture](https://github.com/android/architecture-samples) 
-  [Code with Mitch Youtube Channel](https://www.youtube.com/channel/UCoNZZLhPuuRteu02rh7bzsw) 
-  [Kotlin Community](https://kotlinlang.org/community/) 
- [Kotlin Docs](https://kotlinlang.org/docs/kotlin-docs.pdf)


### Goodluck in programming for android with Kotlin.

# Cheers!!!





