[android-sdk (1.0.1)](../../index.md) / [com.techcentrix.sdk.util](../index.md) / [FutureListener](./index.md)

# FutureListener

`interface FutureListener<V>`

A listener that is called back when a [Future](https://developer.android.com/reference/java/util/concurrent/Future.html) is done.

### Functions

| Name | Summary |
|---|---|
| [onDone](on-done.md) | `abstract fun onDone(future: `[`Future`](https://developer.android.com/reference/java/util/concurrent/Future.html)`<`[`V`](index.md#V)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Invoked when the [Future](https://developer.android.com/reference/java/util/concurrent/Future.html) completes, regardless of how (normally, due to an exception, or cancelled). |
