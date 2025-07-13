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

### スプラッシュ

### 利用規約同意画面

![term](images/term/term.png)

### ホーム

![home](images/home/home.png)

### QR作成種類選択

![create](images/create/list.png)

#### URL形式のQRコード作成

![url](images/create/url.png)

#### Wi-Fi設定情報形式のQRコード作成

![url](images/create/wifi.png)

#### カレンダーイベント形式のQRコード作成

![event](images/create/event.png)

#### 連絡先形式のQRコード作成

![contact](images/create/contact.png)

#### 電話番号形式のQRコード作成

![phone](images/create/phone.png)

#### メール形式のQRコード作成

![mail](images/create/mail.png)

#### SMS形式のQRコード作成

![sms](images/create/sms.png)

#### 位置情報形式のQRコード作成

![geo](images/create/geo.png)

#### テキスト形式のQRコード作成

![text](images/create/text.png)

### 作成済みQRコード一覧

![list](images/created/list.png)

### 作成済みQRコード詳細

![detail](images/created/detail.png)

### 履歴一覧

![list](images/history/list.png)

### お気に入り一覧

![list](images/favorite/list.png)

### 履歴詳細

#### URL

![url](images/history/url.png)

#### Wi-Fi

![wifi](images/history/wifi.png)

#### カレンダーイベント

![event](images/history/event.png)

#### 連絡先

![contact](images/history/contact.png)

#### 電話番号

![phone](images/history/phone.png)

#### メール

![mail](images/history/mail.png)

#### SMS

![sms](images/history/sms.png)

#### 位置情報

![geo](images/history/geo.png)

#### テキスト

![text](images/history/text.png)

### お気に入り詳細

![detail](images/favorite/detail.png)

### 検索一覧

![list](images/search/list.png)

### 設定

#### ダイナミックカラー

| 設定 | ホーム | 備考 |
|-----|-----|-----|
|<img src="images/settings/dynamic/setting_off.png" width="150"/>|<img src="images/settings/dynamic/home_off.png" width="150"/>|OFF<br>OS12〜|
|<img src="images/settings/dynamic/setting_on.png" width="150"/>|<img src="images/settings/dynamic/home_on.png" width="150"/>|ON<br>OS12〜|
|<img src="images/settings/dynamic/OS11.png" width="150"/>|-|〜OS11|

#### ダークモード

![dark](images/settings/dark.png)

#### 履歴の保存

![history](images/settings/history.png)

#### スキャン設定

![scan](images/settings/scan.png)

#### 利用規約

![term](images/settings/term.png)

#### プライバシーポリシー

![policy](images/settings/policy.png)

#### ライセンス

![license](images/settings/license.png)
