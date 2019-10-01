[android-sdk (1.2.1)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](./index.md)

# TechCentrixSDK

`object TechCentrixSDK`

TechCentrix SDK lets you manage and share LED Displays.

### Functions

| Name | Summary |
|---|---|
| [handlePushMessage](handle-push-message.md) | `fun handlePushMessage(message: RemoteMessage): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Handles `RemoteMessage` received in `FirebaseMessagingService`. |
| [init](init.md) | `fun init(config: `[`SDKConfig`](../-s-d-k-config/index.md)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Initializes TechCentrix SDK. **Note:** It can be called only once and must be called before any other actions. |
| [isInitialized](is-initialized.md) | `fun isInitialized(): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Returns `true` if SDK is initialized. |
| [isSignedIn](is-signed-in.md) | `fun isSignedIn(): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Returns `true` if a user is signed in. |
| [isTechCentrixPushMessage](is-tech-centrix-push-message.md) | `fun isTechCentrixPushMessage(message: RemoteMessage): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Returns `true` if `RemoteMessage` received in `FirebaseMessagingService` should be handled by TechCentrix SDK. |
| [signIn](sign-in.md) | `suspend fun signIn(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Signs in/up a user with the given `oneTimeToken`. |
| [signInAsync](sign-in-async.md) | `fun signInAsync(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>? = null): `[`Future`](https://developer.android.com/reference/java/util/concurrent/Future.html)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>`<br>Signs in/up a user asynchronously with the given `oneTimeToken`. |
| [signOut](sign-out.md) | `suspend fun signOut(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Signs out the current signed-in user. |
| [signOutAsync](sign-out-async.md) | `fun signOutAsync(listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Void`](https://developer.android.com/reference/java/lang/Void.html)`?>? = null): `[`Future`](https://developer.android.com/reference/java/util/concurrent/Future.html)`<`[`Void`](https://developer.android.com/reference/java/lang/Void.html)`?>`<br>Signs out the current signed-in user asynchronously. |
