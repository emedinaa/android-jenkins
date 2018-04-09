[Coming soon]# android-jenkins
This is a demo about  how integrate Jenkins with Android

## Environment

- macOS Sierra version 10.12.5
- Jenkins
- Git
- Gradle

### Step 1 - Gradle

SDKMAN

```
sdk install gradle
```

Homebrew

```
sdk install gradle
```

### Step 2 - Jenkins

- Install Jenkins using Homebrew

```
brew install jenkins-lts
```

- Open Jenkins

```
http://localhost:8080
```

- Unlock Jenkins

```
cat /Users/xxxxx/.jenkins/secrets/initialAdminPassword
```

### Step 3 - Configuration

- Plugins

  Manage Jenkins / Manage Plugins / Available
  
  ```
    Android Emulator Plugin
    
    AndroidLint Plugin
    
    Bitbucket Plugin
    
    Git Plugin
    
    Groovy
    
    Gradle Plugin
    
  ```
  
- Environment variables

  Manage Jenkins / Configure System / Global properties /
  
  Check : Environment variables
  
  ```
  Name : ANDROID_HOME
  
  Value : /Users/xxxx/Library/Android/sdk
  ```

## Tips

- sdk Manager

```
sdkmanager --update && yes | sdkmanager --licenses
```

## References

- Gradle https://gradle.org/install/

- Jenkins https://jenkins.io/doc/book/installing/


