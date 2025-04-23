React Native Chat App
Feature	:
Signup & Login ->	Users can create an account and log in using their email and password (handled via Firebase).
Send Text Message	-> Basic chat feature for sending normal messages.
Send Picture ->	Share images without any quality loss.
Group Chat	-> Chat with multiple friends at once, just like a group.
Delete Chat	-> Long press on a chat to delete it whenever you want.
Delete Account ->	You can completely remove your account from the app.
Real-Time Chat	-> Latest message always appears at the top in real-time.

💾 Installation Guide – 
To get this app running on your system, make sure you’ve already installed Git and Node.js (npm comes with it).

Steps to Run the App:

-> Clone the project

->Go inside the folder

->cd react-native-chat
Install the required packages :

-> npm install
Start the app using Expo

-> npx expo start
⚠️ Important: Don’t forget to create your .env file and add Firebase credentials there. Check the docs or comments for help.

-> On your phone:

Install Expo Go from Play Store or App Store

-> Scan the QR code that appears after running the above command to test the app on your phone

🏗️ Build Guide – Easy Steps
To build the app for Android:

-> Make sure your .env file is ready with all Firebase details.

Push environment variables to EAS:

eas secret:push --scope project --env-file .env
-> Start the Android build (using preview profile):

eas build -p android --profile preview
👉 This will create an APK you can install on your device.

📝 Notes to Keep in Mind:
.env is for local use with Expo CLI.

-> For actual builds, define environment variables in eas.json (so they work on EAS Build servers too).

It’s okay to have same variables in both .env and eas.json for smoother builds.

🧪 Want to Build Locally Instead?
Use these commands:

# To build for Android
npm run android

# To build for iOS
npm run ios
