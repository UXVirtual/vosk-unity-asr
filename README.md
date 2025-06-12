# Vosk Unity ASR Sample (Japanese)

## Tested Unity Version

- Unity 6000.0.32f1

## Quick Start

1. Clone or download this repository.
2. **Unity Hub → Open** でプロジェクトを開きます。
3. Demoシーンを開いて実行します

## 内容

- `Assets/Scripts/` : サンプルスクリプト類  
- `Assets/ThirdParty/Vosk` : Vosk C# バインディング & ネイティブ DLL  
- `Assets/ThirdParty/SimpleJson` : JSON パーサ (Vosk 結果解析に使用)

## 備考

- マイク入力が必要です (Windows の場合はプライバシー設定で本アプリのマイク使用を許可)。
- 音声合成機能は macOS 専用 `/usr/bin/say` を呼んでいましたが、Windows では無効化しています。
