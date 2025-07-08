# コードリーダー

## 概要
QR、バーコードのスキャン機能を備えたAndroidアプリ。
Google Play Storeに同様のアプリが多数存在するが、モダンなUIや技術を取り入れているものはそう多くないと感じた。
そこで自らの経験をもとにモダンな印象を与えるアプリを制作。

## 言語、FW、ライブラリ
* Kotlin
* Jetpack Compose
* Android SDK
* Flow
* StateFlow
* Coroutines
* Hilt
* Jetpack Navigation Component
* Adaptive Navigation Suite
* DataStore
* Room
* Google Code Scanner
* MlKit
* Zixing
* Chrome Custom Tabs
* jsoup
* Tink
* Coil
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

## 機能
* QRコード、バーコードのスキャン
* スキャンデータの解析
* スキャンデータの詳細表示
* スキャンデータの保存（履歴、お気に入り）
* スキャンデータの削除
* 保存したスキャンデータの検索
* スキャンデータの共有
* スキャンデータ（URL）のブラウザ表示
* スキャンデータ（SMS）のSMSアプリ連携
* スキャンデータ（メール）のメールアプリ連携
* スキャンデータ（電話番号）の電話アプリ連携
* スキャンデータ（位置情報）のGoogle Mapアプリ連携
* スキャンデータ（カレンダーイベント）のカレンダーアプリ連携
* スキャンデータ（連絡先）の電話帳アプリ連携
* QRコードの作成
* 作成したQRコードの詳細表示
* 作成したQRコードの保存
* 作成したQRコードの削除
* 作成したQRコードの共有
* アプリのテーマの切り替え（ダークモード、ダイナミックカラー）
* コードスキャンのオプション設定（QR CODE、AZTEC、CODE128、CODE39、CODEBAR等）
* その他（利用規約、プライバシーポリシー、ライセンス）

## 画面
### ホーム

### QRコードをつくる

URL、Wi-Fi設定、カレンダーイベント、連絡先、電話番号、メール、SMS、位置情報、テキスト、それぞれの形式のQRコードを作成する

<img src="https://github.com/user-attachments/assets/034eb43c-299a-46c8-98b5-2fbbd0d97c09" width="30%"> <img src="https://github.com/user-attachments/assets/0db7e37c-c1c2-4412-afb4-5f8cf5db2c63" width="30%">

#### URL形式のQRコード作成

| 入力 | バリデーション | ブラウザ確認 | 作成前確認 | 作成完了 | QR共有 | URLコピー |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| <img src="https://github.com/user-attachments/assets/c9f37532-852a-477a-b126-0ee97f16baf8"> | <img src="https://github.com/user-attachments/assets/d400f49d-5d6c-4900-b231-e2d250d55158"> | <img src="https://github.com/user-attachments/assets/099271ad-3407-4f4e-b179-9b688afb7bc2"> | <img src="https://github.com/user-attachments/assets/be9ed197-f2d3-4813-ab1e-78dfe432fe99"> | <img src="https://github.com/user-attachments/assets/0413e149-4509-4ae2-b05c-7a138b8866ff"> | <img src="https://github.com/user-attachments/assets/2c8d52b8-4532-4fa1-a021-666a487e1446"> | <img src="https://github.com/user-attachments/assets/5798f457-bdcf-40c0-8c01-c19e6cb80775"> |

#### Wi-Fi設定情報形式のQRコード作成

| プレースホルダー | 入力 | プルダウン | 作成前確認 | 作成完了 |
| ---- | ---- | ---- | ---- | ---- |
| ![placeholder](images/create/wifi/placeholder.png) | ![input](images/create/wifi/input.png) | ![pulldown](images/create/wifi/pulldown.png) | ![confirm](images/create/wifi/confirm.png) | ![complete](images/create/wifi/complete.png) |

### 作成済みQRコード一覧

### 作成済みQRコード詳細

### スキャン

### 履歴/お気に入り一覧

### 履歴/お気に入り詳細

### 検索一覧

### 検索結果詳細

### 絞り込み

### 設定

| ライトモード | ダイナミックテーマ | ダークモード |
| ---- | ---- | ---- |
| ![lightmode](images/settings/lightmode.png)| ![dynamic](images/settings/dynamic.png) | ![dark](images/settings/dark.png) |










### スキャン設定


### 利用規約/プライバシーポリシー

### ライセンス















