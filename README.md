# iOS Development Challenge

A fun 6 hour challenge for candidates interviewing for a junior to mid-level iOS Developer position.

## Instructions

Using the latest version of Xcode and the Swift programming language, create an iOS application compatible with iOS 11 and later.

The minimum requirements are the following:

1. When the app is launched, a home screen must be presented. The home must have a Tab Bar with 2 tabs.

2. The first tab must present a Google Map (please name it MapViewController), showing the user's current location and a functional My Location button that centers the map on the user's location.

3. The second tab must present a list (please name it ListViewController) of the top 25 places that are located in a 100 meter radius around the user's current location. Make a request to the Google Places API with the user's latitude and longitude coordinates to obtain the places in JSON format and process the received JSON response to populate the list. The list must show an image, use async or lazy loading to load images and places as the list scrolls down. Each row must have the place's name as a title and its street address as as subtitle. For the list, you are expected to use an UITableView, an adapter and the corresponding UITableViewCell row items, you are expected to use modern memory efficient techniques for loading and displaying the data on the cells.

4. When a place on the list is tapped by the app's user, an UIViewController of your choice with the place's details must be presented with more information about the place that was tapped (please name it PlaceViewController). Again, make a request to the Google Places API to request the details of the tapped place, receive the response in JSON and show them on the list. If the back button is tapped while on the place's detail, the PlaceViewController must go away and the app must go back to the list.


Extra points will be awarded if you use:
* You use URLSession and JSONSerialization to make requests and do not use any 3rd party libraries for Neworking and JSON parsing.
* You implement a "refresh map" mechanism to refresh the map with the places in range based on the user's location.
* You implement a "pull to refresh" control on the list that refreshes the list based on the user's location.
* You come up with a nice and modern UI/UX, it is recommended you follow Apple's UI Guidelines (Cupertino look and feel).
* You use Test Driven Development and implement test for your code.

## Deadline

You'll have 6 hours to complete this challenge. The clock starts ticking from the moment you receive access to this repository. If you finish it sooner... hey!, extra points!

**Please be sure to only work in the branch named with your git username. Do not push any changes directly to the master branch.**


## Additional Information

Please add any additional information on how to run the project or any additional comments to the file called README_CANDIDATE.md.


## Third Party APIs Documentation

* Google Maps for iOS: https://developers.google.com/maps/documentation/ios-sdk/intro

* Google Places Cocoapod: https://cocoapods.org/pods/GooglePlaces

* Google Places API Web Service:
  * Place Search: https://developers.google.com/places/web-service/search
  * Place Details: https://developers.google.com/places/web-service/details



## Tools

* Xcode: https://developer.apple.com/xcode/

## Swift Style Guide

* https://google.github.io/swift/#apples-api-style-guidelines
