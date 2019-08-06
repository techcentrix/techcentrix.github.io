[android-sdk (1.1.0)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [isSignedIn](./is-signed-in.md)

# isSignedIn

`@JvmStatic fun isSignedIn(): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Returns `true` if a user is signed in.

If `true` is returned, you can call [com.techcentrix.sdk.ui.TechCentrixActivity.start](../../com.techcentrix.sdk.ui/-tech-centrix-activity/start.md) method to show SDK UI.
If `false` is returned, you must sign in the user using one of the [signIn](sign-in.md) or [signInAsync](sign-in-async.md) methods.

### Exceptions

`IllegalStateException` - when SDK is not initialized

**Return**
`true` if the user is signed in; `false` otherwise

