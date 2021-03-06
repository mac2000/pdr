# pdr

## Path

```bash
export PATH=$PATH:/Users/mac/Documents/sandbox/flutter/udemy/flutter/bin
```

## (Flutter Launcher Icons)[https://pub.dartlang.org/packages/flutter_launcher_icons]

```bash
flutter packages pub run flutter_launcher_icons:main
```

TODO:

# Images

assets/questions - self made images
assets/images - original images

# Resize images trick

```bash
brew install imagemagick
./resize.sh
```

# Build

```bash
flutter build apk
flutter build ios --release
```

APK located at: `build/app/outputs/apk/release/app-release.apk`
APP located at: `build/ios/iphoneos/Runner.app`

# Release

Change version in `pubspec.yaml`

`version: 1.3.0+4` -> `version: 1.3.0+5` e.g. increment last number without it google wont allow you to upload apk complying it already have this version

## Google

[Go to](https://play.google.com/apps/publish/?account=6448344011839007794#ManageReleasesPlace:p=ua.net.marchenko.pdr&appid=4972343131826316274) Release management \ App releases and click on manage link in production track

In production releases window click on "Create release" button

Tap on "Browse files" button and choose apk

## Apple

- [docs](https://flutter.dev/docs/deployment/ios)
- [my apps](https://appstoreconnect.apple.com/WebObjects/iTunesConnect.woa/ra/ng/app)
- [app ids](https://developer.apple.com/account/ios/identifier/bundle)

```
open ios/Runner.xcworkspace
```

menu Product \ Archive \ Distribute App

open source questions and images

codemagic.io

python -c 'import os, json; print json.dumps(os.listdir("assets/questions"))' > assets/questions.json

# Prerequisites

## [Dart SDK](https://www.dartlang.org/tools/sdk#install)

```bash
brew tap dart-lang/dart
brew install dart
```

## [Flutter](https://flutter.dev/docs/get-started/install/macos)

```bash
git clone https://github.com/flutter/flutter
export PATH=$PATH:~/src/github.com/flutter/flutter/bin
```

## Keys

Put key.properties and key.jks to android directory

# Privacy policy

[WebsitePolicies](https://www.websitepolicies.com/policies/manage)
