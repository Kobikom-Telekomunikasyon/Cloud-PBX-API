# Cloud-PBX-API
 
API Method and data type

> URL = http://{yourip}/api/module/{response_type}/{request}/

```php
//PUT request
response_type =>
api_key       => GET
module        => GET
queueAdd      => GET
account       => POST => numeric
name          => POST => string
password      => POST => string
dynmembers    => POST => array
```


> URL = http://{yourip}/api/module/{response_type}/{request}/{account}/

```php
//DELETE request
api_key       => GET
module        => GET
queueDelete   => GET
queueAccount  => GET => numeric
```
