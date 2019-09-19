[android-sdk (1.2.0)](../../../index.md) / [com.techcentrix.sdk](../../index.md) / [SDKConfig](../index.md) / [Builder](./index.md)

# Builder

`class Builder`

Fluent API for creating [SDKConfig](../index.md) instances.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Builder(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`, mobileApiKey: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)`<br>Start building a new [SDKConfig](../index.md) instance. |

### Functions

| Name | Summary |
|---|---|
| [build](build.md) | `fun build(): `[`SDKConfig`](../index.md)<br>Create the [SDKConfig](../index.md) instance. |
| [setAsyncCallsExecutorService](set-async-calls-executor-service.md) | `fun setAsyncCallsExecutorService(asyncCallsExecutorService: `[`ExecutorService`](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html)`): `[`SDKConfig.Builder`](./index.md)<br>Sets optional [ExecutorService](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html) used to execute async calls of the [TechCentrixSDK](../../-tech-centrix-s-d-k/index.md) (for example [TechCentrixSDK.signInAsync](../../-tech-centrix-s-d-k/sign-in-async.md) or [TechCentrixSDK.signOutAsync](../../-tech-centrix-s-d-k/sign-out-async.md)). |
