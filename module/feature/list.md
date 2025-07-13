# :feature:list module

```mermaid
flowchart TD
list[:feature:list]
list --> search
list --> datastore
list --> designsystem
list --> domain
list --> model
list --> utils

search[:feature:search]
search --> datastore
search --> model

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