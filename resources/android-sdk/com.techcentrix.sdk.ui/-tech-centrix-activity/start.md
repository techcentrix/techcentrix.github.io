[android-sdk (1.3.1)](../../index.md) / [com.techcentrix.sdk.ui](../index.md) / [TechCentrixActivity](index.md) / [start](./start.md)

# start

`@JvmStatic fun start(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Starts SDK UI. Call this method only if a user is signed in.

If the user is not signed in, [TechCentrixActivity](index.md) will finish itself immediately.

### Parameters

`context` - Any Activity [Context](https://developer.android.com/reference/android/content/Context.html) object

### Exceptions

`IllegalStateException` - when SDK is not initialized