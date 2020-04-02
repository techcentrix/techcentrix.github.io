[android-sdk (1.4.2)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](./index.md)

# TechCentrixSDK

`object TechCentrixSDK`

TechCentrix SDK lets you manage and share LED Displays.

### Functions

| Name | Summary |
|---|---|
| [handlePushMessage](handle-push-message.md) | Handles `RemoteMessage` received in `FirebaseMessagingService`.`fun handlePushMessage(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`, message: RemoteMessage): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [isSignedIn](is-signed-in.md) | Returns `true` if a user is signed in.`fun isSignedIn(): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isTechCentrixPushMessage](is-tech-centrix-push-message.md) | Returns `true` if `RemoteMessage` received in `FirebaseMessagingService` should be handled by TechCentrix SDK.`fun isTechCentrixPushMessage(message: RemoteMessage): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [setLoggingEnabled](set-logging-enabled.md) | Toggle whether logging is enabled.`fun setLoggingEnabled(enabled: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [signIn](sign-in.md) | Signs in/up a user with the given `oneTimeToken`.`suspend fun signIn(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [signInAsync](sign-in-async.md) | Signs in/up a user asynchronously with the given `oneTimeToken`.`fun signInAsync(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>? = null): `[`Future`](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Future.html)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>` |
| [signOut](sign-out.md) | Signs out the current signed-in user.`suspend fun signOut(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [signOutAsync](sign-out-async.md) | Signs out the current signed-in user asynchronously.`fun signOutAsync(listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`?>? = null): `[`Future`](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Future.html)`<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`?>` |
