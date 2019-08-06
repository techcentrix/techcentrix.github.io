[android-sdk (1.1.0)](../../index.md) / [com.techcentrix.sdk](../index.md) / [TechCentrixSDK](index.md) / [signIn](./sign-in.md)

# signIn

`suspend fun signIn(oneTimeToken: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Signs in/up a user with the given `oneTimeToken`.

### Parameters

`oneTimeToken` - authentication token with a short expiry date

### Exceptions

`IllegalStateException` - when SDK is not initialized

**Return**
`true` if authentication was successful; `false` otherwise

