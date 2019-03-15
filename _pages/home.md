---
defaults:
  # _pages
  - scope:
      path: ""
      type: pages
    values:
      layout: single
      author_profile: true

---
## Welcome

Want to get access, [contact us](mailto:info@techcentrix.com)!

* [About TechCentrix](#about-techcentrix)
* [Flow](#flow)
* [How to integrate with a TechCentrix system](#how-to-integrate-with-a-techcentrix-system)
  * [Dictionary](#dictionary)
  * [Step 1 - Integrate your backend with TechCentrix backend](#step-1---integrate-your-backend-with-techcentrix-backend)
  * [Step 2 - 5 - Integrate your mobile application with TechCentrix SDK](#step-2---5---integrate-your-mobile-application-with-techcentrix-sdk)
    * [Requirements for mobile apps](#requirements-for-mobile-apps)

## About TechCentrix

## Flow

You can find a simplified flow [here](https://github.com/techcentrix/techcentrix.github.io/blob/master/TechCentrix%20SDK%20flow.pdf).

## How to integrate with a TechCentrix system

### Dictionary

Item | Description
--- | ---
oneTimeToken | Token that needs to passed to TechCentrix SDK to sign in/up your user. It's a one time token and with a short expiry date.
Server.API.Key | API key is used between your and TechCentrix's server to generate _oneTimeToken_. It can be stored only on your server. Don't store it in a mobile app, because of security reasons.
TechCentrixAppId | This Id used in _TechCentrixConfig_, so we can identify you on our side.

### Step 1 - Integrate your backend with TechCentrix backend

Every time your app starts TechCentrix module, it should ask your backend to authorize with TechCentrix backend. This REST call will sign up/in your user in our backend. In order to make it safe, this REST call needs to be signed by _Server.API.Key_. This key **must be** stored only on your backend. (Don't store this key in your mobile application)

For REST call preview, you can download Postman collection from [here](https://github.com/techcentrix/techcentrix.github.io/blob/master/external.postman_collection.json).

### Auth External

```
POST https://api.datalyticz.com/user/api/auth/external
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
    * **Content:** `eyJhbGciOiJIUzUxMiJ9.eyJqdGkiOiJjY2Y0MWNkYy1kNWY1LTRlMTEtYWNlOC0zMjY5NzIyMzk3ZmUiLCJzdWIiOiJsdWtlMSIsImF1dGgiOlsiUk9MRV9VU0VSIl0sInR5cGUiOiJhY2Nlc3MiLCJleHAiOjE1NTE4ODk4MTh9.MHAlXtH-6JgJjBda9c1OgfXR-iHMHqAfVhh2KfEFqHHRZqqf-nzAJ8DqFSv37trerjkktggcMprkIn0YsZNiLQ`

* Error Response:
    * **Code:** 401 Unauthorised
    * **Content:** `{ message: "Invalid access token", errorCode: 4 }`

## Step 2 - 5 - Integrate your mobile application with TechCentrix SDK

### Android
#### Requirements
* Kotlin or Java
* android-support //TODO

[Android docs GFM](../resources/android-sdk (1.0.0))

Follow these instruction to integrate your iOS application. //TODO: Add final URL

### iOS
#### Requirements
* iOS 11.0+
* Swift 4.0+

[Follow these instruction to integrate your iOS application.](https://github.com/techcentrix/techcentrix-sdk-ios/blob/master/README.md#step-2---integrate-your-mobile-application-with-techcentrix-sdk)
