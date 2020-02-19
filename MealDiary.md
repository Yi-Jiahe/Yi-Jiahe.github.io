Meal Diary is an app meant to help users keep track of their diet in order to assist them in eating healthier. It seeks to do so by simplifying the process of recording one's meals, encourging awareness over counting calories by making creating a new entry as easy as simply taking a picture of your meal.

While this was not techincally my first foray into app development for I had created a simple web app a number of years earlier, it was my first time writing an app specifically for android in Kotlin. The reason I had chosen to create the app was because I felt that the introduction of Kotlin and Android Studio made the app development process more accessible than before, and I thought that it was my turn to give it a shot.

When I first started learning Kotlin, I picked up most of the basic skills from the tutorial by Google by building and experimenting with their introductory apps, incorporating the knowledge I gained from them into my own app. However, as my app grew more complex with more interations and features, I had to cast my net wider and scour the internet or possible solutions to the difficulties I began to encounter. After much trial and error, I had finally managed to include the features I had desired to include.

The app makes use of intents to use the in-built camera app to take a photo, then uses the Google Places API to provide a location tag to the image, allowing location and time data to be stored. Each entry is stored locally on the user's device, and collectively they are used to populate the RecyclerView used to display the entries. The result can be seen in the screenshot below.

![Meal Diary Screenshot](/images/Meal-Diary-SS.jpeg =250x)

If you are interested in trying the app in its latest stable version, please download the apk [here](/downloadable/Meal Diary v0.1.0.apk). Please note that this version is not meant for commercial use and some features might be unavaliable should the number of API requests exceed my key's quota.

During a recent NTU module, CY0006 Enterprise, Innovation and Leadership, my group and I are looking into the feasibilty of such an app based on its desirablity to actual users. In the process we have gathered postive feedback and learnt more about the revenue and dependency costs of running an app. We are also looking into utilising the Google Vision API to provide more details on the pictures.
