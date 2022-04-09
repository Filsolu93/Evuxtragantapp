# Evuxtragantapp

To make a call, you first need to create an instance of SinchClient:

SinchClient sinchClient = Sinch.getSinchClientBuilder()
        .context(this)
        .userId("current-user-id")
        .applicationKey("app-key")
        .applicationSecret("app-secret")
        .environmentHost("sandbox.sinch.com")
        .build();
Make sure to fill in app-key and app-secret with the key and secret you generated when creating an app in the dashboard! Then, tell the sinch client that you want to have calling in your app, and finally, start the client:

