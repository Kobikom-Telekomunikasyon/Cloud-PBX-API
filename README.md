# Cloud-PBX-API
 
### Kuyruk ve agent'lar için GET/PUT/DELETE method ve data type
Kampanyalar için kuyruk oluşturma ve kuyruk içerisine dinamik agent atamak, kuyruk içerisindeki agent'ları silmek veya kuyruk içerisindeki agent'ların listesini görüntülemek için hazırlanmıştır.
Genel kullanıma yöneliktir.

| Parametre     | Açıklama               | Type   |
| ------------- |:----------------------:| ------:|
| account       | Kuyruk numarası        | numeric|
| name          | Kuyruk adı             | string |
| password      | Kuyruk şifreniz        | string |
| dynmembers    | Dinamik agent'larınız  | array  |


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
account       => GET => numeric
```
#### Kuyruğa tanımlı dinamik agent listesi

> URL = http://{yourpbxip}/api/module/{response_type}/{queueAgents}/

```php
//GET request - queueAgents

responseType  => GET : xml/json
api_key       => GET
module        => GET
account       => GET
```

#### Kuyruğa agent eklemek veya silmek

> URL = http://{yourpbxip}/api/module/{response_type}/{queueUsers}/

```php
//GET request - queueUsers

responseType  => GET : xml/json
api_key       => GET
module        => GET
account       => POST => numeric
dynmembers    => POST => array
make          => POST => bolean => true gönderilen agent ları ekler / false gönderilen agent ları siler
```


Başarılar...
