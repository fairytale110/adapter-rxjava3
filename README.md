# adapter-rxjava3
RxJava 3 adapter for Retrofit 2 based on `rxjava:3.0.1` and `retrofit:2.7.2`

## How
to get this lib into your build:
Add it in your root build.gradle at the end of repositories:
```Gradle
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
 ```
 
 Step 2. Add the dependency
```Gradle
	dependencies {
		...
	        implementation 'com.github.fairytale110:adapter-rxjava3:2.7.2'
	}
```

## Usage
``` Kotlin
import tech.nicesky.retrofit2_adapter_rxjava3.RxJava3CallAdapterFactory

var retrofit = Retrofit.Builder()
            .addCallAdapterFactory(RxJava3CallAdapterFactory.create())
            ...
            .build()

```
