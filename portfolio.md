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

<p float="left">
    <img src="images/create/url/placeholder.png" width="150"/>
    <img src="images/create/url/input.png" width="150"/>
    <img src="images/create/url/validation.png" width="150"/>
    <img src="images/create/url/confirm.png" width="150"/>
    <img src="images/create/url/complete.png" width="150"/>
    <img src="images/create/url/browse_confirm.png" width="150"/>
    <img src="images/create/url/share_qr.png" width="150"/>
    <img src="images/create/url/copy.png" width="150"/>
</p>

#### Wi-Fi設定情報形式のQRコード作成

<p float="left">
    <img src="images/create/wifi/placeholder.png" width="150"/>
    <img src="images/create/wifi/input.png" width="150"/>
    <img src="images/create/wifi/pulldown.png" width="150"/>
    <img src="images/create/wifi/confirm.png" width="150"/>
    <img src="images/create/wifi/complete.png" width="150"/>
</p>

#### カレンダーイベント形式のQRコード作成

<p float="left">
    <img src="images/create/event/placeholder1.png" width="150"/>
    <img src="images/create/event/placeholder2.png" width="150"/>
    <img src="images/create/event/datepicker.png" width="150"/>
    <img src="images/create/event/timepicker.png" width="150"/>
    <img src="images/create/event/input1.png" width="150"/>
    <img src="images/create/event/input2.png" width="150"/>
    <img src="images/create/event/input3.png" width="150"/>
    <img src="images/create/event/input4.png" width="150"/>
    <img src="images/create/event/map.png" width="150"/>
    <img src="images/create/event/validation.png" width="150"/>
    <img src="images/create/event/confirm.png" width="150"/>
    <img src="images/create/event/complate1.png" width="150"/>
    <img src="images/create/event/complete2.png" width="150"/>
</p>

#### 連絡先形式のQRコード作成

<p float="left">
    <img src="images/create/contact/placeholder1.png" width="150"/>
    <img src="images/create/contact/placeholder2.png" width="150"/>
    <img src="images/create/contact/add_phone.png" width="150"/>
    <img src="images/create/contact/add_mail.png" width="150"/>
    <img src="images/create/contact/phone_label_dialog.png" width="150"/>
    <img src="images/create/contact/input1.png" width="150"/>
    <img src="images/create/contact/mail_label_dialog.png" width="150"/>
    <img src="images/create/contact/input2.png" width="150"/>
    <img src="images/create/contact/input3.png" width="150"/>
    <img src="images/create/contact/input4.png" width="150"/>
    <img src="images/create/contact/validation.png" width="150"/>
    <img src="images/create/contact/confirm.png" width="150"/>
    <img src="images/create/contact/conmlete1.png" width="150"/>
    <img src="images/create/contact/complete2.png" width="150"/>
</p>

#### 電話番号形式のQRコード作成

<p float="left">
    <img src="images/create/phone/placeholder.png" width="150"/>
    <img src="images/create/phone/input.png" width="150"/>
    <img src="images/create/phone/validation.png" width="150"/>
    <img src="images/create/phone/confirm.png" width="150"/>
    <img src="images/create/phone/complete.png" width="150"/>
</p>

#### メール形式のQRコード作成

<p float="left">
    <img src="images/create/mail/placeholder.png" width="150"/>
    <img src="images/create/mail/input1.png" width="150"/>
    <img src="images/create/mail/validation.png" width="150"/>
    <img src="images/create/mail/input2.png" width="150"/>
    <img src="images/create/mail/confirm.png" width="150"/>
    <img src="images/create/mail/complete1.png" width="150"/>
    <img src="images/create/mail/complete2.png" width="150"/>
</p>

#### SMS形式のQRコード作成

<p float="left">
    <img src="images/create/sms/placeholder.png" width="150"/>
    <img src="images/create/sms/input.png" width="150"/>
    <img src="images/create/sms/validation.png" width="150"/>
    <img src="images/create/sms/confirm.png" width="150"/>
    <img src="images/create/sms/complete.png" width="150"/>
</p>

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















