# Cloud-PBX-API
 
### Queue ve Agents GET/PUT/DELETE method ve data type


#### Kuyruk ekle

> URL = http://{yourpbxip}/api/module/{responseType}/{addQueue}/

```php
//PUT request - addQueue

responseType  => GET : xml/json
api_key       => GET
module        => GET
queueAdd      => GET
account       => POST => numeric
name          => POST => string
password      => POST => string
dynmembers    => POST => array
```

#### Kuyruk sil

> URL = http://{yourpbxip}/api/module/{responseType}/{request}/{deleteQueue}/

```php
//DELETE request - deleteQueue

responseType  => GET : xml/json
api_key       => GET
module        => GET
queueDelete   => GET
queueAccount  => GET => numeric
```
#### Kuyruğa tanımlı dinamik agent listesi

> URL = http://{yourpbxip}/api/module/{response_type}/{queueAgents}/

```php
//GET request - queueAgents

responseType  => GET : xml/json
api_key       => GET
module        => GET
queueAccount  => GET
```

Başarılar...
