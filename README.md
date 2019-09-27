[![Actions status][actions-image]][actions-url]
[![Dependency status][david-dm-image]][david-dm-url]
[![Dev Dependency status][david-dm-dev-image]][david-dm-dev-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]

# angular-pwa-sample

![lightouse](./lighthouse.png)

This is a PWA sample using Angular CLI.

This sample contains following features.
- Angular Service Worker
- App Shell with Angular Universal

## Tutorial

1. Install Angular CLI

```shell
$ npm i -g @angular/cli
```

2. Create an app

```shell
$ ng new my-app --routing --style=css
$ cd my-app
```

3. Add service worker

```shell
$ ng add @angular/pwa
```

4. Generate App Shell

```shell
$ ng g app-shell --client-project=my-app --universal-project=my-app
```

5. Run `ng run` to build the app

```shell
$ ng run my-app:app-shell:production
```

Congratulations ! Your Angular application is built in `dist/my-app`.

You can see the app by using a static file server.

```
$ npx serve -s ./dist/my-app
```

[actions-url]:https://github.com/puku0x/angular-pwa-sample/actions
[actions-image]:https://action-badges.now.sh/puku0x/angular-pwa-sample?branch=master
[david-dm-url]:https://david-dm.org/puku0x/angular-pwa-sample
[david-dm-image]:https://david-dm.org/puku0x/angular-pwa-sample.svg
[david-dm-dev-url]:https://david-dm.org/puku0x/angular-pwa-sample?type=dev
[david-dm-dev-image]:https://david-dm.org/puku0x/angular-pwa-sample/dev-status.svg
[snyk-url]:https://snyk.io/test/github/puku0x/angular-pwa-sample
[snyk-image]:https://snyk.io/test/github/puku0x/angular-pwa-sample/badge.svg



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
