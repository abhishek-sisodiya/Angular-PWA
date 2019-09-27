*Service Worker detect new build and prompt user to reload.

*To get Notification:
FCM- Firebase cloud messaging.
Realtime-db, collection-fcmTokens,user001

POST: https://fcm.googleapis.com/fcm/send
body:
{"notification": {
  "title": "Hello", 
  "body": "This is Message to firebase"
 },
 "to" : "dJWQc2bFUxSs1lfaA23WK7:APA91bGMYOOBcaQm0IWtPy1lZ0Zui0awmvYQZR6V9woN-0VKZ4o3lY67alp3U-xa0Cl5W86ioyLtnDgdcZ33eh58eraQRkHa63MMortLDNDR5pTlaab6FChzB3SksKWDngQxCZ2B1kpa"
}
