# camerite-android-exercise

- You have up to 1 day to complete the assignment;
- You need to fork the project and send a PR for the main repository.

Overview
--------

This test will validate your knowledges of Android, we have an preference for the quality and inovation. Then, you are open to choose any technology to create your application.

The test is simple: Request the data from our service, parse and show the data on a list. When the user click on the list, open a new screen, it needs to show the informations of determined item.

We will verify the consistency of the application and the structure used, unit tests are a plus. Do your best.

Tasks
-----

- Develop the app using Android Studio + Gradle + JUnit ­- 100% native.
- Handle errors, such as, no internet available, 4XX & 5XX & show a specific message for each one:
  * No Internet Available - “Parece que você está sem internet! Por favor, verifique a sua conexão e tente novamente.”;
  * 4XX- “Houve algum erro na requisição.”;
  * 5XX- “Desculpe, estamos enfrentando problemas técnicos. Por favor, tente novamente mais tarde.”.

Recommendations
---------------

- OkHttp;
- LoganSquare, Gson or Moshi;
- MVP, MVVM or anything else;
- jUnit;
- Any imageloader;
- Support Library;
- RecyclerView.

Data
----

The REST API is available at:

https://camerite.com/test/content.json

Strucuture
----------

List of videos

```json
[{
  "id": 45,
  "title": "Driving a fast car",
  "video_address": "https://somerandomurl.com/videos/824532398.mp4",
  "views": 64389,
  "shot_cdn": "https://d34dchjfu9xdhv.cloudfront.net",
  "user": {
    "id": 931,
    "username": "Camerite guy",
    "followers": 8753,
    "status": 0
  }
}]
```

- `id`: Id of the video on database;
- `title`: Title of the video;
- `video_address`: Address of the video, can be a .mp4;
- `views`: Total of view for the video;
- `user.id`: Id of the user;
- `user.username`: Name of the user;
- `user.followers`: Number of people that follow the user;
- `status`: 0 - Enabled, 1 - Disabled, 2 - Banned.

To load your image, you need to use the `shot_cdn` + `/public/test/images/` with the id(the last id before `.mp4`) of `video_address` + `.jpg`.

Any question? Send a email to pedro@camerite.com, sidney@camerite.com or cristian@camerite.com.