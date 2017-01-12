# Cloud-PBX-API
 
### Queue ve Agents GET/PUT/DELETE method ve data type

> URL = http://{yourpbxip}/api/module/{responseType}/{addQueue}/

> Gönderilecek parametreler
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


> URL = http://{yourpbxip}/api/module/{responseType}/{request}/{deleteQueue}/

> Gönderilecek parametreler
```php
//DELETE request - deleteQueue

responseType  => GET : xml/json
api_key       => GET
module        => GET
queueDelete   => GET
queueAccount  => GET => numeric
```

> URL = http://{yourpbxip}/api/module/{response_type}/{queueAgents}/

> Gönderilecek parametreler
```php
//GET request - queueAgents

responseType  => GET : xml/json
api_key       => GET
module        => GET
queueAccount  => GET
```

Başarılar...
