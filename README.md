# Simple-room

TV Application sample to create a "room" and send/receive message in this "room" with Box Api.
The "room" may be usefull if you want to synhronize the user profile parameters from your mobile App with the TV App.

### Setup Android Studio

Do not forget to set your own credentials (appId and appSecret) provided by Bouygues Telecom in order to build your APK in this file : https://github.com/BboxLab/bboxapi-client-android/blob/master/bboxapi/src/main/res/values/strings.xml

BBOXAPI_APP_ID and BBOXAPI_APP_SECRET are given by Bouygues Telecom. If you dont have these, here is following contact https://dev.bouyguestelecom.fr/dev/?page_id=51

## First step

Create a room (case sensitive) from this TV Application

Send msg to or from this App or from a third party App (bboxapi-client-android https://github.com/BboxLab/bboxapi-client-android)

## Send msg 

curl -X POST -H "x-sessionid: xxxxxxxxxx" -H "Content-Type: application/json" -d '{
  "appId": "string",
  "message": "string"
}' "http://bboxIp:8080/api.bbox.lan/v0/notification/Message/roomName"

Info "x-sessionId" -> https://api.bbox.fr/doc/#Getting%20started


## Authors
* **Gun95**

## License
The MIT License (MIT) Copyright (c) 2017 BboxLab
