# Meal Diary

Meal Diary is an app meant to help users keep track of their diet in order to assist them in eating healthier. It seeks to do so by simplifying the process of recording one's meals, encouraging awareness over counting calories by making creating a new entry as easy as simply taking a picture of your meal.

While this was not technically my first foray into app development for I had created a simple web app a number of years earlier, it was my first time writing an app specifically for android in Kotlin. The reason I had chosen to create the app was because I felt that the introduction of Kotlin and Android Studio made the app development process more accessible than before, and I thought that it was my turn to give it a shot.

When I first started learning Kotlin, I picked up most of the basic skills from the tutorial by Google by building and experimenting with their introductory apps, incorporating the knowledge I gained from them into my own app. However, as my app grew more complex with more interactions and features, I had to cast my net wider and scour the internet or possible solutions to the difficulties I began to encounter. After much trial and error, I had finally managed to include the features I had desired to include.

The app makes use of intents to use the in-built camera app to take a photo, then uses the Google Places API to provide a location tag to the image, allowing location and time data to be stored. Each entry is stored locally on the user's device, and collectively they are used to populate the RecyclerView used to display the entries. The result can be seen in the screenshot below.

<img src="images/Meal-Diary-SS.jpeg"
	width="250"/>

If you are interested in trying this version of the app, please download the apk [here](https://github.com/Yi-Jiahe/Yi-Jiahe.github.io/releases/tag/MealDiaryv0.1.0). Please note that this version is not meant for commercial use and some features might be unavailable should the number of API requests be exceeded.

During a recent NTU module, CY0006 Enterprise, Innovation and Leadership, my group and I are looking into the feasibility of such an app based on its desirability to actual users. In the process we gathered positive feedback and learnt more about the revenue and dependency costs of running an app. We are also looking into utilising the Google Vision API to provide more details on the pictures.

The project also brought back my interest in the project, and I decided to try out another mobile development tool I had recently discovered, Flutter. While I was originally drawn in by its ability to allow developers to develop apps for both Apple and Android from the same codebase, I found it much easier to develop widgets in Flutter as opposed to Kotlin. With the greater flexibility offered by Flutter widgets, I was able to make improvements in the UI, seen below.

![Feature Graphic](images/Feature_graphic.png)

I also created a Google Play developer account to upload it to the Play store so I could share it. If you're interested, you can join the internal testing [here](https://play.google.com/apps/internaltest/4700343135347905465) for a chance to download the app!
