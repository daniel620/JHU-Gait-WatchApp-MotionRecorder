# JHU-Gait-WatchApp-MotionRecorder
## Environment
Swift language version: Swift 4

Apple watch: watchOS 4.3

iPhone: IOS 12.3.1

## Introduction
1. Access sensors(gyroscope, magnetometer, accelerometer, and heart rate sensor) in iPhone and Apple watch.

2. Export data for further study.

## Directory Tree
```
.
├── JHU-MotionRecorder
│   ├── Controller
│   │   ├── AppDelegate.swift
│   │   ├── CollectingDataVC.swift
│   │   ├── ExportDataVC.swift
│   │   ├── RecordIDVC.swift
│   │   └── SettingsTableVC.swift
│   ├── JHU-MotionRecorder.entitlements
│   ├── Model
│   │   ├── Characteristic+CoreDataClass.swift
│   │   ├── CharacteristicName+CoreDataClass.swift
│   │   ├── DataCollector.xcdatamodeld
│   │   │   └── DataCollector.xcdatamodel
│   │   │       └── contents
│   │   ├── Device.swift
│   │   ├── Generated
│   │   │   ├── Characteristic+CoreDataProperties.swift
│   │   │   ├── CharacteristicName+CoreDataProperties.swift
│   │   │   ├── Sensor+CoreDataClass.swift
│   │   │   ├── Sensor+CoreDataProperties.swift
│   │   │   ├── SensorData+CoreDataProperties.swift
│   │   │   └── Session+CoreDataProperties.swift
│   │   ├── Sensor+CoreDataClass.swift
│   │   ├── SensorData+CoreDataClass.swift
│   │   ├── SensorOutput.swift
│   │   ├── Session+CoreDataClass.swift
│   │   ├── SessionContainer.swift
│   │   └── SessionType.swift
│   ├── Sources
│   │   ├── Assets.xcassets
│   │   │   ├── AppIcon.appiconset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── Icon-App-20x20@1x.png
│   │   │   │   ├── Icon-App-20x20@2x.png
│   │   │   │   ├── Icon-App-20x20@3x.png
│   │   │   │   ├── Icon-App-29x29@1x.png
│   │   │   │   ├── Icon-App-29x29@2x.png
│   │   │   │   ├── Icon-App-29x29@3x.png
│   │   │   │   ├── Icon-App-40x40@1x.png
│   │   │   │   ├── Icon-App-40x40@2x.png
│   │   │   │   ├── Icon-App-40x40@3x.png
│   │   │   │   ├── Icon-App-57x57@1x.png
│   │   │   │   ├── Icon-App-57x57@2x.png
│   │   │   │   ├── Icon-App-60x60@2x.png
│   │   │   │   ├── Icon-App-60x60@3x.png
│   │   │   │   ├── Icon-App-72x72@1x.png
│   │   │   │   ├── Icon-App-72x72@2x.png
│   │   │   │   ├── Icon-App-76x76@1x.png
│   │   │   │   ├── Icon-App-76x76@2x.png
│   │   │   │   ├── Icon-App-83.5x83.5@2x.png
│   │   │   │   ├── Icon-Small-50x50@1x.png
│   │   │   │   ├── Icon-Small-50x50@2x.png
│   │   │   │   └── ItunesArtwork@2x.png
│   │   │   ├── AppleWatch.imageset
│   │   │   │   ├── AppleWatch.png
│   │   │   │   └── Contents.json
│   │   │   ├── Contents.json
│   │   │   ├── cc2650_sensortag.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   └── cc2650_sensortag.png
│   │   │   ├── delete.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── delete.png
│   │   │   │   ├── delete@2x.png
│   │   │   │   └── delete@3x.png
│   │   │   ├── error.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── error.png
│   │   │   │   ├── error@2x.png
│   │   │   │   └── error@3x.png
│   │   │   ├── export_csv.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── export_csv.png
│   │   │   │   ├── export_csv@2x.png
│   │   │   │   └── export_csv@3x.png
│   │   │   ├── iPhone.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   └── iPhone.png
│   │   │   ├── ok.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── ok.png
│   │   │   │   ├── ok@2x.png
│   │   │   │   └── ok@3x.png
│   │   │   ├── phone.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   └── phone.png
│   │   │   ├── record.imageset
│   │   │   │   ├── Contents.json
│   │   │   │   ├── record.png
│   │   │   │   ├── record@2x.png
│   │   │   │   └── record@3x.png
│   │   │   └── sensor.imageset
│   │   │       ├── Contents.json
│   │   │       ├── sensor.png
│   │   │       ├── sensor@2x.png
│   │   │       └── sensor@3x.png
│   │   └── Info.plist
│   └── View
│       ├── Base.lproj
│       │   ├── LaunchScreen.storyboard
│       │   └── Main.storyboard
│       ├── ItemSessionSessionCell.swift
│       ├── RoundButton.swift
│       └── SessionIDCell.swift
├── JHU-MotionRecorder.xcodeproj
│   ├── project.pbxproj
│   ├── project.xcworkspace
│   │   ├── contents.xcworkspacedata
│   │   ├── xcshareddata
│   │   │   ├── IDEWorkspaceChecks.plist
│   │   │   ├── WorkspaceSettings.xcsettings
│   │   │   └── swiftpm
│   │   └── xcuserdata
│   │       └── kuzaowuwei.xcuserdatad
│   │           ├── IDEFindNavigatorScopes.plist
│   │           ├── UserInterfaceState.xcuserstate
│   │           └── WorkspaceSettings.xcsettings
│   └── xcuserdata
│       └── kuzaowuwei.xcuserdatad
│           ├── xcdebugger
│           │   └── Breakpoints_v2.xcbkptlist
│           └── xcschemes
│               └── xcschememanagement.plist
├── JHU-MotionRecorderWatch
│   ├── Assets.xcassets
│   │   ├── AppIcon.appiconset
│   │   │   ├── Contents.json
│   │   │   ├── Icon-24@2x.png
│   │   │   ├── Icon-27.5@2x.png
│   │   │   ├── Icon-29@2x.png
│   │   │   ├── Icon-29@3x.png
│   │   │   ├── Icon-40@2x.png
│   │   │   ├── Icon-44@2x.png
│   │   │   ├── Icon-86@2x.png
│   │   │   ├── Icon-98@2x.png
│   │   │   └── iTunesArtwork@2x.png
│   │   └── Contents.json
│   ├── Base.lproj
│   │   └── Interface.storyboard
│   └── Info.plist
├── JHU-MotionRecorderWatch Extension
│   ├── Assets.xcassets
│   │   └── Complication.complicationset
│   │       ├── Circular.imageset
│   │       │   └── Contents.json
│   │       ├── Contents.json
│   │       ├── Extra Large.imageset
│   │       │   └── Contents.json
│   │       ├── Graphic Bezel.imageset
│   │       │   └── Contents.json
│   │       ├── Graphic Circular.imageset
│   │       │   └── Contents.json
│   │       ├── Graphic Corner.imageset
│   │       │   └── Contents.json
│   │       ├── Graphic Extra Large.imageset
│   │       │   └── Contents.json
│   │       ├── Graphic Large Rectangular.imageset
│   │       │   └── Contents.json
│   │       ├── Modular.imageset
│   │       │   └── Contents.json
│   │       └── Utilitarian.imageset
│   │           └── Contents.json
│   ├── ComplicationController.swift
│   ├── ExtensionDelegate.swift
│   ├── Info.plist
│   ├── MainIC.swift
│   ├── MotionCollectorWatch Extension.entitlements
│   ├── NotificationController.swift
│   └── PushNotificationPayload.apns
├── LICENSE
└── images
    ├── screenshot1.png
    ├── screenshot2.png
    ├── screenshot3.png
    └── screenshot4.png

48 directories, 127 files
```
