# Mobile app
### Steps to build the app:
-  Installation of [Android Studio](https://developer.android.com/studio)
-  Installation of [ngrok](https://ngrok.com/) 

We execute the ngrok script and type in the command:
````
ngrok http https://localhost:8765/
````

In the file *RequestManager.kt* (path:CGEEnergy\app\src\main\java\com\cge\cgeenergy\managers) we modify the baseURL with the *url* we see on our *ngrok* terminal

We then connect our android device and launch the application

