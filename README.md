# tripbuddy-public

As the name implies, this repo contains all things that are public which are used in the app. This repo is used to serve static content to both the `iOS` and `Android` apps. All resources are served using [RawGit](https://rawgit.com/) so that we can get the right `Content-Type` in the response header

### Strings
The `iOS` and `Android` both request strings from this repo. Doing this approach we can easily change a string without having to make new build. Also users can get localized strings from this repo based on their device settings. 

The app is very smart to know languages that are supported. If a `Locale` isn't supported, it simply requests for the default which is `strings-en_US.json`

To get a string in the app, use: `LOCALIZATION_BASE_PATH` + **LOCALE-CODE.json**

Here is an example: https://cdn.rawgit.com/tawrahim/tripbuddy-public/master/strings-en_US.json

### Static web resources
| File          | Variable Name  | DEV Link  | PROD Link        |
|:-------------:|:-------------:|:-------------:|:-------------:|
| privacy.html | `PRIVACY_URL` | [Link](https://rawgit.com/tawrahim/tripbuddy-public/master/privacy.html) | [Link](https://cdn.rawgit.com/tawrahim/tripbuddy-public/master/privacy.html) |
| faq.html | `FAQ_URL` | [Link](https://rawgit.com/tawrahim/tripbuddy-public/master/faq.html) | [Link](https://cdn.rawgit.com/tawrahim/tripbuddy-public/master/faq.html) |
| terms.html | `TOS_URL` | [Link](https://rawgit.com/tawrahim/tripbuddy-public/master/terms.html) | [Link](https://cdn.rawgit.com/tawrahim/tripbuddy-public/master/terms.html) |
| licenses.html | `LICENSE_URL` | [Link](https://rawgit.com/tawrahim/tripbuddy-public/master/licenses.html) | [Link](https://cdn.rawgit.com/tawrahim/tripbuddy-public/master/licenses.html) |
