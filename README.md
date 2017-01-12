# Cloud-PBX-API
 
### Kuyruk ve agent'lar için GET/PUT/DELETE method ve data type
Kampanyalar için kuyruk oluşturma ve kuyruk içerisine dinamik agent atamak, kuyruk içerisindeki agent'ları silmek veya kuyruk içerisindeki agent'ların listesini görüntülemek için hazırlanmıştır.
Genel kullanıma yöneliktir.
Soru ve önerilerinizi iletiniz ; yazilim@kobikom.com.tr

| Parametre     | Açıklama               | Type   |
| ------------- |:----------------------:| ------:|
| account       | Kuyruk numarası        | numeric|
| name          | Kuyruk adı             | string |
| password      | Kuyruk şifreniz        | string |
| dynmembers    | Dinamik agent'larınız  | array  |


#### Kuyruk ekle

> URL = http://{yourpbxip}/api/module/addQueue/

```php
//PUT request - module=addQueue

api_key       => GET
module        => GET
account       => POST => numeric
name          => POST => string
password      => POST => string
dynmembers    => POST => array
```

#### Kuyruk sil

> URL = http://{yourpbxip}/api/module/deleteQueue/{queue}/

```php
//DELETE request - module=deleteQueue

api_key       => GET
module        => GET
account       => GET => numeric
```
#### Kuyruğa tanımlı dinamik agent listesi

> URL = http://{yourpbxip}/api/module/queueAgents/{queue}/

```php
//GET request - queueAgents

api_key       => GET
module        => GET
account       => GET
queue         => GET => Tek kuyruga sorgu yapabilir
```

#### Kuyruğa agent eklemek veya silmek

> URL = http://{yourpbxip}/api/module/agentsQueue/

```php
//GET request - agentsQueue

api_key       => GET
module        => GET
account       => POST => numeric
dynmembers    => POST => array
make          => POST => bolean => true > gönderilen agent ları ekler / false > gönderilen agent ları siler
```


Başarılar...
