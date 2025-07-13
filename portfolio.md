# コードリーダー

## 概要
スキャン結果の可視性に特化した、シンプルで使いやすいQR／バーコードスキャン機能を備えたAndroidアプリ。

時間が経ってからスキャン結果を確認する場合でも、目的の情報をすぐに見つけられるような仕組みを採用。

サブ機能としてQRコードの作成機能を備える。

## 言語、ライブラリ
* Kotlin
* Jetpack Compose
* Flow
* StateFlow
* Coroutines
* Hilt
* Jetpack Navigation Component
* Adaptive Navigation Suite
* OSS Licenses
* AdMob

## アーキテクチャ
* MVVM
* Clean Architecture
* マルチモジュール
* Version Catalog
* Convention Plugins

## UnitTest
* JUnit4
* Mockito
* Truth
* Turbine

## 非機能

| 分類 | 内容 |
|-----|-----|
| 対応OS | Android OS10以降 |
| パフォーマンス | 通常の利用でストレスを感じない動作速度 |
| セキュリティ | アプリ内データベースに暗号化してデータ保存（Room + Tink） |
| 可用性 | オフラインでも基本操作が可能<br>（スキャンモジュールがインストール済みの前提） |
| UI/UX | シンプル、且つ、直感的な画面設計 |

## 機能

| 機能名 | 概要 | ライブラリ等 |
|-----|-----|-----|
| QRコード/バーコードのスキャン | 端末のカメラで読み取り、読み取ったデータを解析したのちに保存、表示する | Google Code Scanner、MlKit、Room、Tink、Jetpack Compose |
| スキャン結果の一覧表示 | スキャン結果をリスト形式で表示 | Jetpack Compose、jsoup + Coil（ファビコン表示） |
| スキャン結果の詳細表示 | スキャン結果の詳細データを表形式で表示 | Jetpack Compose、jsoup + Coil（ファビコン表示） |
| スキャン結果の削除 | 一覧表示からの複数選択削除、詳細表示からの削除 | Room、Jetpack Compose |
| スキャン結果の検索 | 任意の検索ワード、追加条件（履歴、お気に入り、各種カテゴリ）、昇順・降順を使用して検索 | Jetpack Compose |
| スキャン結果の共有 | QR画像形式で端末内の他アプリを介して共有 | Zixing、FileProvider、app chooser（Intent） |
| スキャン結果の他アプリ連携 | URL形式データのブラウザ表示、カレンダーイベント形式データのカレンダー保存・イベント開催場所のGoogle Map検索、<br>連絡先形式データの電話帳登録、電話番号形式データの電話発信、メール形式データのメール作成、<br>SMS形式データのSMS作成、位置情報形式データのGoogle Map検索 | Chrome Custom Tabs、app chooser（Intent） |
| QRコードの作成 | URL、Wi-Fi設定情報、カレンダーイベント、連絡先、メール、SMS、電話番号、位置情報、テキスト（文章）形式のQRコードを作成 | Zixing |
| 作成したQRコードの一覧表示 | 作成したQRコードをリスト形式で表示 | Jetpack Compose、jsoup + Coil（ファビコン表示） |
| 作成したQRコードの詳細表示 | 作成したQRコードの詳細データを表形式で表示 | Jetpack Compose、jsoup + Coil（ファビコン表示） |
| 作成したQRコードの削除 | 一覧表示からの複数選択削除、詳細表示からの削除 | Room、Jetpack Compose |
| 作成したQRコードの共有 | QR画像形式で端末内の他アプリを介して共有 | Zixing、FileProvider、app chooser（Intent） |
| スキャン機能のオプション設定 | スキャンする対象の形式に合わせてスキャン精度を上げる<br>（QR CODE、AZTEC、CODE128、CODE39、CODE93、CODEBAR、DATA MATRIX、ITF、PDF417） | Google Code Scanner、MlKit |
| アプリのテーマ切り替え | ダイナミックカラー、ダークモード | Jetpack Compose、DataStore |

## モジュール構成

### app

* [app](module/app.md)

### feature

* [home](module/feature/home.md)
* [create](module/feature/create.md)
* [list](module/feature/list.md)
* [search](module/feature/search.md)
* [setting](module/feature/setting.md)

### core

* [common](module/core/common.md)
* [data](module/core/data.md)
* [datastrore](module/core/datastrore.md)
* [designsystem](module/core/designsystem.md)
* [domain](module/core/domain.md)
* [model](module/core/model.md)

### utils

* [utils](module/utils.md)

## 画面

* [スプラッシュ](screen/splash.md)
* [利用規約同意](screen/agree_terms)
* [ホーム](screen/home.md)
* [QR作成種類選択](screen/choose_create_qr.md)
* [QR作成](screen/create_qr.md)
* [作成済みQRコード一覧](screen/created_qr_list.md)
* [作成済みQRコード詳細](screen/created_qr_detail.md)
* [履歴一覧](screen/history_list.md)
* [履歴詳細](screen/history_detail.md)
* [お気に入り一覧](screen/favorite_list.md)
* [お気に入り詳細](screen/favorite_detail.md)
* [検索](screen/search.md)
* [設定](screen/settings.md)

## 要改善
* Google Code Scannerの廃止
  * Google 開発者サービスが非搭載の端末（中華系の端末）でもスキャン機能を利用できるように、スキャン機能を独自開発する 
* モジュール構成
    * :core:modelが強依存になっている。:core:domainにまとめる。（現状modelモジュールをdomain modelと同等に扱っている）
* 読み取りバーコードの種類を追加
    * EAN13、EAN8、UPC A、UPC Eなどの商品コードのスキャンも可能にする
* スキャン結果の共有方法を変更
    * 現状バーコードをスキャンした結果もQRコードで共有している。スキャンした対象がバーコードの場合はバーコードで共有、QRの場合はQRで共有とした方が自然。


## 補足

エンジニアの経験の備忘録として当アプリを開発

個人で開発したアプリのため収益と運用（サポート、保守）が割に合わないためリリースを見送り
