# PackagesMaven

Android Base SDK Maven packages repository.

Used by AndroidBaseSDKProject to host shared Android components.

## 使用方式

```groOvy
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.PREFER_PROJECT)
    repositories {
        maven {
            name = "GitHubPackages"
            url = uri("https://maven.pkg.github.com/lvtong199881/PackagesMaven")
            credentials {
                username = "lvtong199881"
                password = providers.environmentVariable("GITHUB_TOKEN")
            }
        }
    }
}

dependencies {
    implementation("com.mohanlv:base:1.2.28")
}
```
