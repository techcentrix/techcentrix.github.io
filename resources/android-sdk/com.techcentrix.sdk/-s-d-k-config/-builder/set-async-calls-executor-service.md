[android-sdk (1.1.0)](../../../index.md) / [com.techcentrix.sdk](../../index.md) / [SDKConfig](../index.md) / [Builder](index.md) / [setAsyncCallsExecutorService](./set-async-calls-executor-service.md)

# setAsyncCallsExecutorService

`fun setAsyncCallsExecutorService(asyncCallsExecutorService: `[`ExecutorService`](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html)`): `[`SDKConfig.Builder`](index.md)

Sets optional [ExecutorService](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html) used to execute async calls of the [TechCentrixSDK](../../-tech-centrix-s-d-k/index.md)
(for example [TechCentrixSDK.signInAsync](../../-tech-centrix-s-d-k/sign-in-async.md) or [TechCentrixSDK.signOutAsync](../../-tech-centrix-s-d-k/sign-out-async.md)).

[TechCentrixSDK](../../-tech-centrix-s-d-k/index.md) will create its own [ExecutorService](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html) if you don't provide one.

**Note:** This [ExecutorService](https://developer.android.com/reference/java/util/concurrent/ExecutorService.html) is not used with `suspend` versions of [TechCentrixSDK](../../-tech-centrix-s-d-k/index.md) methods like
[TechCentrixSDK.signIn](../../-tech-centrix-s-d-k/sign-in.md) or [TechCentrixSDK.signOut](../../-tech-centrix-s-d-k/sign-out.md)

