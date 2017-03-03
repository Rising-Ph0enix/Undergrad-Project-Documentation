# Procedure to export APK files (live document)

**Step 1:**

Go to the gradle file of your app.

Edit it to allow export of unsigned apk

Mine (2017) looks like this

android {
    compileSdkVersion 25
    buildToolsVersion "25.0.2"
    defaultConfig {
        applicationId "com.example.dell.mygps"
        minSdkVersion 15
        targetSdkVersion 25
        versionCode 1
        versionName "1.0"
        testInstrumentationRunner "android.support.test.runner.AndroidJUnitRunner"
    }
    buildTypes {
        release {
            minifyEnabled true
            proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
        }

        releaseUnsigned.initWith(buildTypes.release)
        releaseUnsigned {
            signingConfig null
        }
    }
}

**Step 2:**

In the menu bar above

Go to Build -> Build APK

Your APK file will be in Android Project directory / your app / build / outputs / YOUR APK FILE !

(You can view by File -> Open)

For me this is my path:

C:\Users\dell\AndroidStudioProjects\MyGPS\app\build\outputs\apk\app-debug.apk

**Step 3:**

You can now send your APK file to your phone via:

i. email: (if you have internet connection on your phone)

Send a mail to yourself with attachement of the apk file. & Then in your phone open the mail -> open the link -> download. Install. :D Party!

ii. usb (enable file sharing)
Copy straigtaway -> Open -> download
