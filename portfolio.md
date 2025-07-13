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

![splash](images/splash.png)

### 利用規約同意画面

![agree_terms](images/term.png)

### ホーム

![home](images/home.png)

### QR作成種類選択

![choose_create](images/create/list.png)

#### URL形式のQRコード作成

![url_qr](images/create/url.png)

#### Wi-Fi設定情報形式のQRコード作成

![wifi_qr](images/create/wifi.png)

#### カレンダーイベント形式のQRコード作成

![event_qr](images/create/event.png)

#### 連絡先形式のQRコード作成

![contact_qr](images/create/contact.png)

#### 電話番号形式のQRコード作成

![phone_qr](images/create/phone.png)

#### メール形式のQRコード作成

![mail_qr](images/create/mail.png)

#### SMS形式のQRコード作成

![sms_qr](images/create/sms.png)

#### 位置情報形式のQRコード作成

![geo_qr](images/create/geo.png)

#### テキスト形式のQRコード作成

![text_qr](images/create/text.png)

### 作成済みQRコード一覧

![created_qr](images/created/list.png)

### 作成済みQRコード詳細

![qr_detail](images/created/detail.png)

### 履歴一覧

![history_list](images/history/list.png)

### お気に入り一覧

![favorite_list](images/favorite/list.png)

### 履歴詳細

#### URL

![url_history](images/history/url.png)

#### Wi-Fi

![wifi_history](images/history/wifi.png)

#### カレンダーイベント

![event_history](images/history/event.png)

#### 連絡先

![contact_history](images/history/contact.png)

#### 電話番号

![phone_history](images/history/phone.png)

#### メール

![mail_history](images/history/mail.png)

#### SMS

![sms_history](images/history/sms.png)

#### 位置情報

![geo_history](images/history/geo.png)

#### テキスト

![text_history](images/history/text.png)

### お気に入り詳細

![favorite_detail](images/favorite/detail.png)

### 検索一覧

![search](images/search.png)

### 設定

#### ダイナミックカラー

| 設定 | ホーム | 備考 |
|-----|-----|-----|
|<img src="images/settings/dynamic/setting_off.png" width="150"/>|<img src="images/settings/dynamic/home_off.png" width="150"/>|OFF<br>OS12〜|
|<img src="images/settings/dynamic/setting_on.png" width="150"/>|<img src="images/settings/dynamic/home_on.png" width="150"/>|ON<br>OS12〜|
|<img src="images/settings/dynamic/OS11.png" width="150"/>|-|〜OS11|

#### ダークモード

![darkmode](images/settings/dark.png)

#### 履歴の保存

![history_setting](images/settings/history.png)

#### スキャン設定

![scan_setting](images/settings/scan.png)

#### 利用規約

![term](images/settings/term.png)

#### プライバシーポリシー

![policy](images/settings/policy.png)

#### ライセンス

![license](images/settings/license.png)
