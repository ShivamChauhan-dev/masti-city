# Masti City — Android game

Ye ek poora Android app project hai. Game phone mein install hoga, apne icon ke saath,
full screen aur landscape mein chalega, aur bina internet ke bhi khelega.

## Tarika 1: Android Studio se APK banao (computer chahiye)

1. Android Studio download karke install karo: https://developer.android.com/studio
2. Ye zip extract karo. Android Studio kholo, "Open" dabao aur `MastiCity` folder chuno.
3. Pehli baar wo kuch cheezein download karega (5–10 minute). Neeche progress bar khatam hone do.
4. Upar menu se: Build → Build App Bundle(s) / APK(s) → Build APK(s).
5. Ban jaane par "locate" link aayega. File ka naam `app-debug.apk` hoga.
6. Ye APK phone mein bhejo (WhatsApp, USB, Google Drive) aur khol ke install karo.
   Phone "unknown apps" ki permission maange to us app ke liye allow kar do.

Phone USB se juda ho (Developer options mein USB debugging on) to seedha hara ▶ Run button
dabane se game phone mein install hokar khul jaayega.

## Tarika 2: GitHub se APK banao (Android Studio install nahi karna)

1. github.com par account banao aur ek naya repository banao.
2. "uploading an existing file" se is folder ki saari files upload karo
   (`.github` folder bhi zaroori hai).
3. Repository mein "Actions" tab kholo. "APK banao" apne aap chalega (3–5 minute).
4. Hara ✓ aane par us run ko kholo, neeche "Artifacts" mein `MastiCity-apk` download karo.
   Uske andar `app-debug.apk` hai — use phone mein install karo.

## Game badalna ho to

Poora game `app/src/main/assets/index.html` mein hai. Usme badlav karke APK dobara banao.
App ka naam `app/src/main/res/values/strings.xml` mein hai.

## Play Store par daalna ho to

Build → Generate Signed App Bundle se `.aab` file banao aur Google Play Console
(ek baar ki $25 fees) par upload karo. Bacchon ke liye game ho to Play Console ke
"Families" niyam bhi bharne padte hain.
