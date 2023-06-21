---
title: "What is Google Location Services API"
description: "...."
pubDate: "2016-05-15"
categories: 
  - "archived"
---

[![](/images/gps-location.png)](https://3.bp.blogspot.com/-rkbpEpnOLPA/VzgP5Pnc19I/AAAAAAAAC7E/xDIgUIN4zUs3h7t0JqI_A-iErjYr7C5AQCLcB/s1600/gps-location.png)

  

Knowing your user’s location is useful information in many applications we develop and use today. There are a lot of popular location-based applications out there that are making our lives easier, as well as changing the way that we use these services. An example is the wildly popular application Foursquare, where users who frequent to an establishment and “check in” often win discounts. Uber, which helps you get a ride from your mobile phone at a lower rate than a normal taxi. The list is large and still growing.

  

Google Location Services API, also known as FusedLocationProviderApi, is Google’s recommended way of getting a user’s location. It provides the best accuracy based on our needs. Some of the advantages of using this API over the previous one are:

  

- **Simplicity:** Unlike the previous API, you no longer have to deal with multiple providers. Instead, you specify high-level needs, such as “high accuracy” or “low power”, and it will take a suitable approach.
- **Availability:** Gives your app immediate access to the best, most recent known location. Usually this information is readily available, you just have to ask for it.
- **Power-efficiency:** Minimizes your application’s usage of power.
- **Versatility:** Meets a wide range of needs, from foreground uses - needing highly accurate location data, to background uses - requiring only periodic location updates with negligible power impact.

  

  

Read the [Android Developer’s Guide to the Google Location Services API](https://www.toptal.com/android/android-developers-guide-to-google-location-services-api) to learn how to use Google Location Services API in your app.
