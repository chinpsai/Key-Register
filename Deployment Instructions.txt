# Key Register Phone Icon (PWA) Deployment Instructions

# 1. First, understand one thing
The real program for this app runs on Google Apps Script, so it needs an internet connection to work. The files in this folder are only a "launcher shell plus desktop icon," so that one tap on the icon opens the app.
This means that with no network, the icon will open, but the app itself won't (Apps Script can't run offline).

# 2. Upload to GitHub Pages (free, gives you a web address)

Go to github.com and log in to your account.
Create a new repository (New repository). Name it key-register, choose Public, and click Create.
On the page, click "uploading an existing file" and upload all the files in this folder (index.html, config.js, manifest.webmanifest, sw.js, and the four icons). Click Commit.
Go to the repository's Settings → Pages.
For Source, choose "Deploy from a branch."
For Branch, choose main, set the folder to / (root), and click Save.
Wait 1 minute. A web address will appear at the top of the page, like this: https://your-username.github.io/key-register/
Copy this address.

# 3. Add the icon to a phone's home screen
Android (Chrome):
Open the address above in Chrome → tap ⋮ at the top right → "Install app" or "Add to home screen" → Install.

iPhone (Safari, you must use Safari):
Open the address in Safari → tap the "Share" button at the bottom → scroll down and find "Add to Home Screen" → Add.

When done, a Key Register icon appears on the home screen. Tap it to open the app.

# 4. If you want to change the code later
After editing, upload the files to the GitHub repository again, overwriting the files with the same names. Refresh once on the phone and the change takes effect. There's no need to install again.

# 5. If colleagues want to install from a file (Android)
Go to https://www.pwabuilder.com, enter your github.io address, and it will generate an Android APK that you can send to colleagues to install. iPhone doesn't support this method.
