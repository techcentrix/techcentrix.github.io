---
layout: single
title: "Quick-Start Guide"
---

Want to get access? [Contact us](mailto:info@techcentrix.com)!

## TechCentrix SDK Architecture

![](https://github.com/techcentrix/techcentrix.github.io/raw/master/resources/TechCentrix%20SDK%20Architecture.jpg)
[Better quality flow](https://github.com/techcentrix/techcentrix.github.io/raw/master/resources/TechCentrix%20SDK%20Architecture.pdf).

## Dictionary

Item | Description
--- | ---
oneTimeToken | Token that needs to passed to TechCentrix SDK to sign in/up your user. It's a one time token and has a short expiry date.
Server.API.Key | API key is used between your and TechCentrix's server to generate _oneTimeToken_. It can be stored only on your server. Don't store it in a mobile app, because of security reasons.
Mobile.API.Key | It's used in _TechCentrixConfig_, so we can identify you on our side.
TechCentrix Config file | Excel file with Server.API.Key, Mobile.API.Key, Gradle & CocoaPods Access, Firebase Server Key etc. You can find a template [here](https://github.com/techcentrix/techcentrix.github.io/raw/master/resources/TechCentrix%20Config%20File%20-%20TEMPLATE.xlsx).

## Backend Integration
### Integrate your backend with TechCentrix backend

Every time your app starts TechCentrix module, it should ask your backend to authorize with TechCentrix backend. This REST call will sign up/in your user in our backend. In order to make it safe, this REST call needs to be signed by _Server.API.Key_. This key **must be** stored only on your backend. (Don't store this key in your mobile application)

For REST call preview, you can download Postman collection from [here](https://github.com/techcentrix/techcentrix.github.io/raw/master/resources/TechCentrix%20-%20External%20Auth.postman_collection.json).

### Auth External

```
POST https://api.techcentrix.com/user/api/auth/external
```

Headers

```
Authorization: Bearer Server.API.Key
Content-Type: application/json
```

Request Body

```
{
  "id": "user1-external", // unique id for that user. Could be same as in your database, or any other string
  "email": "user1@techcentrix.com", // email address of user
  "firstName": "User1Name" // first name of user signed in your application
}
```
* Success Response:
    * **Code:** 200
    * **Content:** `eyJhbGciOiJIUzUxMiJ9.eyJqdGkiOiJjY2Y0MWNkYy1kNWY1LTRlMT...`

* Error Response:
    * **Code:** 401 Unauthorised
    * **Content:** `{ message: "Invalid access token", errorCode: 4 }`

## Mobile integration
TechCentrix SDK supports 2 mobile platforms: Android & iOS.

### Android
#### Requirements
* Kotlin & Java
* Android 5.0 (API 21) or newer
* project based on AndroidX libraries (old Android Support libraries are not supported)

#### API Documentation
We have more in-depth [API Documentation](/resources/android-sdk).

#### Step by step instructions
Follow this [instruction to integrate](https://github.com/techcentrix/techcentrix-sdk-android/) your Android application.

### iOS
#### Requirements
* Swift 5.0+
* iOS 11+

#### API Documentation
We have more in-depth [API Documentation](/resources/ios-sdk).

#### Step by step instructions
Follow this [instruction to integrate](https://github.com/techcentrix/techcentrix-sdk-ios) your iOS application.
