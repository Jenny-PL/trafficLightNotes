# Tech stack:
1. Typescript
2. React
3. HTML/CSS
4. Python
5. Flask
6. DB? (SQL?)

Deployment Plan:  
[PWA (progressive web app)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
    - **This allows you to download the app onto your phone and use with an icon.**
   1. Will need to add a `manifest file` 
        - [manifest file](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Installable_PWAs)
   2. The file with contain 4 things:
      1. A web manifest, with the correct fields filled in
      2. The web site to be served from a **secure (HTTPS)** domain
      3. An icon to represent the app on the device
      4. A service worker registered, to allow the app to work offline (this is required only by Chrome for Android currently)
