[android-sdk (1.2.3)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [handlePushMessage](./handle-push-message.md)

# handlePushMessage

`@JvmStatic fun handlePushMessage(message: RemoteMessage): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Handles `RemoteMessage` received in `FirebaseMessagingService`.

Call this method only if [isTechCentrixPushMessage](is-tech-centrix-push-message.md) returned `true` for passed in `message` object.

### Exceptions

`IllegalArgumentException` - when `message` is not intended for TechCentrix SDK

`IllegalStateException` - when SDK is not initialized