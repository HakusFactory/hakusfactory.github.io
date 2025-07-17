# :feature:home module

```mermaid
flowchart TD
home[:feature:home]

home --> common
home --> designsystem
home --> domain
home --> utils

common[:core:common]

designsystem[:core:designsystem]
designsystem --> utils

domain[:core:domain]

utils[:utils]
```