# :feature:search module

```mermaid
flowchart TD
search[:feature:search]

search --> common
search --> designsystem
search --> domain
search --> utils

common[:core:common]

designsystem[:core:designsystem]
designsystem --> utils

domain[:core:domain]

utils[:utils]
```
