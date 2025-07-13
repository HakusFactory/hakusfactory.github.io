# :feature:search module

```mermaid
flowchart TD
search[:feature:search]

search --> datastore
search --> designsystem
search --> domain
search --> model
search --> utils

designsystem[:core:designsystem]
designsystem --> utils

domain[:core:domain]
domain --> common
domain --> model
domain --> data
domain --> utils

model[:core:model]
model --> utils

data[:core:data]
data --> common
data --> database
data --> model
data --> utils

datastore[:core:datastore]
datastore --> model

utils[:utils]
database[:core:database]
common[:core:common]
```
