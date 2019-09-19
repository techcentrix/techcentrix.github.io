[android-sdk (1.2.0)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [signInAsync](./sign-in-async.md)

# signInAsync

`@JvmStatic @JvmOverloads fun signInAsync(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, listener: `[`FutureListener`](../../com.techcentrix.sdk.util/-future-listener/index.md)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>? = null): `[`Future`](https://developer.android.com/reference/java/util/concurrent/Future.html)`<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>`

Signs in/up a user asynchronously with the given `oneTimeToken`.

### Parameters

`oneTimeToken` - authentication token with a short expiry date

`listener` - optional [FutureListener](../../com.techcentrix.sdk.util/-future-listener/index.md) will be notified when the user has finished signing in

### Exceptions

`IllegalStateException` - when SDK is not initialized

**Return**
[Future](https://developer.android.com/reference/java/util/concurrent/Future.html) representing this asynchronous operation (`true` if authentication was successful; `false` otherwise)

