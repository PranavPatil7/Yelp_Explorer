# YelpExplorer


## Project Description

YelpExplorer is a multiplatform project that shows a list of businesses, their details and latest reviews using
[Yelp](https://www.yelp.com/)'s API.

I originally created this project to learn about GraphQL but since Yelp is also serving its data with a REST API,
I thought it would be a great opportunity to showcase the power of Clean Architecture when it comes to being able
to swap one data layer for another without having to modify the domain and presentation layers.

I then thought it would be a great experience to port this Android project to Flutter and ReactNative to learn more
about all the different technologies that exist to build multiplatform applications.

This project is available in:<br/>
[Compose/Kotlin](https://github.com/matthieucoisne/YelpExplorer)<br/>
[Flutter/Dart](https://github.com/matthieucoisne/YelpExplorer-Flutter)<br/>
[ReactNative/TypeScript](https://github.com/matthieucoisne/YelpExplorer-ReactNative)<br/>

### Screenshots

| Business List | Business Details |
|:-------------:|:----------------:|
|![YelpExplorer - Business List](https://github.com/matthieucoisne/YelpExplorer/blob/main/media/YelpExplorer-KMP-BusinessList.png) | ![YelpExplorer - Business Details](https://github.com/matthieucoisne/YelpExplorer/blob/main/media/YelpExplorer-KMP-BusinessDetails.png)|

## Project Characteristics

* 100% [Kotlin](https://kotlinlang.org/)
* Modern architecture (Clean Architecture, Model-View-ViewModel, Dependency Injection)
* Declarative UI framework using [Jetpack Compose](https://developer.android.com/jetpack/compose)
* Testing
* Material design
* Continuous Integration with GitHub [Actions](https://github.com/matthieucoisne/YelpExplorer/actions)
* Project management with GitHub [Project Board](https://github.com/matthieucoisne/YelpExplorer/projects/1)

## Tech Stack

* Tech Stack
    * [Kotlin](https://kotlinlang.org/)
    * [Coroutines](https://kotlinlang.org/docs/coroutines-overview.html)
    * [Flow](https://kotlinlang.org/docs/flow.html)
    * [Koin](https://github.com/InsertKoinIO/koin)
    * [Retrofit](https://square.github.io/retrofit)
    * [ApolloGraphQL](https://github.com/apollographql/apollo-android)
    * [Jetpack](https://developer.android.com/jetpack)
        * [Navigation](https://developer.android.com/guide/navigation)
        * [ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel)
        * [Compose](https://developer.android.com/jetpack/compose)
    * [Coil](https://github.com/coil-kt/coil)
    * [and more...](https://github.com/matthieucoisne/YelpExplorer/blob/main/app/build.gradle.kts)
* Architecture
    * Clean Architecture
    * MVVM
    * [Modern Android Architecture](https://developer.android.com/topic/architecture#recommended-app-arch)

## Development Setup

### Yelp API Key

If you want to run this project on an device or an emulator, you need to obtain your own API key from Yelp and
provide it to the app.

1. Request your API key: [https://www.yelp.com/developers/documentation/v3/authentication](https://www.yelp.com/developers/documentation/v3/authentication)<br/>
2. Update [Const.kt](https://github.com/matthieucoisne/YelpExplorer/blob/main/app/src/main/java/com/yelpexplorer/core/utils/Const.kt) with your key

### REST vs GraphQL

This project allows you to either use the GraphQL API or the REST API to retrieve data.<br/>
To switch between one or the other, you can change the value of `DATASOURCE` in [Const.kt](https://github.com/matthieucoisne/YelpExplorer/blob/main/app/src/main/java/com/yelpexplorer/core/utils/Const.kt).


