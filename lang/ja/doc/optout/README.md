[TOP](../../README.md)　>　オプトアウトの実装

---

## （オプション）オプトアウトの実装
広告会社によってターゲティング広告に利用されないことをユーザーに選択させることが可能です。アプリケーションの起動時において、プライバシーポリシーや利用規約を表示するダイアログでユーザーがオプトアウトを選択した場合、効果測定の結果の通知と共に、F.O.Xが広告会社に対してそのユーザーがオプトアウトを選択したことを通知します。


![Language](http://img.shields.io/badge/language-Objective–C-blue.svg?style=flat)
```objc
// 初回起動のインストール計測
CYZFoxTrackOption* option = [CYZFoxTrackOption new];
option.optout = YES;
[CYZFox trackInstall:option];
```

![Language](https://img.shields.io/badge/language-Swift-orange.svg?style=flat)
```Swift
// 初回起動のインストール計測
let option: CYZFoxTrackOption = CYZFoxTrackOption()
option.optout = true
CYZFox.trackInstallWithOption(option)
```

---
[トップ](../../README.md)