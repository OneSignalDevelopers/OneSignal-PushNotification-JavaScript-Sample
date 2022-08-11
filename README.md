# OneSignal OneSignal-PushNotification-JavaScript-Sample

<p>
  <a href="https://github.com/OneSignal/onesignal-expo-plugin/graphs/commit-activity" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a>
  <a href="https://twitter.com/onesignaldevs" target="_blank">
    <img alt="Twitter: onesignaldevelopers" src="https://img.shields.io/twitter/follow/onesignaldevs?style=social" />
  </a>
</p>

This sample code shows how to add push notifications to your website using [OneSignal](https://onesignal.com/) and JavaScript.

## Requirements
- [OneSignal Account](https://onesignal.com/)

#### OneSignal Keys
Learn how to get the OneSignal App ID and OneSignal API Key [here](https://documentation.onesignal.com/docs/accounts-and-keys).

### Adding OneSignal To Your Website
You can add the following code to your *index.js* file like shown in this code sample or inside of you html `<head>` tag wrapped with a `<script>` tag.

The following code will make OneSignal aware that this website will be using the OneSignal Push Notifications and it will allow the users to subscribe to the website to start receving the notifications.

```javascript
window.OneSignal = window.OneSignal || [];
OneSignal.push(function() {
    OneSignal.init({
        appId: "YOUR-APP-ID",
        safari_web_id: "YOUR-SAFARI-WEB-ID",
        notifyButton: {
            enable: true,
            size: "small",
            position: "bottom-left",
        },
        allowLocalhostAsSecureOrigin: true,
    });
});
```

In the code above, We are using the [notifyButton](https://documentation.onesignal.com/docs/web-push-sdk#init-notifybutton-parameters) property which will add a bell Icon with the properties specified such as the size and the position.

### Show Your Support

Give a :star:️ if this project helped you!

### Join the OneSignal Developers Community
The OneSignal Developer community is a group of passionate individuals who work with OneSignal products. Community members have the opportunity to expand their network and knowledge across different technologies.

* Website: https://onesignal.com/onesignal-developers
* Twitter: [@OneSignalDevs](https://twitter.com/onesignal)
* Github:  [@OneSignalDevelopers](https://github.com/OneSignal)
* Discord: [@onesignal-metabase](https://linkedin.com/company/onesignal)
