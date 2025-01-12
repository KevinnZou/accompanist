# WebView wrapper for Jetpack Compose

[![](https://jitpack.io/v/KevinnZou/compose-webview.svg)](https://jitpack.io/#KevinnZou/compose-webview)

> **Note**
> This library has been migrated to [compose-webview](https://github.com/KevinnZou/compose-webview) to independent from the accompanist library.

According to the [official documentation](https://medium.com/androiddevelopers/an-update-on-jetpack-compose-accompanist-libraries-august-2023-ac4cbbf059f1) updated on August 2023,
Jetpack Compose Accompanist library decided to deprecate the Web library with no replacement.
However, as a contributor to this library, I am still relying on it to provide WebView support in my App. Thus, I decided to fork that library and make future updates on it.
This is a fork of the original library with the latest version 0.33.1-alpha.

For more information, visit the documentation: https://google.github.io/accompanist/web/

## Basic Usage

To implement this wrapper there are two key APIs which are needed: WebView, which provides the layout, and rememberWebViewState(url) which provides some remembered state including the URL to display.

The basic usage is as follows:
```kotlin
val state = rememberWebViewState("https://example.com")

WebView(state)
```
This will display a WebView in your Compose layout that shows the URL provided.

## Download

[![](https://jitpack.io/v/KevinnZou/compose-webview.svg)](https://jitpack.io/#KevinnZou/compose-webview)

```groovy
repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation "com.github.KevinnZou:compose-webview:v0.33.1"
}
```
