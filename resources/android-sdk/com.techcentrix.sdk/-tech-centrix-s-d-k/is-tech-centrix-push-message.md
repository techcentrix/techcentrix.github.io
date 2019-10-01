[android-sdk (1.2.1)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [isTechCentrixPushMessage](./is-tech-centrix-push-message.md)

# isTechCentrixPushMessage

`@JvmStatic fun isTechCentrixPushMessage(message: RemoteMessage): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Returns `true` if `RemoteMessage` received in `FirebaseMessagingService` should be handled by TechCentrix SDK.

If `true` is returned, you should call [handlePushMessage](handle-push-message.md) method with passed in `message` object.

### Exceptions

`IllegalStateException` - when SDK is not initialized

**Return**
`true` if `message` should be handled by TechCentrix SDK; `false` otherwise

