Appus Splash
=====================

Appus Splash is a tool which allows to easily create nice Splash animation and attach it to your activity.

* [Demo](#demo)
* [Getting Started](#getting-started)
* [Customization](#customization)
* [Info](#info)

# Demo
![](https://github.com/roman-voronoy/Appus/blob/master/Splash/image/splash_demo.gif)

# Getting Started

##Usage example:


    public class MainActivity extends Activity {

        @Override
        protected void onCreate(Bundle savedInstanceState) {
            super.onCreate(savedInstanceState);

            .... your onCreate code here ....

            Splash.Builder splash = new Splash.Builder(this, getActionBar());
            splash.perform();
        }
    }


##Setup:

1. Add "splash" module to your project
2. Add to settings.gradle file:

        include ':splash'

3. Add to build.gradle main app module file:

        compile project(':splash')
4. Done!


# Customization

Set custom color of background:


        splash.setBackgroundColor(getResources().getColor(R.color.blue));

Set custom image for background:


        splash.setBackgroundImage(getResources().getDrawable(R.drawable.default_splash_image));

Set custom image for splash:


        splash.setSplashImage(getResources().getDrawable(R.drawable.default_splash_image));

Set custom color of splash image:


        splash.setSplashImageColor(getResources().getColor(R.color.blue));


# Info

Developed By
------------

* Igor Malytsky, Appus Studio

License
--------

    Copyright 2015 Appus Studio.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.