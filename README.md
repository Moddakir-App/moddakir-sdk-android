﻿# Moddakir-AndroidSDK
Android Library connects you Directly with teacher to learn the Holy Qur’an  📖

##  Getting Started
These instructions will help you setup, integrate and run your project integrated with our SDK.


##  Prerequisits
Android SDK version above 31.

##  Integration Steps
1. Add the JitPack repository to your settings.gradle:
```java
dependencyResolutionManagement {
   repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
   repositories {
       google()
       mavenCentral()
       maven { url 'https://jitpack.io' }
   }
}
```



2. Add the dependency
```java
 dependencies {
   implementation 'com.github.Moddakir-App:moddakir-sdk-android:LatestReleaseNumber'
 }
```



##  Quick Start

Call makeCall method :
```java
makeCall(String AppID,String AppKey, Context Context ,String Gender,String Name,String Phone,String Email,String Language)
```

### to initialize a new call with a random teacher and it will be responsible for:

Validate the user’s name,user's phone number,user's email ,user's gender and language.

Present the waiting screen to the user while trying to connect with a teacher.

Present the in-call screen once the teacher accepts the call.

Present the rating screen after the call ends if it continues more than 30 seconds.

Present the rating done pop-up after rating the teacher and the call.


### this funtion take:

AppID : Contact Moddakir Support to get this value

AppKey: Contact Moddakir Support to get this value

Context: Context of activity that will start the call

Gender: The user’s gender "male/female"

Name: The user's Name

Phone: The user Phone include the country code

Email: The user Email

Language: application language "ar/en/fr/in/ur"
