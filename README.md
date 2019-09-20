# ionic_Push_notification_Postman

Follow This link
https://enappd.com/blog/implement-ionic-4-firebase-push/34/

//POST: https://fcm.googleapis.com/fcm/send
//HEADER: Content-Type: application/json
//HEADER: Authorization: key=AIzaSy*******************
{
  "notification":{
    "title":"Push new",
    "body":"Push Notification ionic 3",
    "subtitle":"This is sub title",
    "sound":"default",
    "click_action":"asif",
    "color": "#228B22",
    "badge": "8",
    "icon":"fcm_push_icon"
    
  },
  "data":{
    "key1":"value1",
    "key2":"value2",
    "meta":{
    	"tnt":"ekushal"
    }
  },
    "to":"/topics/notpayed",
    "priority":"high",
    "restricted_package_name":"com.tnt.app"
}
//sound: optional field if you want sound with the notification
//click_action: must be present with the specified value for Android
//icon: white icon resource name for Android >5.0
//data: put any "param":"value" and retreive them in the JavaScript notification callback
//to: device token or /topic/topicExample
//priority: must be set to "high" for delivering notifications on closed iOS apps
//restricted_package_name: optional field if you want to send only to a restricted app package (i.e: com.myapp.test)
