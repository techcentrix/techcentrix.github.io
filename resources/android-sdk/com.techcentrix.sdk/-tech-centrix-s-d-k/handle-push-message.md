[android-sdk (1.4.3)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [handlePushMessage](./handle-push-message.md)

# handlePushMessage

`@JvmStatic fun handlePushMessage(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`, message: RemoteMessage): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Handles `RemoteMessage` received in `FirebaseMessagingService`.

Call this method only if [isTechCentrixPushMessage](is-tech-centrix-push-message.md) returned `true` for passed in `message` object.

### Parameters

`context` - Any Android [Context](https://developer.android.com/reference/android/content/Context.html) object to initialize SDK if needed