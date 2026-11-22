# mactyagi.github.io

Support pages for my iOS apps, served by GitHub Pages at https://mactyagi.github.io.

- `app-ads.txt`: the AdMob seller line. It has to stay at the root of the domain,
  and one file covers every app on this AdMob account.
- `index.html`: the list of apps.
- `cleava/`: support page for Cleava: Clean Storage Space.
- `cleava/privacy/`: Cleava's privacy policy. It names every service the app sends data to, so update it when one is added or removed.
- `cleava/terms/`: Cleava's Terms of Use, which is also the custom EULA in App Store Connect.
  Paste the same text into App Store Connect when this page changes.
- `habit-tracker/privacy/`: the privacy policy of Habitude: Build & Quit Tracker. The folder keeps the app's first
  name because App Store Connect and the app link to it. No support page yet, and not on the list in `index.html`
  until the app is on the App Store. Like Cleava's, it names every service the app sends data to and what goes there,
  so update it when the app starts sending something new (a Firebase product, a new analytics event, a new field in
  Help & About's messages), together with the App Privacy answers in App Store Connect.

## Adding an app

1. Copy `cleava/` to a new folder named after the app and edit the text.
2. Add the app to the list in `index.html`.
3. In App Store Connect, set the app's Support URL to `https://mactyagi.github.io/<folder>/`
   and its Marketing URL to the same address (AdMob checks this domain for `app-ads.txt`).
