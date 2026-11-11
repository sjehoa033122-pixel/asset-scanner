HOSPITAL ASSET SCANNER - hosting + APK steps

1) HOST THE FOLDER (free, about 5 minutes) - GitHub Pages
   - Create a free account at github.com, make a new PUBLIC repository (e.g. asset-scanner).
   - Upload everything from this folder (index.html, manifest.json, sw.js, lib/, icons/).
   - Repository Settings > Pages > Source: "Deploy from a branch", branch: main, folder: / (root). Save.
   - After a minute your app is live at https://YOURNAME.github.io/asset-scanner/
   - Test it on your phone (Chrome): camera should work and "Add to Home screen" should appear.
   Note: a public repo means anyone with the link can open the app. Your asset data is NOT in the repo; it is saved on each phone.

2) MAKE THE APK
   - Go to https://www.pwabuilder.com , paste your live address, press Start.
   - Choose Package for stores > Android > Generate. Download the zip.
   - Inside is an .apk (for sideloading) and an .aab (Google Play). Send the .apk to staff phones and tap to install (allow "install unknown apps").
   - Keep the signing key file PWABuilder gives you; you need it for future updates.

Data note: each phone keeps its own inventory (saved on the device). Use Report > Export CSV to back up or combine.
