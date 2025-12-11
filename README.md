# HpEasyAuthentication
Easy workflow for basic authentication in Unity Projects

### Requirements
1. Sign in with Apple requires **App ID**. https://developer.apple.com 
2. Sign in with Google Play Games requires **Client ID & Secret** https://play.google.com/console/developers


### Packages To Install (First Steps)
1. Authentication (com.unity.services.authentication)
2. Apple Auth: https://assetstore.unity.com/packages/tools/integration/sign-in-with-apple-plugin-for-unity-152088
3. Play Games Unity Plugin: https://github.com/playgameservices/play-games-plugin-for-unity/tree/master/current-build
4. Dowload and import the hpeasyauthentication unity package


### Setup

1. Developer Apple
* Create New App
* While setting up "Certificates, Identifiers & Profiles", ensure Capabilities, **Sign
  In with Apple** is enabled
* Copy App ID (Bundle Id - com.companyname.product)

2. Play Games Console
* Create new app
* Setup instructions https://developer.android.com/games/pgs/unity/unity-start
  (Create Google Cloud Console Project,setup consent page, create **Web** OAuth client 
  ID, 
  Copy/Download web client ID and secret, Add Test audience,
  Link cloud project to Play 
  Games 
  Services in 
  Play Console, add game server credentials)

3. Cloud Unity
* Goto https://cloud.unity.com create a project or select an existing one
* Goto **Player Authentication**  under Gaming Services
* Select **Identity Providers**
* Add Identity Providers, *Unity Player Accounts* , *Sign in with Apple* , *Google
  Play Games*
* Add necessary information
* Create/Change Environment to development

4. Unity Editor
* Setup Android Setup for Play Games (Resources & Nearby setup)
* Project Settings -> Authentication, all selected Identity Providers should appear 
  with all fields filled.
* Add entitlements build post process script for iOS builds 
