# Vosk Unity ASR Sample (Japanese)

## Tested Unity Version

- Unity 6000.0.32f1

## Quick Start

1. Clone or download this repository.
2. Open the project via **Unity Hub → Open**.
3. Open and run the Demo scene.

## Installation via Unity Package Manager

If you wish to add only the Vosk library to an existing project, please specify the Git URL in the Unity Package Manager (UPM) by following these steps.

1. Open `Window > Package Manager` in the Unity editor.
2. Click the `+` button → select **Add package from git URL...**
3. Enter the following URL and click **Add**:

```
https://github.com/ayutaz/vosk-unity-asr.git?path=Assets/ThirdParty/Vosk
```

This will install the package `com.yousan.vosk`. The dependency library `com.unity.nuget.newtonsoft-json` (v3.2.1) will also be resolved automatically.

## Contents

- `Assets/Scripts/`: Sample scripts
- `Assets/ThirdParty/Vosk`: Vosk C# bindings and native DLLs
- `Packages/manifest.json`: Newtonsoft.Json dependency has been added

## Notes

- Microphone input is required (on Windows, please allow this app to use the microphone in your privacy settings).
- The speech synthesiser feature previously called the macOS-exclusive `/usr/bin/say`, but it has been disabled for Windows.
