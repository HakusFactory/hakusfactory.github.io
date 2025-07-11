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

![create](images/create/create.png)

#### URL形式のQRコード作成

![url](images/create/url/create_url.png)

#### Wi-Fi設定情報形式のQRコード作成

![url](images/create/wifi/create_wifi.png)

#### カレンダーイベント形式のQRコード作成

![event](images/create/event/event.png)

#### 連絡先形式のQRコード作成

![contact](images/create/contact/contact.png)

#### 電話番号形式のQRコード作成

![phone](images/create/phone/phone.png)

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

#### 位置情報形式のQRコード作成

<p float="left">
    <img src="images/create/geo/permission.png" width="150"/>
    <img src="images/create/geo/input.png" width="150"/>
    <img src="images/create/geo/map.png" width="150"/>
    <img src="images/create/geo/validation.png" width="150"/>
    <img src="images/create/geo/confirm.png" width="150"/>
    <img src="images/create/geo/complete.png" width="150"/>
    <img src="images/create/geo/request_gps.png" width="150"/>
    <img src="images/create/geo/denied_permisson.png" width="150"/>
    <img src="images/create/geo/app_setting.png" width="150"/>
</p>

#### テキスト形式のQRコード作成

<p float="left">
    <img src="images/create/text/placeholder.png" width="150"/>
    <img src="images/create/text/input.png" width="150"/>
    <img src="images/create/text/confirm.png" width="150"/>
    <img src="images/create/text/complete.png" width="150"/>
</p>

### 作成済みQRコード一覧

<p float="left">
    <img src="images/created/list.png" width="150"/>
    <img src="images/created/list2.png" width="150"/>
    <img src="images/created/menu1.png" width="150"/>
    <img src="images/created/selsected.png" width="150"/>
    <img src="images/created/confirm.png" width="150"/>
    <img src="images/created/all_selected.png" width="150"/>
    <img src="images/created/empty.png" width="150"/>
</p>

### 作成済みQRコード詳細

<p float="left">
    <img src="images/created/detail/url.png" width="150"/>
    <img src="images/created/detail/wifi.png" width="150"/>
    <img src="images/created/detail/event1.png" width="150"/>
    <img src="images/created/detail/event2.png" width="150"/>
    <img src="images/created/detail/contact1.png" width="150"/>
    <img src="images/created/detail/contact2.png" width="150"/>
    <img src="images/created/detail/phone.png" width="150"/>
    <img src="images/created/detail/mail1.png" width="150"/>
    <img src="images/created/detail/mail2.png" width="150"/>
    <img src="images/created/detail/sms.png" width="150"/>
    <img src="images/created/detail/geo.png" width="150"/>
    <img src="images/created/detail/text.png" width="150"/>
    <img src="images/created/detail/share.png" width="150"/>
    <img src="images/created/detail/delete.png" width="150"/>
</p>

### スキャン

### 履歴一覧

<p float="left">
    <img src="images/history/empty.png" width="150"/>
    <img src="images/history/list1.png" width="150"/>
    <img src="images/history/list2.png" width="150"/>
    <img src="images/history/menu1.png" width="150"/>
    <img src="images/history/menu2.png" width="150"/>
    <img src="images/history/menu3.png" width="150"/>
    <img src="images/history/selected.png" width="150"/>
    <img src="images/history/delete_confirm.png" width="150"/>
    <img src="images/history/deleted.png" width="150"/>
</p>

### お気に入り一覧

<p float="left">
    <img src="images/favorite/empty.png" width="150"/>
    <img src="images/favorite/list.png" width="150"/>
    <img src="images/favorite/menu1.png" width="150"/>
    <img src="images/favorite/menu2.png" width="150"/>
    <img src="images/favorite/menu3.png" width="150"/>
    <img src="images/favorite/delete_confirm.png" width="150"/>
    <img src="images/favorite/deleted.png" width="150"/>
</p>

### 履歴詳細

#### URL

