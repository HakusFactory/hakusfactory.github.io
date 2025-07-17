# :feature:list module

```mermaid
flowchart TD
list[:feature:list]

list --> common
list --> designsystem
list --> domain
list --> utils

common[:core:common]

designsystem[:core:designsystem]
designsystem --> utils

domain[:core:domain]

utils[:utils]
```

## 役割

履歴一覧画面、履歴詳細画面、お気に入り一覧画面、お気に入り詳細画面関連のロジックを配置

* Navigation関連のロジックを配置
* 画面UI関連のロジックを配置
* ViewModelを配置