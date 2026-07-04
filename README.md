# PhantomLives releases

Public distribution home for the PhantomLives apps. The source monorepo
(`bronty13/PhantomLives`) is private; this repo holds only what installed
apps and users need to fetch anonymously:

- **Release assets** — installers/zips per app, under per-app tags
  (`molly-v*`, `sidemolly-v*`, `purplemind-v*`, `purplededup-v*`, …).
- **Rolling updater feeds** — one prerelease per Tauri app holding the
  newest updater manifest (`molly-updater-feed`, `sidemolly-updater-feed`,
  `purplemind-updater-feed`). App updater endpoints point here.
- **Sparkle appcasts** — `<App>/appcast.xml` committed in this repo, served
  raw (`raw.githubusercontent.com/bronty13/phantomlives-releases/main/...`).

Nothing here is authored by hand: release scripts and CI in the private
monorepo publish into this repo. Do not delete the `*-updater-feed`
prereleases — installed apps poll them.
