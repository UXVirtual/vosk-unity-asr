# Vosk Unity ASR Sample (Japanese)

## Tested Unity Version

- Unity 6000.0.32f1

## Quick Start

1. Clone or download this repository.
2. **Unity Hub → Open** でプロジェクトを開きます。
3. Demoシーンを開いて実行します

## Unity Package Manager からの導入

既存プロジェクトに Vosk ライブラリのみを追加したい場合は、以下の手順で Unity Package Manager (UPM) に Git URL を指定してください。

1. Unity エディタで `Window > Package Manager` を開く  
2. `+` ボタン → **Add package from git URL...** を選択  
3. 次の URL を入力して **Add** を押す

```
https://github.com/ayutaz/vosk-unity-asr.git?path=Assets/ThirdParty/Vosk
```

これによりパッケージ名 `com.yousan.vosk` がインストールされます。依存ライブラリ `com.unity.nuget.newtonsoft-json` (v3.2.1) も自動で解決されます。

## 内容

- `Assets/Scripts/` : サンプルスクリプト類  
- `Assets/ThirdParty/Vosk` : Vosk C# バインディング & ネイティブ DLL  
- `Packages/manifest.json` : Newtonsoft.Json 依存が追加されています

## 備考

- マイク入力が必要です (Windows の場合はプライバシー設定で本アプリのマイク使用を許可)。
- 音声合成機能は macOS 専用 `/usr/bin/say` を呼んでいましたが、Windows では無効化しています。
