[android-sdk (1.2.1)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [signOutAsync](./sign-out-async.md)

# signOutAsync

`@JvmStatic @JvmOverloads fun signOutAsync(listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Void`](https://developer.android.com/reference/java/lang/Void.html)`?>? = null): `[`Future`](https://developer.android.com/reference/java/util/concurrent/Future.html)`<`[`Void`](https://developer.android.com/reference/java/lang/Void.html)`?>`

Signs out the current signed-in user asynchronously.

### Parameters

`listener` - optional [FutureListener](../../com.techcentrix.sdk.util/-future-listener/index.md) will be notified when the user has finished signing out

### Exceptions

`IllegalStateException` - when SDK is not initialized

**Return**
[Future](https://developer.android.com/reference/java/util/concurrent/Future.html) representing this asynchronous operation