<p float="left">
    <img src="images/history/detail/url/url.png" width="150"/>
    <img src="images/history/detail/url/browser.png" width="150"/>
    <img src="images/history/detail/url/favorite.png" width="150"/>
    <img src="images/history/detail/url/share_dialog.png" width="150"/>
    <img src="images/history/detail/url/share.png" width="150"/>
    <img src="images/history/detail/url/delete_confirm.png" width="150"/>
    <img src="images/history/detail/url/deleted.png" width="150"/>
</p>

#### Wi-Fi

<p float="left">
    <img src="images/history/detail/wifi/wifi.png" width="150"/>
    <img src="images/history/detail/wifi/wifi_settings.png" width="150"/>
</p>

#### カレンダーイベント

<p float="left">
    <img src="images/history/detail/event/event1.png" width="150"/>
    <img src="images/history/detail/event/event2.png" width="150"/>
    <img src="images/history/detail/event/calender1.png" width="150"/>
    <img src="images/history/detail/event/calender2.png" width="150"/>
    <img src="images/history/detail/event/map.png" width="150"/>
</p>

#### 連絡先

<p float="left">
    <img src="images/history/detail/contact/contact1.png" width="150"/>
    <img src="images/history/detail/contact/contact2.png" width="150"/>
    <!-- <img src="images/history/detail/contact/directory1.png" width="150"/>
    <img src="images/history/detail/contact/directory2.png" width="150"/> -->
</p>

#### 電話番号

<p float="left">
    <img src="images/history/detail/phone/phone.png" width="150"/>
    <img src="images/history/detail/phone/tel.png" width="150"/>
</p>

#### メール

<p float="left">
    <img src="images/history/detail/mail/mail.png" width="150"/>
    <img src="images/history/detail/mail/share.png" width="150"/>
    <img src="images/history/detail/mail/mail_app.png" width="150"/>
</p>

#### SMS

<p float="left">
    <img src="images/history/detail/sms/sms.png" width="150"/>
    <img src="images/history/detail/sms/sms_app.png" width="150"/>
    <img src="images/history/detail/sms/tel.png" width="150"/>
</p>

#### 位置情報

<p float="left">
    <img src="images/history/detail/geo/geo.png" width="150"/>
    <img src="images/history/detail/geo/map.png" width="150"/>
</p>

#### テキスト

<p float="left">
    <img src="images/history/detail/text/text.png" width="150"/>
</p>

### お気に入り詳細

<p float="left">
    <img src="images/favorite/detail/url.png" width="150"/>
    <img src="images/favorite/detail/share_dialog.png" width="150"/>
    <img src="images/favorite/detail/share.png" width="150"/>
    <img src="images/favorite/detail/confirm_delete.png" width="150"/>
    <img src="images/favorite/detail/deleted.png" width="150"/>
    <img src="images/favorite/detail/confirm_favorite_cancel.png" width="150"/>
    <img src="images/favorite/detail/canceled_favorite.png" width="150"/>
</p>

### 検索一覧

<p float="left">
    <img src="images/search/empty.png" width="150"/>
    <img src="images/search/list.png" width="150"/>
    <img src="images/search/keyword1.png" width="150"/>
    <img src="images/search/keyword2.png" width="150"/>
    <img src="images/search/not_found.png" width="150"/>
    <img src="images/search/sort_modal.png" width="150"/>
    <img src="images/search/sort_old.png" width="150"/>
    <img src="images/search/sort_favorite.png" width="150"/>
    <img src="images/search/menu1.png" width="150"/>
    <img src="images/search/menu2.png" width="150"/>
    <img src="images/search/delete_confirm.png" width="150"/>
    <img src="images/search/deleted.png" width="150"/>
</p>

### 検索結果詳細

<p float="left">
    <img src="images/search/detail/history.png" width="150"/>
    <img src="images/search/detail/favorite.png" width="150"/>
</p>

### 設定

<p float="left">
    <img src="images/settings/lightmode.png" width="150"/>
    <img src="images/settings/dynamic.png" width="150"/>
    <img src="images/settings/dark.png" width="150"/>
    <img src="images/settings/scan_setting1.png" width="150"/>
    <img src="images/settings/scan_setting2.png" width="150"/>
    <img src="images/settings/license.png" width="150"/>
</p>
