[android-sdk (1.2.2)](../../../index.md) / [com.techcentrix.sdk](../../index.md) / [SDKConfig](../index.md) / [Builder](index.md) / [&lt;init&gt;](./-init-.md)

# &lt;init&gt;

`Builder(context: `[`Context`](https://developer.android.com/reference/android/content/Context.html)`, mobileApiKey: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)`

Start building a new [SDKConfig](../index.md) instance.

### Parameters

`context` - Any Android [Context](https://developer.android.com/reference/android/content/Context.html) object. It is safe to pass in an Activity context as the [SDKConfig](../index.md)
instance keeps a reference to the Application context internally to avoid memory leaks.

`mobileApiKey` - API key received from TechCentrix which uniquely identifies your application within our backend

### Exceptions

`IllegalArgumentException` - when `mobileApiKey` is blank

**Constructor**
Start building a new [SDKConfig](../index.md) instance.

