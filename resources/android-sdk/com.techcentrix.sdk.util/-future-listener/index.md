[android-sdk (1.4.3)](../../index.md) / [com.techcentrix.sdk.util](../index.md) / [FutureListener](./index.md)

# FutureListener

`interface FutureListener<V>`

A listener that is called back when a [Future](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Future.html) is done.

### Functions

| Name | Summary |
|---|---|
| [onDone](on-done.md) | Invoked when the [Future](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Future.html) completes, regardless of how (normally, due to an exception, or cancelled).`abstract fun onDone(future: `[`Future`](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Future.html)`<V>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
