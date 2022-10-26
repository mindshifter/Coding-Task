# Android Coding Task

#### Overview

**Coding Task is a simple registration application with validations and data store persistence.**

# Used SDK

| SDK       | URL                                                                    | USAGE                                                                                                                                                                                                                                    |
|-----------|------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Koin      | <https://github.com/InsertKoinIO/koin/blob/main/README.md>             | Used for dependency injection                                                                                                                                                                                                            |
| DataStore | <https://developer.android.com/topic/libraries/architecture/datastore> | Jetpack DataStore is a data storage solution that allows you to store key-value pairs or typed objects with protocol buffers. DataStore uses Kotlin coroutines and Flow to store data asynchronously, consistently, and transactionally. |

# Development

Coding Task was build with **MVVM** architecture and **Material3 UI**
**RegistrationViewModel.kt** is handling all the data changes and data validations from **UI**
**ConfirmationViewModel.kt** is observing data changes from **DataStore**
If validation passes data is stored in **DataStore** using a custom Json Serializer from **kotlinx-serialization-json**

Also I included validators UnitTests and UI tests
