# Rayfield for Android TV

**A TV-focused client for the Rayfield media ecosystem.**

This repository contains Rayfield's Android TV client, based on Jellyfin for Android TV. It is intended for television and remote-control use, connecting to a compatible self-hosted media server so you can browse and play media from the comfort of your living room.

## Project goals

- **TV-first navigation** designed around directional-pad and remote-control interaction.
- **Personal media access** through a compatible Rayfield/Jellyfin server.
- **Open-source development** with a codebase that can be inspected and improved.
- **Upstream-aware maintenance** that respects the project's Jellyfin lineage and existing notices.

## Building locally

The project uses Gradle and the Android SDK. The build instructions below explain how to generate a debug APK. Review the repository's license and attribution notices before redistributing modified builds.

Rayfield is an independent project derived from Jellyfin for Android TV.

---

## Building

The app uses Gradle and requires the Android SDK. We recommend using Android Studio, which includes all required dependencies, for
development and building. For manual building without Android Studio make sure a compatible JDK and Android SDK are installed and in your
PATH, then use the Gradle wrapper (`./gradlew`) to build the project with the `assembleDebug` Gradle task to generate an apk file:

```shell
./gradlew assembleDebug
```

The task will create an APK file in the `/app/build/outputs/apk/debug` directory. This APK file uses a different app-id from our stable
builds and can be manually installed to your device.

## Branching

The `master` branch is the primary development branch and the target for all pull requests. It is **unstable** and may contain breaking
changes or unresolved bugs. For production deployments and forks, always use the latest `release-x.y.z` branch. Do not base production work
or long-lived forks on `master`.

Release branches are created at the start of a beta cycle and are kept up to date with each published release. Maintainers will cherry-pick
selected changes into release branches as needed for backports. These branches are reused for subsequent patch releases.

## Translating

Translations can be improved very easily from our [Weblate](https://translate.jellyfin.org/projects/jellyfin-android/jellyfin-androidtv)
instance. Look through the following graphic to see if your native language could use some work! We cannot accept changes to translation
files via pull requests.

<p align="center">
<a href="https://translate.jellyfin.org/engage/jellyfin-android/">
<img alt="Detailed Translation Status" src="https://translate.jellyfin.org/widgets/jellyfin-android/-/jellyfin-androidtv/multi-auto.svg"/>
</a>
</p>
