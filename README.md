# romashka-site

Static public pages for the Romashka app, served by GitHub Pages from `main`.

| Page | Path | Used for |
|---|---|---|
| Account deletion (RU/EN, Android/iOS) | `delete-account/` | Google Play → Data safety → Data deletion URL; App Store Connect → App Privacy |

Plain HTML, no build step. Fonts (Onest) and brand colours are copied from the Android app
(`romashka-android/app/src/main/res/font`, `presentation/common/theme`). Screenshots come from the app with
personal data blurred. Android screenshots are `img/step*.webp`, iOS ones are `img/ios-step*.webp`.

The page shows the steps for the visitor's platform (iPhone/iPad → iOS, otherwise Android); `?platform=ios` or
`?platform=android` forces one, and the switch next to the heading changes it.

Preview locally: `python3 -m http.server 8741` and open http://localhost:8741/delete-account/.
