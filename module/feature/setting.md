# :feature:setting module

```mermaid
flowchart TD
setting[:feature:setting]

setting --> common
setting --> designsystem
setting --> domain
setting --> utils

common[:core:common]

designsystem[:core:designsystem]
designsystem --> utils

domain[:core:domain]

utils[:utils]
```

## 役割

設定画面関連のロジックを配置

* Navigation関連のロジックを配置
* 画面UI関連のロジックを配置
* ViewModelを配置