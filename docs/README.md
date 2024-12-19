
[](#api-ux-ntlc-contract-account-overview-v2)

# ➤ API UX NTLC Contract Account Overview V2
Version v3.0.0


[](#-indice)

## ➤ 📖 Indice

[](#table-of-contents)

## ➤ Table of Contents

* [➤ API UX NTLC Contract Account Overview V2](#-api-ux-ntlc-contract-account-overview-v2)
	* [➤ 📖 Indice](#--indice)
	* [➤ Decripcion General](#-decripcion-general)
		* [Documentación Extendida](#documentacin-extendida)
		* [Base URLs:](#base-urls)
	* [➤ Endpoints](#-endpoints)
	* [➤ listCompanies](#-listcompanies)
* [➤ You can also use wget](#-you-can-also-use-wget)
		* [Acerca de la funcionalidad expuesta ](#acerca-de-la-funcionalidad-expuesta-)
		* [Data de Prueba](#data-de-prueba)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api)
		* [Path Parameters](#path-parameters)
		* [Variantes válidas del Payload (Cuerpo del mesaje)](#variantes-vlidas-del-payload-cuerpo-del-mesaje)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters)
		* [Variantes validas del Payload (Cuerpo del mensaje)](#variantes-validas-del-payload-cuerpo-del-mensaje)
		* [Lista de Valores usadas en esta versión de la API](#lista-de-valores-usadas-en-esta-versin-de-la-api)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api)
	* [➤ listCompanyAccounts](#-listcompanyaccounts)
* [➤ You can also use wget](#-you-can-also-use-wget-1)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta)
		* [Data de Prueba](#data-de-prueba-1)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-1)
		* [Path Parameters](#path-parameters-1)
		* [Variantes válidas del Payload (Cuerpo del mesaje)](#variantes-vlidas-del-payload-cuerpo-del-mesaje-1)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-1)
		* [Variantes validas del Payload (Cuerpo del mensaje)](#variantes-validas-del-payload-cuerpo-del-mensaje-1)
		* [Lista de Valores usadas en esta versión de la API](#lista-de-valores-usadas-en-esta-versin-de-la-api-1)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api-1)
	* [➤ listAccounts](#-listaccounts)
* [➤ You can also use wget](#-you-can-also-use-wget-2)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta-1)
		* [Data de Prueba](#data-de-prueba-2)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-2)
		* [Path Parameters](#path-parameters-2)
		* [Variantes válidas del Payload (Cuerpo del mesaje)](#variantes-vlidas-del-payload-cuerpo-del-mesaje-2)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-2)
		* [Variantes validas del Payload (Cuerpo del mensaje)](#variantes-validas-del-payload-cuerpo-del-mensaje-2)
		* [Lista de Valores usadas en esta versión de la API](#lista-de-valores-usadas-en-esta-versin-de-la-api-2)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api-2)
	* [➤ addFileOrder](#-addfileorder)
* [➤ You can also use wget](#-you-can-also-use-wget-3)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta-2)
		* [Data de Prueba](#data-de-prueba-3)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-3)
		* [Path Parameters](#path-parameters-3)
		* [Variantes válidas del Payload (Cuerpo del mesaje)](#variantes-vlidas-del-payload-cuerpo-del-mesaje-3)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-3)
		* [Variantes validas del Payload (Cuerpo del mensaje)](#variantes-validas-del-payload-cuerpo-del-mensaje-3)
		* [Lista de Valores usadas en esta versión de la API](#lista-de-valores-usadas-en-esta-versin-de-la-api-3)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api-3)
* [➤ Schemas](#-schemas)
		* [Properties](#properties)
		* [Properties](#properties-1)
		* [Properties](#properties-2)
		* [Properties](#properties-3)
		* [Properties](#properties-4)
		* [Properties](#properties-5)
		* [Properties](#properties-6)
		* [Properties](#properties-7)
		* [Properties](#properties-8)
		* [Properties](#properties-9)
		* [Properties](#properties-10)
	* [➤ Autenticacion](#-autenticacion)
	* [➤ Documentación de Arquitectura](#-documentacin-de-arquitectura)
	* [➤ Portal de APIs](#-portal-de-apis)
	* [➤ Diagramas de arquitectura](#-diagramas-de-arquitectura)
	* [➤ Deuda tecnica](#-deuda-tecnica)


[](#decripcion-general)

## ➤ Decripcion General
Esta API permite solicitar la generacion de los archivos de exportacion de las cuentas, de todas las empresas de un contrato, en Saldos y Movimientos, OB.

### Documentación Extendida

<a href="https://confluence.com.pe/pages/viewpage.action?pageId=554759484">Para más información.</a>

### Base URLs:

* <a href="/channel/ntlc/v2">/channel/ntlc/v2</a>



[](#endpoints)

## ➤ Endpoints

|Nro|TAG|HTTP Operation|Endpoint|Description|
|---|---|---|---|---|
|1|Company|GET|/companies|Obtiene la lista de empresas de un contrato.|
|2|Company|GET|/company-accounts|Obtiene una lista de compañias con sus cuentas.|
|3|Account|GET|/accounts|Obtiene una lista de cuentas de una compañia.|
|4|File order|POST|/file-orders/company-accounts|Crea una solicitud para generar un archivo con el listado de cuentas de las compañias seleccionas.|


<h1 id="api-ux-ntlc-contract-account-overview-v2-company">Company</h1>


[](#listcompanies)

## ➤ listCompanies

<a id="opIdlistCompanies"></a>

> Code samples

```shell

[](#you-can-also-use-wget)

# ➤ You can also use wget
curl -X GET /channel/ntlc/v2/companies \
  -H 'Accept: application/json' \
  -H 'Authorization: Bearer 363536363jjxnj63633611' \
  -H 'Request-ID: 550e8400-e29b-41d4-a716-446655440000' \
  -H 'X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000'

```

```http
GET /channel/ntlc/v2/companies HTTP/1.1

Accept: application/json
Authorization: Bearer 363536363jjxnj63633611
Request-ID: 550e8400-e29b-41d4-a716-446655440000
X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000

```

```javascript

const headers = {
  'Accept':'application/json',
  'Authorization':'Bearer 363536363jjxnj63633611',
  'Request-ID':'550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN':'550e8400-e29b-41d4-a716-446655440000'
};

fetch('/channel/ntlc/v2/companies',
{
  method: 'GET',

  headers: headers
})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});

```

```ruby
require 'rest-client'
require 'json'

headers = {
  'Accept' => 'application/json',
  'Authorization' => 'Bearer 363536363jjxnj63633611',
  'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000'
}

result = RestClient.get '/channel/ntlc/v2/companies',
  params: {
  }, headers: headers

p JSON.parse(result)

```

```python
import requests
headers = {
  'Accept': 'application/json',
  'Authorization': 'Bearer 363536363jjxnj63633611',
  'Request-ID': '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN': '550e8400-e29b-41d4-a716-446655440000'
}

r = requests.get('/channel/ntlc/v2/companies', headers = headers)

print(r.json())

```

```php
<?php

require 'vendor/autoload.php';

$headers = array(
    'Accept' => 'application/json',
    'Authorization' => 'Bearer 363536363jjxnj63633611',
    'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
    'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000',
);

$client = new \GuzzleHttp\Client();

// Define array of request body.
$request_body = array();

try {
    $response = $client->request('GET','/channel/ntlc/v2/companies', array(
        'headers' => $headers,
        'json' => $request_body,
       )
    );
    print_r($response->getBody()->getContents());
 }
 catch (\GuzzleHttp\Exception\BadResponseException $e) {
    // handle exception or api errors.
    print_r($e->getMessage());
 }

 // ...

```

```java
URL obj = new URL("/channel/ntlc/v2/companies");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());

```

```go
package main

import (
       "bytes"
       "net/http"
)

func main() {

    headers := map[string][]string{
        "Accept": []string{"application/json"},
        "Authorization": []string{"Bearer 363536363jjxnj63633611"},
        "Request-ID": []string{"550e8400-e29b-41d4-a716-446655440000"},
        "X-AUTH-TOKEN": []string{"550e8400-e29b-41d4-a716-446655440000"},
    }

    data := bytes.NewBuffer([]byte{jsonReq})
    req, err := http.NewRequest("GET", "/channel/ntlc/v2/companies", data)
    req.Header = headers

    client := &http.Client{}
    resp, err := client.Do(req)
    // ...
}

```

`GET /companies`

*Obtiene la lista de empresas de un contrato.*

### Acerca de la funcionalidad expuesta 

El servicio brinda la lista con la información de las empresas que puede ver un usuario.

### Data de Prueba
No aplica.

### Precondiciones para el consumo de esta versión de la API
No aplica.

### Path Parameters
No aplica.

### Variantes válidas del Payload (Cuerpo del mesaje)
No aplica.

### Usos válidos de Query Parameters
No aplica.

### Variantes validas del Payload (Cuerpo del mensaje)
No aplica.

### Lista de Valores usadas en esta versión de la API
No aplica.

### Códigos de error usados en esta versión de la API

| Código | HTTP Status | Descripción |
|--------|-------------|-------------|
| TL0002 | 409 | Ocurrió un error al validar las reglas de negocio. |
| TL0003 | 400 | Los datos proporcionados no son validos. |
| TL0004 | 500 | Ocurrió un error interno en el servicio. |
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos.
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion. |

<h3 id="listcompanies-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token de Authorización|
|Request-ID|header|string|true|Este campo es un valor estandar ya existente y sera usado como identificador.|
|X-AUTH-TOKEN|header|string|true|Identificador de sesion de usuario.|

> Example responses

> 200 Response

```json
[
  {
    "documentValue": "20461896344",
    "documentType": "1",
    "description": "121321",
    "isPrincipal": true,
    "accountsQuantity": 12,
    "creditCardsQuantity": 4
  }
]
```

> 400 Response

```json
{
  "code": "TL0003",
  "description": "Los datos proporcionados no son validos.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0003",
      "component": "Channel Contract Account Overview",
      "description": "Los datos proporcionados no son validos."
    }
  ]
}
```

> 401 Response

```json
{
  "code": "TL0011",
  "description": "No esta autorizado correctamente para ejecutar esta operación.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0011",
      "component": "Channel Contract Account Overview",
      "description": "No esta autorizado correctamente para ejecutar esta operación."
    }
  ]
}
```

> 409 Response

```json
{
  "code": "TL0002",
  "description": "Ocurrió un error al validar las reglas de negocio.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0002",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error al validar las reglas de negocio."
    }
  ]
}
```

> 500 Response

```json
{
  "code": "TL0004",
  "description": "Ocurrió un error interno en el servicio.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0004",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error interno en el servicio."
    }
  ]
}
```

> 503 Response

```json
{
  "code": "TL0009",
  "description": "Ocurrio un error intentando invocar servicios externos.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0009",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrio un error intentando invocar servicios externos."
    }
  ]
}
```

<h3 id="listcompanies-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se obtuvo la lista de compañias correctamente.|Inline|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|La operación no devolvió una respuesta.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|Los datos proporcionados no son validos.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|No esta autorizado correctamente para ejecutar esta operación.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Ocurrió un error al validar las reglas de negocio.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Ocurrió un error interno en el servicio.|[ApiException](#schemaapiexception)|
|503|[Service Unavailable](https://tools.ietf.org/html/rfc7231#section-6.6.4)|Ocurrio un error intentando invocar servicios externos.|[ApiException](#schemaapiexception)|

<h3 id="listcompanies-responseschema">Response Schema</h3>

Status Code **200**

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[[CompanyListResponse](#schemacompanylistresponse)]|false|none|none|
|» documentValue|string|false|none|Valor del documento|
|» documentType|string|false|none|Tipo de documento|
|» description|string|false|none|Nombre de empresa o raz&oacute;n social|
|» isPrincipal|boolean|false|none|Identificador de empresa principal|
|» accountsQuantity|integer(int32)|false|none|Numero de cuentas de la empresa|
|» creditCardsQuantity|integer(int32)|false|none|Numero de tarjetas de credito de la empresa|

<aside class="success">
This operation does not require authentication
</aside>


[](#listcompanyaccounts)

## ➤ listCompanyAccounts

<a id="opIdlistCompanyAccounts"></a>

> Code samples

```shell

[](#you-can-also-use-wget)

# ➤ You can also use wget
curl -X GET /channel/ntlc/v2/company-accounts \
  -H 'Accept: application/json' \
  -H 'Authorization: Bearer 363536363jjxnj63633611' \
  -H 'Request-ID: 550e8400-e29b-41d4-a716-446655440000' \
  -H 'X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000'

```

```http
GET /channel/ntlc/v2/company-accounts HTTP/1.1

Accept: application/json
Authorization: Bearer 363536363jjxnj63633611
Request-ID: 550e8400-e29b-41d4-a716-446655440000
X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000

```

```javascript

const headers = {
  'Accept':'application/json',
  'Authorization':'Bearer 363536363jjxnj63633611',
  'Request-ID':'550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN':'550e8400-e29b-41d4-a716-446655440000'
};

fetch('/channel/ntlc/v2/company-accounts',
{
  method: 'GET',

  headers: headers
})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});

```

```ruby
require 'rest-client'
require 'json'

headers = {
  'Accept' => 'application/json',
  'Authorization' => 'Bearer 363536363jjxnj63633611',
  'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000'
}

result = RestClient.get '/channel/ntlc/v2/company-accounts',
  params: {
  }, headers: headers

p JSON.parse(result)

```

```python
import requests
headers = {
  'Accept': 'application/json',
  'Authorization': 'Bearer 363536363jjxnj63633611',
  'Request-ID': '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN': '550e8400-e29b-41d4-a716-446655440000'
}

r = requests.get('/channel/ntlc/v2/company-accounts', headers = headers)

print(r.json())

```

```php
<?php

require 'vendor/autoload.php';

$headers = array(
    'Accept' => 'application/json',
    'Authorization' => 'Bearer 363536363jjxnj63633611',
    'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
    'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000',
);

$client = new \GuzzleHttp\Client();

// Define array of request body.
$request_body = array();

try {
    $response = $client->request('GET','/channel/ntlc/v2/company-accounts', array(
        'headers' => $headers,
        'json' => $request_body,
       )
    );
    print_r($response->getBody()->getContents());
 }
 catch (\GuzzleHttp\Exception\BadResponseException $e) {
    // handle exception or api errors.
    print_r($e->getMessage());
 }

 // ...

```

```java
URL obj = new URL("/channel/ntlc/v2/company-accounts");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());

```

```go
package main

import (
       "bytes"
       "net/http"
)

func main() {

    headers := map[string][]string{
        "Accept": []string{"application/json"},
        "Authorization": []string{"Bearer 363536363jjxnj63633611"},
        "Request-ID": []string{"550e8400-e29b-41d4-a716-446655440000"},
        "X-AUTH-TOKEN": []string{"550e8400-e29b-41d4-a716-446655440000"},
    }

    data := bytes.NewBuffer([]byte{jsonReq})
    req, err := http.NewRequest("GET", "/channel/ntlc/v2/company-accounts", data)
    req.Header = headers

    client := &http.Client{}
    resp, err := client.Do(req)
    // ...
}

```

`GET /company-accounts`

*Obtiene una lista de compañias con sus cuentas.*

### Acerca de la funcionalidad expuesta

El servicio brinda las cuentas de las compañias seleccionadas para realizar la impresion.

### Data de Prueba
No aplica.

### Precondiciones para el consumo de esta versión de la API
No aplica.

### Path Parameters
No aplica.

### Variantes válidas del Payload (Cuerpo del mesaje)
No aplica.

### Usos válidos de Query Parameters
No aplica.

### Variantes validas del Payload (Cuerpo del mensaje)
No aplica.

### Lista de Valores usadas en esta versión de la API
No aplica.

### Códigos de error usados en esta versión de la API

| Código | HTTP Status | Descripción |
|--------|-------------|-------------|
| TL0002 | 409 | Ocurrió un error al validar las reglas de negocio. |
| TL0003 | 400 | Los datos proporcionados no son validos. |
| TL0004 | 500 | Ocurrió un error interno en el servicio. |
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos.
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion. |

<h3 id="listcompanyaccounts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token de Authorización|
|Request-ID|header|string|true|Este campo es un valor estandar ya existente y sera usado como identificador.|
|X-AUTH-TOKEN|header|string|true|Identificador de sesion de usuario.|

> Example responses

> 200 Response

```json
[
  {
    "company": {
      "documentValue": "20131257750",
      "documentType": "6",
      "description": "COSAPI SAC",
      "isPrincipal": true
    },
    "accounts": [
      {
        "accountId": "1931070017161004",
        "formattedAccountNumber": "193-107001716-1-61",
        "aliasAccount": "CUENTA PERU 2022",
        "statusCode": "a",
        "statusDescription": "Activa",
        "familyCode": "c",
        "familyDescription": "Corriente",
        "currencyCode": "USD",
        "currencyDescription": "Dolares",
        "currencySymbol": "$",
        "amountAvailable": 10,
        "amountUnavailable": 0,
        "amountAccountant": 10,
        "hashAccountId": "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0"
      }
    ]
  }
]
```

> 400 Response

```json
{
  "code": "TL0003",
  "description": "Los datos proporcionados no son validos.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0003",
      "component": "Channel Contract Account Overview",
      "description": "Los datos proporcionados no son validos."
    }
  ]
}
```

> 401 Response

```json
{
  "code": "TL0011",
  "description": "No esta autorizado correctamente para ejecutar esta operación.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0011",
      "component": "Channel Contract Account Overview",
      "description": "No esta autorizado correctamente para ejecutar esta operación."
    }
  ]
}
```

> 409 Response

```json
{
  "code": "TL0002",
  "description": "Ocurrió un error al validar las reglas de negocio.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0002",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error al validar las reglas de negocio."
    }
  ]
}
```

> 500 Response

```json
{
  "code": "TL0004",
  "description": "Ocurrió un error interno en el servicio.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0004",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error interno en el servicio."
    }
  ]
}
```

> 503 Response

```json
{
  "code": "TL0009",
  "description": "Ocurrio un error intentando invocar servicios externos.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0009",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrio un error intentando invocar servicios externos."
    }
  ]
}
```

<h3 id="listcompanyaccounts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se obtuvo la lista de las cuentas correctamente.|Inline|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|La operación no devolvió una respuesta.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|Los datos proporcionados no son validos.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|No esta autorizado correctamente para ejecutar esta operación.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Ocurrió un error al validar las reglas de negocio.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Ocurrió un error interno en el servicio.|[ApiException](#schemaapiexception)|
|503|[Service Unavailable](https://tools.ietf.org/html/rfc7231#section-6.6.4)|Ocurrio un error intentando invocar servicios externos.|[ApiException](#schemaapiexception)|

<h3 id="listcompanyaccounts-responseschema">Response Schema</h3>

Status Code **200**

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[[CompanyWithAccounts](#schemacompanywithaccounts)]|false|none|none|
|» company|[Company](#schemacompany)|false|none|Empresa|
|»» documentValue|string|false|none|none|
|»» documentType|string|false|none|none|
|»» description|string|false|none|none|
|»» isPrincipal|boolean|false|none|none|
|» accounts|[[Accounts](#schemaaccounts)]|false|none|[Listado de cuentas.]|
|»» accountId|string|true|none|N&uacute;mero de cuenta.|
|»» formattedAccountNumber|string|true|none|Formato de la cuenta.|
|»» aliasAccount|string|true|none|Alias de una cuenta.|
|»» statusCode|string|true|none|C&oacute;digo de status.|
|»» statusDescription|string|true|none|Descripci&oacute;n de status.|
|»» familyCode|string|true|none|C&oacute;digo de family.|
|»» familyDescription|string|true|none|Descripci&oacute;n de family.|
|»» currencyCode|string|true|none|C&oacute;digo tipo de moneda.|
|»» currencyDescription|string|true|none|Descripci&oacute;n tipo de moneda.|
|»» currencySymbol|string|true|none|Simbolo tipo de moneda.|
|»» amountAvailable|number|true|none|Saldo Disponible.|
|»» amountUnavailable|number|true|none|Saldo no Disponible.|
|»» amountAccountant|number|true|none|Saldo Contado.|
|»» hashAccountId|string|false|none|N&uacute;mero de cuenta encriptada.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-ux-ntlc-contract-account-overview-v2-account">Account</h1>


[](#listaccounts)

## ➤ listAccounts

<a id="opIdlistAccounts"></a>

> Code samples

```shell

[](#you-can-also-use-wget)

# ➤ You can also use wget
curl -X GET /channel/ntlc/v2/accounts \
  -H 'Accept: application/json' \
  -H 'Authorization: Bearer 363536363jjxnj63633611' \
  -H 'Request-ID: 550e8400-e29b-41d4-a716-446655440000' \
  -H 'X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000'

```

```http
GET /channel/ntlc/v2/accounts HTTP/1.1

Accept: application/json
Authorization: Bearer 363536363jjxnj63633611
Request-ID: 550e8400-e29b-41d4-a716-446655440000
X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000

```

```javascript

const headers = {
  'Accept':'application/json',
  'Authorization':'Bearer 363536363jjxnj63633611',
  'Request-ID':'550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN':'550e8400-e29b-41d4-a716-446655440000'
};

fetch('/channel/ntlc/v2/accounts',
{
  method: 'GET',

  headers: headers
})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});

```

```ruby
require 'rest-client'
require 'json'

headers = {
  'Accept' => 'application/json',
  'Authorization' => 'Bearer 363536363jjxnj63633611',
  'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000'
}

result = RestClient.get '/channel/ntlc/v2/accounts',
  params: {
  }, headers: headers

p JSON.parse(result)

```

```python
import requests
headers = {
  'Accept': 'application/json',
  'Authorization': 'Bearer 363536363jjxnj63633611',
  'Request-ID': '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN': '550e8400-e29b-41d4-a716-446655440000'
}

r = requests.get('/channel/ntlc/v2/accounts', headers = headers)

print(r.json())

```

```php
<?php

require 'vendor/autoload.php';

$headers = array(
    'Accept' => 'application/json',
    'Authorization' => 'Bearer 363536363jjxnj63633611',
    'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
    'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000',
);

$client = new \GuzzleHttp\Client();

// Define array of request body.
$request_body = array();

try {
    $response = $client->request('GET','/channel/ntlc/v2/accounts', array(
        'headers' => $headers,
        'json' => $request_body,
       )
    );
    print_r($response->getBody()->getContents());
 }
 catch (\GuzzleHttp\Exception\BadResponseException $e) {
    // handle exception or api errors.
    print_r($e->getMessage());
 }

 // ...

```

```java
URL obj = new URL("/channel/ntlc/v2/accounts");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());

```

```go
package main

import (
       "bytes"
       "net/http"
)

func main() {

    headers := map[string][]string{
        "Accept": []string{"application/json"},
        "Authorization": []string{"Bearer 363536363jjxnj63633611"},
        "Request-ID": []string{"550e8400-e29b-41d4-a716-446655440000"},
        "X-AUTH-TOKEN": []string{"550e8400-e29b-41d4-a716-446655440000"},
    }

    data := bytes.NewBuffer([]byte{jsonReq})
    req, err := http.NewRequest("GET", "/channel/ntlc/v2/accounts", data)
    req.Header = headers

    client := &http.Client{}
    resp, err := client.Do(req)
    // ...
}

```

`GET /accounts`

*Obtiene una lista de cuentas de una compañia.*

### Acerca de la funcionalidad expuesta

El servicio brinda las cuentas de la compañia seleccionada.

### Data de Prueba
No aplica.

### Precondiciones para el consumo de esta versión de la API
No aplica.

### Path Parameters
No aplica.

### Variantes válidas del Payload (Cuerpo del mesaje)
No aplica.

### Usos válidos de Query Parameters
No aplica.

### Variantes validas del Payload (Cuerpo del mensaje)
No aplica.

### Lista de Valores usadas en esta versión de la API
No aplica.

### Códigos de error usados en esta versión de la API

| Código | HTTP Status | Descripción |
|--------|-------------|-------------|
| TL0002 | 409 | Ocurrió un error al validar las reglas de negocio. |
| TL0003 | 400 | Los datos proporcionados no son validos. |
| TL0004 | 500 | Ocurrió un error interno en el servicio. |
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos.
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion. |

<h3 id="listaccounts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token de Authorización|
|Request-ID|header|string|true|Este campo es un valor estandar ya existente y sera usado como identificador.|
|X-AUTH-TOKEN|header|string|true|Identificador de sesion de usuario.|
|documentType|query|string|false|none|
|documentValue|query|string|false|none|
|sort|query|string|false|none|
|order|query|string|false|none|

> Example responses

> 200 Response

```json
[
  {
    "accountId": "1931070017161004",
    "formattedAccountNumber": "193-107001716-1-61",
    "aliasAccount": "CUENTA PERU 2022",
    "statusCode": "a",
    "statusDescription": "Activa",
    "familyCode": "c",
    "familyDescription": "Corriente",
    "currencyCode": "USD",
    "currencyDescription": "Dolares",
    "currencySymbol": "$",
    "amountAvailable": 10,
    "amountUnavailable": 0,
    "amountAccountant": 10,
    "hashAccountId": "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0"
  }
]
```

> 400 Response

```json
{
  "code": "TL0003",
  "description": "Los datos proporcionados no son validos.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0003",
      "component": "Channel Contract Account Overview",
      "description": "Los datos proporcionados no son validos."
    }
  ]
}
```

> 401 Response

```json
{
  "code": "TL0011",
  "description": "No esta autorizado correctamente para ejecutar esta operación.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0011",
      "component": "Channel Contract Account Overview",
      "description": "No esta autorizado correctamente para ejecutar esta operación."
    }
  ]
}
```

> 409 Response

```json
{
  "code": "TL0002",
  "description": "Ocurrió un error al validar las reglas de negocio.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0002",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error al validar las reglas de negocio."
    }
  ]
}
```

> 500 Response

```json
{
  "code": "TL0004",
  "description": "Ocurrió un error interno en el servicio.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0004",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrió un error interno en el servicio."
    }
  ]
}
```

> 503 Response

```json
{
  "code": "TL0009",
  "description": "Ocurrio un error intentando invocar servicios externos.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0009",
      "component": "Channel Contract Account Overview",
      "description": "Ocurrio un error intentando invocar servicios externos."
    }
  ]
}
```

<h3 id="listaccounts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se obtuvo la lista de las cuentas correctamente.|Inline|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|La operación no devolvió una respuesta.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|Los datos proporcionados no son validos.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|No esta autorizado correctamente para ejecutar esta operación.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Ocurrió un error al validar las reglas de negocio.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Ocurrió un error interno en el servicio.|[ApiException](#schemaapiexception)|
|503|[Service Unavailable](https://tools.ietf.org/html/rfc7231#section-6.6.4)|Ocurrio un error intentando invocar servicios externos.|[ApiException](#schemaapiexception)|

<h3 id="listaccounts-responseschema">Response Schema</h3>

Status Code **200**

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[[Accounts](#schemaaccounts)]|false|none|[Listado de cuentas.]|
|» accountId|string|true|none|N&uacute;mero de cuenta.|
|» formattedAccountNumber|string|true|none|Formato de la cuenta.|
|» aliasAccount|string|true|none|Alias de una cuenta.|
|» statusCode|string|true|none|C&oacute;digo de status.|
|» statusDescription|string|true|none|Descripci&oacute;n de status.|
|» familyCode|string|true|none|C&oacute;digo de family.|
|» familyDescription|string|true|none|Descripci&oacute;n de family.|
|» currencyCode|string|true|none|C&oacute;digo tipo de moneda.|
|» currencyDescription|string|true|none|Descripci&oacute;n tipo de moneda.|
|» currencySymbol|string|true|none|Simbolo tipo de moneda.|
|» amountAvailable|number|true|none|Saldo Disponible.|
|» amountUnavailable|number|true|none|Saldo no Disponible.|
|» amountAccountant|number|true|none|Saldo Contado.|
|» hashAccountId|string|false|none|N&uacute;mero de cuenta encriptada.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-ux-ntlc-contract-account-overview-v2-file-order">File order</h1>


[](#addfileorder)

## ➤ addFileOrder

<a id="opIdaddFileOrder"></a>

> Code samples

```shell

[](#you-can-also-use-wget)

# ➤ You can also use wget
curl -X POST /channel/ntlc/v2/file-orders/company-accounts \
  -H 'Content-Type: application/json' \
  -H 'Accept: application/json' \
  -H 'Authorization: Bearer 363536363jjxnj63633611' \
  -H 'Request-ID: 550e8400-e29b-41d4-a716-446655440000' \
  -H 'X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000'

```

```http
POST /channel/ntlc/v2/file-orders/company-accounts HTTP/1.1

Content-Type: application/json
Accept: application/json
Authorization: Bearer 363536363jjxnj63633611
Request-ID: 550e8400-e29b-41d4-a716-446655440000
X-AUTH-TOKEN: 550e8400-e29b-41d4-a716-446655440000

```

```javascript
const inputBody = '{
  "companyListFilter": [
    {
      "documentType": "6",
      "documentValue": "20307500630",
      "accountListFilter": [
        "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0",
        "b525b195650cccb3a4a4e04b1dfc98965f16a5c6e455d3d24052f48812672a28"
      ]
    }
  ],
  "columnsTable": [
    "account",
    "status",
    "accountType",
    "currency",
    "availableBalance",
    "countableBalance",
    "balanceNotAvailable"
  ],
  "fileFormat": "pdf",
  "txtSeparator": ";"
}';
const headers = {
  'Content-Type':'application/json',
  'Accept':'application/json',
  'Authorization':'Bearer 363536363jjxnj63633611',
  'Request-ID':'550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN':'550e8400-e29b-41d4-a716-446655440000'
};

fetch('/channel/ntlc/v2/file-orders/company-accounts',
{
  method: 'POST',
  body: inputBody,
  headers: headers
})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});

```

```ruby
require 'rest-client'
require 'json'

headers = {
  'Content-Type' => 'application/json',
  'Accept' => 'application/json',
  'Authorization' => 'Bearer 363536363jjxnj63633611',
  'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000'
}

result = RestClient.post '/channel/ntlc/v2/file-orders/company-accounts',
  params: {
  }, headers: headers

p JSON.parse(result)

```

```python
import requests
headers = {
  'Content-Type': 'application/json',
  'Accept': 'application/json',
  'Authorization': 'Bearer 363536363jjxnj63633611',
  'Request-ID': '550e8400-e29b-41d4-a716-446655440000',
  'X-AUTH-TOKEN': '550e8400-e29b-41d4-a716-446655440000'
}

r = requests.post('/channel/ntlc/v2/file-orders/company-accounts', headers = headers)

print(r.json())

```

```php
<?php

require 'vendor/autoload.php';

$headers = array(
    'Content-Type' => 'application/json',
    'Accept' => 'application/json',
    'Authorization' => 'Bearer 363536363jjxnj63633611',
    'Request-ID' => '550e8400-e29b-41d4-a716-446655440000',
    'X-AUTH-TOKEN' => '550e8400-e29b-41d4-a716-446655440000',
);

$client = new \GuzzleHttp\Client();

// Define array of request body.
$request_body = array();

try {
    $response = $client->request('POST','/channel/ntlc/v2/file-orders/company-accounts', array(
        'headers' => $headers,
        'json' => $request_body,
       )
    );
    print_r($response->getBody()->getContents());
 }
 catch (\GuzzleHttp\Exception\BadResponseException $e) {
    // handle exception or api errors.
    print_r($e->getMessage());
 }

 // ...

```

```java
URL obj = new URL("/channel/ntlc/v2/file-orders/company-accounts");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());

```

```go
package main

import (
       "bytes"
       "net/http"
)

func main() {

    headers := map[string][]string{
        "Content-Type": []string{"application/json"},
        "Accept": []string{"application/json"},
        "Authorization": []string{"Bearer 363536363jjxnj63633611"},
        "Request-ID": []string{"550e8400-e29b-41d4-a716-446655440000"},
        "X-AUTH-TOKEN": []string{"550e8400-e29b-41d4-a716-446655440000"},
    }

    data := bytes.NewBuffer([]byte{jsonReq})
    req, err := http.NewRequest("POST", "/channel/ntlc/v2/file-orders/company-accounts", data)
    req.Header = headers

    client := &http.Client{}
    resp, err := client.Do(req)
    // ...
}

```

`POST /file-orders/company-accounts`

*Crea una solicitud para generar un archivo con el listado de cuentas de las compañias seleccionas.*

### Acerca de la funcionalidad expuesta

El servicio crea la solicitud para la exportación de un archivo con un listado de cuentas y sus saldos, de las compañias seleccionadas.

### Data de Prueba
No aplica.

### Precondiciones para el consumo de esta versión de la API
No aplica.

### Path Parameters
No aplica.

### Variantes válidas del Payload (Cuerpo del mesaje)
No aplica.

### Usos válidos de Query Parameters
No aplica.

### Variantes validas del Payload (Cuerpo del mensaje)
No aplica.

### Lista de Valores usadas en esta versión de la API
No aplica.

### Códigos de error usados en esta versión de la API

| Código | HTTP Status | Descripción |
|--------|-------------|-------------|
| TL0002 | 409 | Ocurrió un error al validar las reglas de negocio. |
| TL0003 | 400 | Los datos proporcionados no son validos. |
| TL0004 | 500 | Ocurrió un error interno en el servicio. |
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos.
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion. |

> Body parameter

```json
{
  "companyListFilter": [
    {
      "documentType": "6",
      "documentValue": "20307500630",
      "accountListFilter": [
        "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0",
        "b525b195650cccb3a4a4e04b1dfc98965f16a5c6e455d3d24052f48812672a28"
      ]
    }
  ],
  "columnsTable": [
    "account",
    "status",
    "accountType",
    "currency",
    "availableBalance",
    "countableBalance",
    "balanceNotAvailable"
  ],
  "fileFormat": "pdf",
  "txtSeparator": ";"
}
```

<h3 id="addfileorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token de Authorización|
|Request-ID|header|string|true|Este campo es un valor estandar ya existente y sera usado como identificador.|
|X-AUTH-TOKEN|header|string|true|Identificador de sesion de usuario.|
|body|body|[ContractAccountExportRequest](#schemacontractaccountexportrequest)|false|none|

> Example responses

> 200 Response

```json
{
  "fileRequestNumber": "1232",
  "fileName": "archivo_todas_las_empresas"
}
```

> 400 Response

```json
{
  "code": "TL0003",
  "description": "Los datos proporcionados no son validos.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0003",
      "component": "Channel File Order Management",
      "description": "Los datos proporcionados no son validos."
    }
  ]
}
```

> 401 Response

```json
{
  "code": "TL0011",
  "description": "No esta autorizado correctamente para ejecutar esta operación.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0011",
      "component": "Channel File Order Management",
      "description": "No esta autorizado correctamente para ejecutar esta operación."
    }
  ]
}
```

> 409 Response

```json
{
  "code": "TL0002",
  "description": "Ocurrió un error al validar las reglas de negocio.",
  "errorType": "FUNCTIONAL",
  "exceptionDetail": [
    {
      "code": "TL0002",
      "component": "Channel File Order Management",
      "description": "Ocurrió un error al validar las reglas de negocio."
    }
  ]
}
```

> 500 Response

```json
{
  "code": "TL0004",
  "description": "Ocurrió un error interno en el servicio.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0004",
      "component": "Channel File Order Management",
      "description": "Ocurrió un error interno en el servicio."
    }
  ]
}
```

> 503 Response

```json
{
  "code": "TL0009",
  "description": "Ocurrio un error intentando invocar servicios externos.",
  "errorType": "TECHNICAL",
  "exceptionDetail": [
    {
      "code": "TL0009",
      "component": "Channel File Order Management",
      "description": "Ocurrio un error intentando invocar servicios externos."
    }
  ]
}
```

<h3 id="addfileorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se gener&oacute; correctamente la solicitud.|[ContractAccountExportResponse](#schemacontractaccountexportresponse)|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|La operación no devolvió una respuesta.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|Los datos proporcionados no son validos.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|No esta autorizado correctamente para ejecutar esta operación.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Ocurrió un error al validar las reglas de negocio.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Ocurrió un error interno en el servicio.|[ApiException](#schemaapiexception)|
|503|[Service Unavailable](https://tools.ietf.org/html/rfc7231#section-6.6.4)|Ocurrio un error intentando invocar servicios externos.|[ApiException](#schemaapiexception)|

<aside class="success">
This operation does not require authentication
</aside>


[](#schemas)

# ➤ Schemas

<h2 id="tocS_CompanyWithAccounts">CompanyWithAccounts</h2>

<a id="schemacompanywithaccounts"></a>
<a id="schema_CompanyWithAccounts"></a>
<a id="tocScompanywithaccounts"></a>
<a id="tocscompanywithaccounts"></a>

```json
{
  "company": {
    "documentValue": "20131257750",
    "documentType": "6",
    "description": "COSAPI SAC",
    "isPrincipal": true
  },
  "accounts": [
    {
      "accountId": "1931070017161004",
      "formattedAccountNumber": "193-107001716-1-61",
      "aliasAccount": "CUENTA PERU 2022",
      "statusCode": "a",
      "statusDescription": "Activa",
      "familyCode": "c",
      "familyDescription": "Corriente",
      "currencyCode": "USD",
      "currencyDescription": "Dolares",
      "currencySymbol": "$",
      "amountAvailable": 10,
      "amountUnavailable": 0,
      "amountAccountant": 10,
      "hashAccountId": "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|company|[Company](#schemacompany)|false|none|Empresa|
|accounts|[[Accounts](#schemaaccounts)]|false|none|[Listado de cuentas.]|

<h2 id="tocS_Company">Company</h2>

<a id="schemacompany"></a>
<a id="schema_Company"></a>
<a id="tocScompany"></a>
<a id="tocscompany"></a>

```json
{
  "documentValue": "20131257750",
  "documentType": "6",
  "description": "COSAPI SAC",
  "isPrincipal": true
}

```

Empresa

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|documentValue|string|false|none|none|
|documentType|string|false|none|none|
|description|string|false|none|none|
|isPrincipal|boolean|false|none|none|

<h2 id="tocS_ContractAccountExportRequest">ContractAccountExportRequest</h2>

<a id="schemacontractaccountexportrequest"></a>
<a id="schema_ContractAccountExportRequest"></a>
<a id="tocScontractaccountexportrequest"></a>
<a id="tocscontractaccountexportrequest"></a>

```json
{
  "companyListFilter": [
    {
      "documentType": "6",
      "documentValue": "20307500630",
      "accountListFilter": [
        "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0",
        "b525b195650cccb3a4a4e04b1dfc98965f16a5c6e455d3d24052f48812672a28"
      ]
    }
  ],
  "columnsTable": [
    "account",
    "status",
    "accountType",
    "currency",
    "availableBalance",
    "countableBalance",
    "balanceNotAvailable"
  ],
  "fileFormat": "pdf",
  "txtSeparator": ";"
}

```

ContractAccountExportRequest

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|companyListFilter|[companyListFilter](#schemacompanylistfilter)|false|none|none|
|columnsTable|[string]|true|none|none|
|fileFormat|string|true|none|Formato para exportar|
|txtSeparator|string|false|none|Separador de columnas para el formato txt|

<h2 id="tocS_companyListFilter">companyListFilter</h2>

<a id="schemacompanylistfilter"></a>
<a id="schema_companyListFilter"></a>
<a id="tocScompanylistfilter"></a>
<a id="tocscompanylistfilter"></a>

```json
[
  {
    "documentType": "6",
    "documentValue": "20307500630",
    "accountListFilter": [
      "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0",
      "b525b195650cccb3a4a4e04b1dfc98965f16a5c6e455d3d24052f48812672a28"
    ]
  }
]

```

companyListFilter

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|companyListFilter|[[companyFilter](#schemacompanyfilter)]|false|none|none|

<h2 id="tocS_companyFilter">companyFilter</h2>

<a id="schemacompanyfilter"></a>
<a id="schema_companyFilter"></a>
<a id="tocScompanyfilter"></a>
<a id="tocscompanyfilter"></a>

```json
{
  "documentType": "6",
  "documentValue": "20307500630",
  "accountListFilter": [
    "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0",
    "b525b195650cccb3a4a4e04b1dfc98965f16a5c6e455d3d24052f48812672a28"
  ]
}

```

companyFilter

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|documentType|string|false|none|none|
|documentValue|string|false|none|none|
|accountListFilter|[string]|false|none|none|

<h2 id="tocS_ContractAccountExportResponse">ContractAccountExportResponse</h2>

<a id="schemacontractaccountexportresponse"></a>
<a id="schema_ContractAccountExportResponse"></a>
<a id="tocScontractaccountexportresponse"></a>
<a id="tocscontractaccountexportresponse"></a>

```json
{
  "fileRequestNumber": "1232",
  "fileName": "archivo_todas_las_empresas"
}

```

Objeto con la informacion de la solicitud de exportacion

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|fileRequestNumber|string|false|none|none|
|fileName|string|false|none|none|

<h2 id="tocS_ContractAccountOverviewHeaders">ContractAccountOverviewHeaders</h2>

<a id="schemacontractaccountoverviewheaders"></a>
<a id="schema_ContractAccountOverviewHeaders"></a>
<a id="tocScontractaccountoverviewheaders"></a>
<a id="tocscontractaccountoverviewheaders"></a>

```json
{}

```

### Properties

*None*

<h2 id="tocS_Accounts">Accounts</h2>

<a id="schemaaccounts"></a>
<a id="schema_Accounts"></a>
<a id="tocSaccounts"></a>
<a id="tocsaccounts"></a>

```json
{
  "accountId": "1931070017161004",
  "formattedAccountNumber": "193-107001716-1-61",
  "aliasAccount": "CUENTA PERU 2022",
  "statusCode": "a",
  "statusDescription": "Activa",
  "familyCode": "c",
  "familyDescription": "Corriente",
  "currencyCode": "USD",
  "currencyDescription": "Dolares",
  "currencySymbol": "$",
  "amountAvailable": 10,
  "amountUnavailable": 0,
  "amountAccountant": 10,
  "hashAccountId": "fec5446f2b5e9d8b474f4a22cff649c25453d95f1a9915afb3b22eb2f83ee4f0"
}

```

Listado de cuentas.

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|accountId|string|true|none|N&uacute;mero de cuenta.|
|formattedAccountNumber|string|true|none|Formato de la cuenta.|
|aliasAccount|string|true|none|Alias de una cuenta.|
|statusCode|string|true|none|C&oacute;digo de status.|
|statusDescription|string|true|none|Descripci&oacute;n de status.|
|familyCode|string|true|none|C&oacute;digo de family.|
|familyDescription|string|true|none|Descripci&oacute;n de family.|
|currencyCode|string|true|none|C&oacute;digo tipo de moneda.|
|currencyDescription|string|true|none|Descripci&oacute;n tipo de moneda.|
|currencySymbol|string|true|none|Simbolo tipo de moneda.|
|amountAvailable|number|true|none|Saldo Disponible.|
|amountUnavailable|number|true|none|Saldo no Disponible.|
|amountAccountant|number|true|none|Saldo Contado.|
|hashAccountId|string|false|none|N&uacute;mero de cuenta encriptada.|

<h2 id="tocS_CompanyListResponse">CompanyListResponse</h2>

<a id="schemacompanylistresponse"></a>
<a id="schema_CompanyListResponse"></a>
<a id="tocScompanylistresponse"></a>
<a id="tocscompanylistresponse"></a>

```json
{
  "documentValue": "20461896344",
  "documentType": "1",
  "description": "121321",
  "isPrincipal": true,
  "accountsQuantity": 12,
  "creditCardsQuantity": 4
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|documentValue|string|false|none|Valor del documento|
|documentType|string|false|none|Tipo de documento|
|description|string|false|none|Nombre de empresa o raz&oacute;n social|
|isPrincipal|boolean|false|none|Identificador de empresa principal|
|accountsQuantity|integer(int32)|false|none|Numero de cuentas de la empresa|
|creditCardsQuantity|integer(int32)|false|none|Numero de tarjetas de credito de la empresa|

<h2 id="tocS_ApiException">ApiException</h2>

<a id="schemaapiexception"></a>
<a id="schema_ApiException"></a>
<a id="tocSapiexception"></a>
<a id="tocsapiexception"></a>

```json
{
  "code": "TL0001",
  "description": "Error al llamar al servicio",
  "errorType": "TECHNICAL",
  "exceptionDetails": [
    {
      "code": "MB0008",
      "component": "MB.CardInqV2",
      "description": "Codigo invalido para el canal"
    }
  ],
  "properties": {}
}

```

ApiException

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Codigo de error de Sistema|
|description|string|false|none|Descripcion del error de Sistema|
|errorType|string|false|none|Tipo de Error de Sistema|
|exceptionDetails|[[ApiExceptionDetail](#schemaapiexceptiondetail)]|false|none|Lista de detalles del error|
|properties|object|false|none|Lista de propiedades especiales.|

<h2 id="tocS_ApiExceptionDetail">ApiExceptionDetail</h2>

<a id="schemaapiexceptiondetail"></a>
<a id="schema_ApiExceptionDetail"></a>
<a id="tocSapiexceptiondetail"></a>
<a id="tocsapiexceptiondetail"></a>

```json
{
  "code": "MB0008",
  "component": "MB.CardInqV2",
  "description": "Codigo invalido para el canal"
}

```

ApiExceptionDetail

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Codigo de error del Detalle/Proveedor|
|component|string|false|none|Nombre del componente de falla|
|description|string|false|none|Descripcion del Detalle|

undefined



[](#autenticacion)

## ➤ Autenticacion
Esta API está protegida por el protocolo Open Authentication (OAuth). Luego del intercambio de token con OAuth, se concede un token OAuth válido para acceder a los diferentes endpoints API en nombre de un usuario de la aplicación autorizada.
Para ello, se deben generar el Cliente CAS:

[](#documentacin-de-arquitectura)

## ➤ Documentación de Arquitectura
Documentación de la Arquitectura de Solución asociada al API.
 
| Código SDAS      | Descripción                |
| :--------  | :------------------------- |
| **CODIGO_SDAS** | Creación del API |

alex


[](#portal-de-apis)

## ➤ Portal de APIs
El API se encuentra en el Portafolio de APIs en el siguiente link https://www.portalapisbcp.com/#/api-detail/_ID-PORTAL_

alex


[](#diagramas-de-arquitectura)

## ➤ Diagramas de arquitectura


![Diagrama](/assets/images/diagrama.svg)

alex


[](#deuda-tecnica)

## ➤ Deuda tecnica

Este documento describe la deuda técnica identificada en el archivo `openapi.yaml`. La deuda técnica en un archivo OpenAPI puede tener un impacto significativo en la calidad de la documentación, el desarrollo de los servicios, y la integración con sistemas externos.

---

alex
