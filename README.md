**Android browser app based on Custom Tabs protocol.**

<img src="android-app/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png" align="left"
width="200"
    hspace="10" vspace="10">

Lynket utilizes Chrome Custom Tab API to create a customized browsing experience while adding innovative features like background loading with floating bubbles, article mode and multitasking using Android's recent menu.

Lynket is available for free on the Google Play Store.


<a href="https://play.google.com/store/apps/details?id=arun.com.chromer">
    <img alt="Get it on Google Play"
        height="80"
        src="https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png" />
</a>

This is simple Splash Screen App | The Splash screen is used for basically two things. Number one usage of splash screen is to welcome our app users to into the app with a nice UI and the second critical usage is to make sure your app loads all the basic information while the Splash screen is being displayed to the user.<a href="https://github.com/SabithPkcMnr/SplashScreen/blob/master/app/src/main/java/com/sabithpkcmnr/splashscreen/ActivitySplash.java">here</a>
<img src="/screenshots/sabith_pkc_mnr_github_repo_splash_screen_intro.webp">
<br>

## Implementation - Now the timer is based on postDelayed() public method. This method will help us to queue a process to a certain period of time that we set for the method and app will perform that task after that time period.

First we set the time for the timer using a very simple `int SPLASH_TIME` variable
```groovy
int SPLASH_TIME = 3000; //This is 3 seconds
```

```groovy
new Handler().postDelayed(new Runnable() {
            @Override
            public void run() {
                //Do any action here. Now we are moving to next page
                Intent mySuperIntent = new Intent(ActivitySplash.this, ActivityHome.class);
                startActivity(mySuperIntent);

                //This 'finish()' is for exiting the app when back button pressed from Home page which is ActivityHome
                finish();

            }
        }, SPLASH_TIME);
```

<br>You canb also watch the complete tutorial video from my very on YouTube channel here:<br>
[![Click to watch tutorial video](https://img.youtube.com/vi/jXtof6OUtcE/0.jpg)](https://www.youtube.com/watch?v=jXtof6OUtcE)
<br><br>
<h4>Hey, while you're here why don't you think of following me for awesome projects like this, ah? <a href="https://github.com/SabithPkcMnr">Follow Me on my Profile!</a></h4>

<br>
Now grab a cup of hot or cold coffee☕ and let's get started. Feel free to give a star, fork and play around the ads.

This app make it easy for you to implement Facebook ads very easily into your Android App and it is very similar to how we used to  implement the [Google AdMob Ads](https://developers.google.com/admob/android/quick-start/ "Yoo my boi click to open this page").
