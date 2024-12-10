
[](#api-pv-nrem-remittance-order-v1)

# ➤ API PV NREM Remittance Order V1
Version v1.0.3


[](#-indice)

## ➤ 📖 Indice

[](#table-of-contents)

## ➤ Table of Contents

* [➤ API PV NREM Remittance Order V1](#-api-pv-nrem-remittance-order-v1)
	* [➤ 📖 Indice](#--indice)
	* [➤ Decripcion General](#-decripcion-general)
		* [Documentación Extendida](#documentacin-extendida)
		* [Base URLs:](#base-urls)
	* [➤ Endpoints](#-endpoints)
	* [➤ getRemittanceOrder](#-getremittanceorder)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta)
		* [Información complementaria](#informacin-complementaria)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api)
		* [Data de Prueba](#data-de-prueba)
		* [Variantes válidas del Payload (Cuerpo del mensaje)](#variantes-vlidas-del-payload-cuerpo-del-mensaje)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api)
	* [➤ createRemittanceOrder](#-createremittanceorder)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta-1)
		* [URI de acceso a la API](#uri-de-acceso-a-la-api)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-1)
		* [Data de Prueba](#data-de-prueba-1)
		* [Headers Requeridos](#headers-requeridos)
		* [Path Parameters válidos en esta version de la API](#path-parameters-vlidos-en-esta-version-de-la-api)
		* [Query Parameters válidos en esta version de la API](#query-parameters-vlidos-en-esta-version-de-la-api)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-1)
		* [Variantes válidas del Payload (Cuerpo del mesaje)](#variantes-vlidas-del-payload-cuerpo-del-mesaje)
		* [Lista de Valores usadas en esta versión de la API](#lista-de-valores-usadas-en-esta-versin-de-la-api)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api-1)
	* [➤ getRemittanceOrderExchangeRate](#-getremittanceorderexchangerate)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta-2)
		* [Información complementaria](#informacin-complementaria-1)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-2)
		* [Data de Prueba](#data-de-prueba-2)
		* [Variantes válidas del Payload (Cuerpo del mensaje)](#variantes-vlidas-del-payload-cuerpo-del-mensaje-1)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-2)
		* [Códigos de error usados en esta versión de la API](#cdigos-de-error-usados-en-esta-versin-de-la-api-2)
	* [➤ createAnnulationOrder](#-createannulationorder)
		* [Acerca de la funcionalidad expuesta](#acerca-de-la-funcionalidad-expuesta-3)
		* [Información complementaria](#informacin-complementaria-2)
		* [Precondiciones para el consumo de esta versión de la API](#precondiciones-para-el-consumo-de-esta-versin-de-la-api-3)
		* [Data de Prueba](#data-de-prueba-3)
		* [Variantes válidas del Payload (Cuerpo del mensaje)](#variantes-vlidas-del-payload-cuerpo-del-mensaje-2)
		* [Usos válidos de Query Parameters](#usos-vlidos-de-query-parameters-3)
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
		* [Properties](#properties-11)
		* [Properties](#properties-12)
		* [Properties](#properties-13)
			* [Enumerated Values](#enumerated-values)
		* [Properties](#properties-14)
		* [Properties](#properties-15)
		* [Properties](#properties-16)
		* [Properties](#properties-17)
		* [Properties](#properties-18)
		* [Properties](#properties-19)
		* [Properties](#properties-20)
		* [Properties](#properties-21)
	* [➤ Autenticacion](#-autenticacion)
	* [➤ Documentación de Arquitectura](#-documentacin-de-arquitectura)
	* [➤ Portal de APIs](#-portal-de-apis)
	* [➤ Diagramas de arquitectura](#-diagramas-de-arquitectura)
	* [➤ Deuda tecnica](#-deuda-tecnica)
	* [➤ Deuda tecnica](#-deuda-tecnica-1)
	* [➤ **1. Estructura General**](#-1-estructura-general)
		* [Problemas:](#problemas)
		* [Soluciones:](#soluciones)
	* [➤ **2. Falta de Descripciones Detalladas**](#-2-falta-de-descripciones-detalladas)
		* [Problemas:](#problemas-1)
		* [Soluciones:](#soluciones-1)
	* [➤ **3. Inconsistencias en los Tipos de Datos**](#-3-inconsistencias-en-los-tipos-de-datos)
		* [Problemas:](#problemas-2)
		* [Soluciones:](#soluciones-2)
	* [➤ **4. Falta de Versionamiento**](#-4-falta-de-versionamiento)
		* [Problemas:](#problemas-3)
		* [Soluciones:](#soluciones-3)
	* [➤ **5. Códigos de Error y Respuestas**](#-5-cdigos-de-error-y-respuestas)
		* [Problemas:](#problemas-4)
		* [Soluciones:](#soluciones-4)
	* [➤ **6. Seguridad**](#-6-seguridad)
		* [Problemas:](#problemas-5)
		* [Soluciones:](#soluciones-5)
	* [➤ **7. Herramientas y Generación Automática**](#-7-herramientas-y-generacin-automtica)
		* [Problemas:](#problemas-6)
		* [Soluciones:](#soluciones-6)
	* [➤ **8. Testing**](#-8-testing)
		* [Problemas:](#problemas-7)
		* [Soluciones:](#soluciones-7)
	* [➤ **Conclusión**](#-conclusin)


[](#decripcion-general)

## ➤ Decripcion General
Permite registrar, anular y obtener el detalle de una orden de remesa, tambien permite obtener el tipo de cambio para una remesadora.

### Documentación Extendida

<a href="docs/README.md">Más información</a>

### Base URLs:

* <a href="/private/nrem/v1">/private/nrem/v1</a>

[](#endpoints)

## ➤ Endpoints

|Nro|TAG|HTTP Operation|Endpoint|Description|
|---|---|---|---|---|
|1|Remittance Orders|GET|/remittance-orders|Consultar solicitud de remesa.|
|2|Remittance Orders|POST|/remittance-orders|Registrar solicitud de remesa.|
|3|Remittance Orders|GET|/remittance-orders/exchange-rate|Consultar tipo de cambio.|
|4|Remittance Order Annulation|POST|/remittance-orders/annulations|Registrar anulacion de solicitud de remesa.|


<h1 id="api-pv-nrem-remittance-order-v1-remittance-orders">Remittance Orders</h1>


[](#getremittanceorder)

## ➤ getRemittanceOrder

<a id="opIdgetRemittanceOrder"></a>

`GET /remittance-orders`

*Consultar solicitud de remesa.*

### Acerca de la funcionalidad expuesta
La funcionalidad permite obtener datos relacionados a la orden de remesa para poder realizar seguimiento, los datos obtenidos son el estado de la orden,el terminal, la agencia, nombre del canal, codigo generado por el aplicativo remittance, la sucursal, fecha de registro, nombre y dni del beneficiario.

### Información complementaria
***“[Documentación Confluence APIS](https://confluence.lima.bcp.com.pe/display/MFCCPUB/APIS+de+Negocio)”***

### Precondiciones para el consumo de esta versión de la API
No aplica

### Data de Prueba
No aplica

### Variantes válidas del Payload (Cuerpo del mensaje)
No aplica.        

### Usos válidos de Query Parameters
| Query Params | Tipo de Dato | Descripcion | 
|----------|--------------|----------------
| referenceId | string | Clave de Referencia de cada envIo. | 
| merchantId | string | C??digo asignado por BCP a cada Compaña. | 

### Códigos de error usados en esta versión de la API
| Codigo | HTTP Status | Descripcion|
|--------|-------------|-------------|
| TL0003 | 400 | Los datos proporcionados no son válidos.|
| TL0004 | 503 | El servicio no se encuentra disponible. Por favor reintente mas tarde.|
| TL0005 | 500 | No se encontro el servidor solicitado.|
| TL0006 | 409 | Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|
| TL0007 | 500 | Ocurrio un error en el servicio externo.|
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos. Por favor contactarse con el Soporte Tecnico.|
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion.|
| TL9999 | 500 | Ocurrió un error inesperado. Por favor contactarse con Soporte Técnico.|

<h3 id="getremittanceorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token JWT de Authorización|
|subscription-key|header|string|true|Clave de suscripción, este campo es obtenido al momento de suscribirse al api o producto.|
|request-date|header|string|false|Fecha y hora en la que se realizó la petición. Esta cabecera puede ser usada para temas de auditoría.|
|request-id|header|string|false|Este campo es el identificador de la petición que será utilizado para fines de trazabilidad, es un valor estándar en formato UUID según RFC 4122.|
|app-code|header|string|false|Codigo de la aplicacion que invoca el servicio. Se debe usar el codigo de 2 caracteres que tienen asignada las aplicaciones, puede ser el canal.|
|caller-name|header|string|false|Este campo es el dominio desde el cual fue invocado el api.|
|referenceId|query|string|true|Clave de Referencia de cada envío.|
|merchantId|query|string|true|Código asignado por BCP a cada Compañía.|

> Example responses

> 200 Response

```json
{
  "title": "RemittanceOrderSearchResponse",
  "type": "object",
  "properties": {
    "remittanceOrderId": {
      "type": "string",
      "description": "Número Interno de la Operación en Remittance",
      "example": "9372834.0"
    },
    "registerDate": {
      "type": "string",
      "description": "Fecha y Hora de la operación",
      "example": "2019-10-20|19:00:00"
    },
    "status": {
      "title": "Status",
      "type": "object",
      "properties": {
        "code": {
          "type": "string",
          "description": "Estado de la Remesa ",
          "example": "ABONADO"
        },
        "description": {
          "type": "string",
          "description": "Descripción del estado de la Remesa ",
          "example": "Remesa disponible"
        }
      }
    },
    "beneficiary": {
      "title": "BeneficiarySearchResponse",
      "type": "object",
      "properties": {
        "beneficiaryId": {
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "type": "string",
          "description": "Nombre y apellidos completos del beneficiario.",
          "example": "Pablo Orladini Cevallos"
        }
      }
    },
    "branch": {
      "title": "Branch",
      "type": "object",
      "properties": {
        "branchOfficeId": {
          "type": "string",
          "description": "Código de sucursal ",
          "example": "193"
        }
      }
    },
    "agency": {
      "title": "Agency",
      "type": "object",
      "properties": {
        "agencyId": {
          "type": "string",
          "description": "Código de agencia",
          "example": "000"
        }
      }
    },
    "terminalId": {
      "type": "string",
      "description": "Terminal",
      "example": "H984649"
    },
    "referenceSource": {
      "type": "string",
      "description": "Nombre del Canal",
      "example": "AGENTE"
    }
  }
}
```

<h3 id="getremittanceorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se obtuvo el detalle de la orden de remesa|[RemittanceOrderSearchResponse](#schemaremittanceordersearchresponse)|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|No se pudo entender la solicitud debido a una sintaxis incorrecta.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|La solicitud requiere autenticaci&oacute;n de usuario. Si la solicitud ya incluia credenciales de autorizaci&oacute;n entonces se ha rechazado la autorizaci&oacute;n para esas credenciales.|[ApiException](#schemaapiexception)|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Se entendi&oacute; la solicitud, pero no se cumplir&aacute; debido a problemas relacionados con el cliente. El acceso al URI solicitado por el cliente esta prohibido por alg&uacute;n motivo.|[ApiException](#schemaapiexception)|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|No se ha encontrado nada que coincida con el URI de solicitud. El recurso especificado no existe o no puede mapear a un recurso.|[ApiException](#schemaapiexception)|
|405|[Method Not Allowed](https://tools.ietf.org/html/rfc7231#section-6.5.5)|El metodo especificado en la solicitud no esta permitido para el recurso identificado por el URI de solicitud.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|[ApiException](#schemaapiexception)|
|429|[Too Many Requests](https://tools.ietf.org/html/rfc6585#section-4)|El usuario ha enviado demasiadas solicitudes en un periodo de tiempo determinado. Esto sera controlado en el API Management.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Se encontro una condicion inesperada que impidio cumplir con la solicitud.|[ApiException](#schemaapiexception)|

<aside class="success">
This operation does not require authentication
</aside>


[](#createremittanceorder)

## ➤ createRemittanceOrder

<a id="opIdcreateRemittanceOrder"></a>

`POST /remittance-orders`

*Registrar solicitud de remesa.*

### Acerca de la funcionalidad expuesta
La funcionalidad permite ordenar una remesa. Los datos de una orden de remesa que se permite registrar son datos de la persona que envia, del beneficiario, información interna e información financiera.

### URI de acceso a la API
| Método | URI |
|--------|-------------|
|POST| /payment-initiation/v1/remittance-orders|

### Precondiciones para el consumo de esta versión de la API
No aplica.

### Data de Prueba
Ninguno.

### Headers Requeridos
| Header | Ejemplo |
|--------|-------------|
|Authorization|Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik|
|Ocp-Apim-Subscription-Key|5d95308ef8c9429eba5beee04bb15623|

### Path Parameters válidos en esta version de la API
Ninguno.

### Query Parameters válidos en esta version de la API
No aplica.

### Usos válidos de Query Parameters
No aplica.

### Variantes válidas del Payload (Cuerpo del mesaje)
 Datos validos para el registro de una orden de remesa. 
```
{
  "referenceId": "1275900000000001",
  "registerDate": "2019-10-21 00:00:00",
  "amount": 105.59,
  "amountPEN": 390.683,
  "exchangeRate": 3.7,
  "description": "PAGADOR BANCO DE CREDITO DEL PERU",
  "merchant": {
    "merchantId": "AAAAAAAAAAA"
  },
  "currency": {
    "code": "USD"
  },
  "sender": {
    "senderId": "154852154",
    "fullName": "RAMIREZ LOJA FREDY",
    "address": {
      "summary": "AV LOS PROCERES 345 D 101 A 12 URB FOVIPOL",
      "phoneNumber": "+013132000",
      "geolocation": {
        "province": {
          "description": "MICHIGAN"
        },
        "country": {
          "code": "USA",
          "description": "Estados Unidos"
        }
      }
    },
    "contactAddresses": [{
      "value": "+105927668437",
      "addressType": {
        "code": "CELULAR"
      }
    }],
    "cardAccountNumber": "192836470549756300000",
    "merchantSenderId": "70830409",
    "birthDate": "12/12/12",
    "birthDate": "Peru"
  },
  "beneficiary": {
    "beneficiaryId": "154852154",
    "fullName": "Pablo Orladini Cevallos",
    "address": {
      "summary": "AV LOS PROCERES 345 D 101 A 12 URB FOVIPOL",
      "phoneNumber": "+013132000",
      "geolocation": {
        "province": {
          "description": "MICHIGAN"
        },
        "country": {
          "code": "USA",
          "description": "Estados Unidos"
        }
      }
    },
    "contactAddresses": [{
      "value": "+105927668437",
      "addressType": {
        "code": "CELULAR"
      }
    }]
  },
  "depositInformation": {
    "account": {
      "accountId": "5434567891124625"
    }
  },
  "channel": "ACCOUNT"
}
```      

### Lista de Valores usadas en esta versión de la API
| Campo |
|-------|
| RemittanceOrders.currency |
|RemittanceOrders.sender.address.country |
|RemittanceOrders.sender.contactAddresses.addressType |
|RemittanceOrders.beneficiary.address.country   |
|RemittanceOrders.beneficiary.contactAddresses.addressType  | 
 
### Códigos de error usados en esta versión de la API
| Codigo | HTTP Status | Descripcion|
|--------|-------------|-------------|
| TL0003 | 400 | Los datos proporcionados no son válidos.|
| TL0004 | 503 | El servicio no se encuentra disponible. Por favor reintente mas tarde.|
| TL0005 | 500 | No se encontro el servidor solicitado.|
| TL0006 | 409 | Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|
| TL0007 | 500 | Ocurrio un error en el servicio externo.|
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos. Por favor contactarse con el Soporte Tecnico.|
| TL0011| 401 | No esta autorizado correctamente para ejecutar esta operacion.|
| TL9999 | 500 | Ocurrió un error inesperado. Por favor contactarse con Soporte Técnico.|

> Body parameter

```json
{
  "title": "RemittanceOrdersRequest",
  "type": "object",
  "properties": {
    "referenceId": {
      "maxLength": 16,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Clave de Referencia de cada envío.",
      "example": "1275900000000001"
    },
    "registerDate": {
      "maxLength": 19,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Fecha de envio",
      "example": "2019-10-21 00:00:00"
    },
    "amount": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Importe otorgado en la transacción",
      "format": "double",
      "example": 105.59
    },
    "amountPEN": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Importe otorgado en la transacción convertido a soles",
      "format": "double",
      "example": 390.683
    },
    "exchangeRate": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Tipo de cambio dolares a soles",
      "format": "double",
      "example": 3.7
    },
    "description": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Detalles de la orden.",
      "example": "PAGADOR BANCO DE CREDITO DEL PERU"
    },
    "merchant": {
      "title": "Merchant",
      "type": "object",
      "properties": {
        "merchantId": {
          "maxLength": 11,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Código asignado por BCP a cada Compañía."
        }
      }
    },
    "currency": {
      "title": "Currency",
      "type": "object",
      "properties": {
        "code": {
          "maxLength": 3,
          "minLength": 3,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Código de Tipo de moneda utilizada en la transacción.",
          "example": "USD"
        }
      }
    },
    "sender": {
      "title": "Sender",
      "type": "object",
      "properties": {
        "senderId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Nombre y apellidos completos del ordenante.",
          "example": "RAMIREZ LOJA FREDY"
        },
        "address": {
          "title": "Address",
          "type": "object",
          "properties": {
            "summary": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Direccion detallada.",
              "example": "AV LOS PROCERES 345 URB FOVIPOL"
            },
            "phoneNumber": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de telefono.",
              "example": "+013132000"
            },
            "geolocation": {
              "title": "Geolocation",
              "type": "object",
              "properties": {
                "province": {
                  "title": "Province",
                  "type": "object",
                  "properties": {
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del departamento/provincia del ordenante.",
                      "example": "MICHIGAN"
                    }
                  }
                },
                "country": {
                  "title": "Country",
                  "type": "object",
                  "properties": {
                    "code": {
                      "type": "string",
                      "description": "Código del pais.",
                      "example": "USA"
                    },
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del pais.",
                      "example": "Estados Unidos"
                    }
                  }
                }
              }
            }
          }
        },
        "contactAddresses": {
          "type": "array",
          "description": "Lista de Direcciones del la persona.",
          "items": {
            "title": "ContactAddressesCreate",
            "type": "object",
            "properties": {
              "value": {
                "maxLength": 35,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Número de celular /correo.",
                "example": "+105927668437"
              },
              "addressType": {
                "title": "AddressType",
                "type": "object",
                "properties": {
                  "code": {
                    "maxLength": 7,
                    "minLength": 1,
                    "pattern": "[a-zA-Z0-9-_]*$",
                    "type": "string",
                    "description": "Tipo de contacto Número de celular /correo.",
                    "example": "CELULAR"
                  }
                }
              }
            }
          }
        },
        "cardAccountNumber": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Numero de Cuenta o tarjeta de banco de la persona que envia la remesa.",
          "example": "192836470549756311012"
        },
        "merchantSenderId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Numero de identificacion del Sender.",
          "example": "70830409"
        },
        "birthDate": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Fecha de nacimiento.",
          "example": "12/12/12"
        },
        "birthCountry": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Pais de nacimiento.",
          "example": "Peru"
        }
      }
    },
    "beneficiary": {
      "title": "Beneficiary",
      "type": "object",
      "properties": {
        "beneficiaryId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Nombre y apellidos completos del beneficiario.",
          "example": "Pablo Orladini Cevallos"
        },
        "address": {
          "title": "Address",
          "type": "object",
          "properties": {
            "summary": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Direccion detallada.",
              "example": "AV LOS PROCERES 345 URB FOVIPOL"
            },
            "phoneNumber": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de telefono.",
              "example": "+013132000"
            },
            "geolocation": {
              "title": "Geolocation",
              "type": "object",
              "properties": {
                "province": {
                  "title": "Province",
                  "type": "object",
                  "properties": {
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del departamento/provincia del ordenante.",
                      "example": "MICHIGAN"
                    }
                  }
                },
                "country": {
                  "title": "Country",
                  "type": "object",
                  "properties": {
                    "code": {
                      "type": "string",
                      "description": "Código del pais.",
                      "example": "USA"
                    },
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del pais.",
                      "example": "Estados Unidos"
                    }
                  }
                }
              }
            }
          }
        },
        "contactAddresses": {
          "type": "array",
          "description": "Lista de Direcciones del la persona.",
          "items": {
            "title": "ContactAddressesCreate",
            "type": "object",
            "properties": {
              "value": {
                "maxLength": 35,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Número de celular /correo.",
                "example": "+105927668437"
              },
              "addressType": {
                "title": "AddressType",
                "type": "object",
                "properties": {
                  "code": {
                    "maxLength": 7,
                    "minLength": 1,
                    "pattern": "[a-zA-Z0-9-_]*$",
                    "type": "string",
                    "description": "Tipo de contacto Número de celular /correo.",
                    "example": "CELULAR"
                  }
                }
              }
            }
          }
        }
      }
    },
    "depositInformation": {
      "title": "DepositInformation",
      "type": "object",
      "properties": {
        "account": {
          "title": "Account",
          "type": "object",
          "properties": {
            "accountId": {
              "maxLength": 30,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de cuenta a depositar del cliente beneficiario",
              "example": "5434567891124625"
            }
          }
        }
      }
    },
    "channel": {
      "type": "string",
      "description": "Canal para el abono.",
      "enum": [
        "ACCOUNT",
        "PHONE",
        "COUNTER"
      ]
    }
  }
}
```

<h3 id="createremittanceorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token JWT de Authorización|
|subscription-key|header|string|true|Clave de suscripción, este campo es obtenido al momento de suscribirse al api o producto.|
|request-date|header|string|false|Fecha y hora en la que se realizó la petición. Esta cabecera puede ser usada para temas de auditoría.|
|request-id|header|string|false|Este campo es el identificador de la petición que será utilizado para fines de trazabilidad, es un valor estándar en formato UUID según RFC 4122.|
|app-code|header|string|false|Codigo de la aplicacion que invoca el servicio. Se debe usar el codigo de 2 caracteres que tienen asignada las aplicaciones, puede ser el canal.|
|caller-name|header|string|false|Este campo es el dominio desde el cual fue invocado el api.|
|body|body|[RemittanceOrdersRequest](#schemaremittanceordersrequest)|false|none|

> Example responses

> 400 Response

```json
{
  "title": "ApiException",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Codigo de error de Sistema",
      "example": "TL0001"
    },
    "description": {
      "type": "string",
      "description": "Descripcion del error de Sistema",
      "example": "Error al llamar al servicio"
    },
    "errorType": {
      "type": "string",
      "description": "Tipo de Error de Sistema",
      "example": "TECHNICAL"
    },
    "exceptionDetails": {
      "type": "array",
      "description": "Lista de detalles del error",
      "items": {
        "title": "ApiExceptionDetail",
        "type": "object",
        "properties": {
          "code": {
            "type": "string",
            "description": "Codigo de error del Detalle/Proveedor",
            "example": "MB0008"
          },
          "component": {
            "type": "string",
            "description": "Nombre del componente de falla",
            "example": "MB.CardInqV2"
          },
          "description": {
            "type": "string",
            "description": "Descripcion del Detalle",
            "example": "Codigo invalido para el canal"
          }
        },
        "description": "Datos del error técnico."
      }
    },
    "properties": {
      "type": "object",
      "properties": {},
      "description": "Lista de propiedades especiales."
    }
  },
  "description": "Datos del error de sistema."
}
```

<h3 id="createremittanceorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Remesa Registrada.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|No se pudo entender la solicitud debido a una sintaxis incorrecta.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|La solicitud requiere autenticaci&oacute;n de usuario. Si la solicitud ya incluia credenciales de autorizaci&oacute;n entonces se ha rechazado la autorizaci&oacute;n para esas credenciales.|[ApiException](#schemaapiexception)|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Se entendi&oacute; la solicitud, pero no se cumplir&aacute; debido a problemas relacionados con el cliente. El acceso al URI solicitado por el cliente esta prohibido por alg&uacute;n motivo.|[ApiException](#schemaapiexception)|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|No se ha encontrado nada que coincida con el URI de solicitud. El recurso especificado no existe o no puede mapear a un recurso.|[ApiException](#schemaapiexception)|
|405|[Method Not Allowed](https://tools.ietf.org/html/rfc7231#section-6.5.5)|El metodo especificado en la solicitud no esta permitido para el recurso identificado por el URI de solicitud.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|[ApiException](#schemaapiexception)|
|429|[Too Many Requests](https://tools.ietf.org/html/rfc6585#section-4)|El usuario ha enviado demasiadas solicitudes en un periodo de tiempo determinado. Esto sera controlado en el API Management.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Se encontro una condicion inesperada que impidio cumplir con la solicitud.|[ApiException](#schemaapiexception)|

<aside class="success">
This operation does not require authentication
</aside>


[](#getremittanceorderexchangerate)

## ➤ getRemittanceOrderExchangeRate

<a id="opIdgetRemittanceOrderExchangeRate"></a>

`GET /remittance-orders/exchange-rate`

*Consultar tipo de cambio.*

### Acerca de la funcionalidad expuesta
La funcionalidad permite permite obtener el tipo de cambio de cambio pizarra de la remesadora 

### Información complementaria
***“[Documentación Confluence APIS](https://confluence.lima.bcp.com.pe/display/MFCCPUB/APIS+de+Negocio)”***

### Precondiciones para el consumo de esta versión de la API
No aplica

### Data de Prueba
No aplica

### Variantes válidas del Payload (Cuerpo del mensaje)
No aplica.        

### Usos válidos de Query Parameters
| Query Params | Tipo de Dato | Descripcion | 
|----------|--------------|----------------
| merchantId | string | Código asignado por BCP a cada Compaña. | 

### Códigos de error usados en esta versión de la API
| Codigo | HTTP Status | Descripcion|
|--------|-------------|-------------|
| TL0003 | 400 | Los datos proporcionados no son válidos.|
| TL0004 | 503 | El servicio no se encuentra disponible. Por favor reintente mas tarde.|
| TL0005 | 500 | No se encontro el servidor solicitado.|
| TL0006 | 409 | Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|
| TL0007 | 500 | Ocurrio un error en el servicio externo.|
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos. Por favor contactarse con el Soporte Tecnico.|
| TL0011 | 401 | No esta autorizado correctamente para ejecutar esta operacion.|
| TL9999 | 500 | Ocurrió un error inesperado. Por favor contactarse con Soporte Técnico.|

<h3 id="getremittanceorderexchangerate-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token JWT de Authorización|
|subscription-key|header|string|true|Clave de suscripción, este campo es obtenido al momento de suscribirse al api o producto.|
|request-date|header|string|false|Fecha y hora en la que se realizó la petición. Esta cabecera puede ser usada para temas de auditoría.|
|request-id|header|string|false|Este campo es el identificador de la petición que será utilizado para fines de trazabilidad, es un valor estándar en formato UUID según RFC 4122.|
|app-code|header|string|false|Codigo de la aplicacion que invoca el servicio. Se debe usar el codigo de 2 caracteres que tienen asignada las aplicaciones, puede ser el canal.|
|caller-name|header|string|false|Este campo es el dominio desde el cual fue invocado el api.|
|merchantId|query|string|true|Código asignado por BCP a cada Compañía.|

> Example responses

> 200 Response

```json
{
  "type": "object",
  "properties": {
    "remittanceExchangeRate": {
      "type": "string",
      "description": "Número tipo cambio pizarra",
      "example": "3.71"
    }
  }
}
```

<h3 id="getremittanceorderexchangerate-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Se obtuvo el detalle de la orden de remesa.|[RemittanceOrderSearchExchangeRate](#schemaremittanceordersearchexchangerate)|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|No se pudo entender la solicitud debido a una sintaxis incorrecta.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|La solicitud requiere autenticaci&oacute;n de usuario. Si la solicitud ya incluia credenciales de autorizaci&oacute;n entonces se ha rechazado la autorizaci&oacute;n para esas credenciales.|[ApiException](#schemaapiexception)|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Se entendi&oacute; la solicitud, pero no se cumplir&aacute; debido a problemas relacionados con el cliente. El acceso al URI solicitado por el cliente esta prohibido por alg&uacute;n motivo.|[ApiException](#schemaapiexception)|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|No se ha encontrado nada que coincida con el URI de solicitud. El recurso especificado no existe o no puede mapear a un recurso.|[ApiException](#schemaapiexception)|
|405|[Method Not Allowed](https://tools.ietf.org/html/rfc7231#section-6.5.5)|El metodo especificado en la solicitud no esta permitido para el recurso identificado por el URI de solicitud.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|[ApiException](#schemaapiexception)|
|429|[Too Many Requests](https://tools.ietf.org/html/rfc6585#section-4)|El usuario ha enviado demasiadas solicitudes en un periodo de tiempo determinado. Esto sera controlado en el API Management.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Se encontro una condicion inesperada que impidio cumplir con la solicitud.|[ApiException](#schemaapiexception)|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="api-pv-nrem-remittance-order-v1-remittance-order-annulation">Remittance Order Annulation</h1>


[](#createannulationorder)

## ➤ createAnnulationOrder

<a id="opIdcreateAnnulationOrder"></a>

`POST /remittance-orders/annulations`

*Registrar anulacion de solicitud de remesa.*

### Acerca de la funcionalidad expuesta
Servicio que permite registrar una orden de anulacion pra una remesa

### Información complementaria
***“[Documentación Confluence APIS](https://confluence.lima.bcp.com.pe/display/MFCCPUB/APIS+de+Negocio)”***

### Precondiciones para el consumo de esta versión de la API
No aplica

### Data de Prueba
No aplica

### Variantes válidas del Payload (Cuerpo del mensaje)
No aplica.        

### Usos válidos de Query Parameters
| Query Params | Tipo de Dato | Descripcion | 
|----------|--------------|----------------
| referenceId | string | Clave de Referencia de cada envIo. | 
| merchantId | string | C??digo asignado por BCP a cada Compaña. | 

### Códigos de error usados en esta versión de la API
| Codigo | HTTP Status | Descripcion|
|--------|-------------|-------------|
| TL0003 | 400 | Los datos proporcionados no son válidos.|
| TL0004 | 503 | El servicio no se encuentra disponible. Por favor reintente mas tarde.|
| TL0005 | 500 | No se encontro el servidor solicitado.|
| TL0006 | 409 | Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|
| TL0007 | 500 | Ocurrio un error en el servicio externo.|
| TL0009 | 503 | Ocurrio un error intentando invocar servicios externos. Por favor contactarse con el Soporte Tecnico.|
| TL0011| 401 | No esta autorizado correctamente para ejecutar esta operacion.|
| TL9999 | 500 | Ocurrió un error inesperado. Por favor contactarse con Soporte Técnico.|

<h3 id="createannulationorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Authorization|header|string|true|Token JWT de Authorización|
|subscription-key|header|string|true|Clave de suscripción, este campo es obtenido al momento de suscribirse al api o producto.|
|request-date|header|string|false|Fecha y hora en la que se realizó la petición. Esta cabecera puede ser usada para temas de auditoría.|
|request-id|header|string|false|Este campo es el identificador de la petición que será utilizado para fines de trazabilidad, es un valor estándar en formato UUID según RFC 4122.|
|app-code|header|string|false|Codigo de la aplicacion que invoca el servicio. Se debe usar el codigo de 2 caracteres que tienen asignada las aplicaciones, puede ser el canal.|
|caller-name|header|string|false|Este campo es el dominio desde el cual fue invocado el api.|
|referenceId|query|string|true|Clave de Referencia de cada envío.|
|merchantId|query|string|true|Código asignado por BCP a cada Compañía.|

> Example responses

> 400 Response

```json
{
  "title": "ApiException",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Codigo de error de Sistema",
      "example": "TL0001"
    },
    "description": {
      "type": "string",
      "description": "Descripcion del error de Sistema",
      "example": "Error al llamar al servicio"
    },
    "errorType": {
      "type": "string",
      "description": "Tipo de Error de Sistema",
      "example": "TECHNICAL"
    },
    "exceptionDetails": {
      "type": "array",
      "description": "Lista de detalles del error",
      "items": {
        "title": "ApiExceptionDetail",
        "type": "object",
        "properties": {
          "code": {
            "type": "string",
            "description": "Codigo de error del Detalle/Proveedor",
            "example": "MB0008"
          },
          "component": {
            "type": "string",
            "description": "Nombre del componente de falla",
            "example": "MB.CardInqV2"
          },
          "description": {
            "type": "string",
            "description": "Descripcion del Detalle",
            "example": "Codigo invalido para el canal"
          }
        },
        "description": "Datos del error técnico."
      }
    },
    "properties": {
      "type": "object",
      "properties": {},
      "description": "Lista de propiedades especiales."
    }
  },
  "description": "Datos del error de sistema."
}
```

<h3 id="createannulationorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Orden de anulación Registrada.|None|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|No se pudo entender la solicitud debido a una sintaxis incorrecta.|[ApiException](#schemaapiexception)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|La solicitud requiere autenticaci&oacute;n de usuario. Si la solicitud ya incluia credenciales de autorizaci&oacute;n entonces se ha rechazado la autorizaci&oacute;n para esas credenciales.|[ApiException](#schemaapiexception)|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Se entendi&oacute; la solicitud, pero no se cumplir&aacute; debido a problemas relacionados con el cliente. El acceso al URI solicitado por el cliente esta prohibido por alg&uacute;n motivo.|[ApiException](#schemaapiexception)|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|No se ha encontrado nada que coincida con el URI de solicitud. El recurso especificado no existe o no puede mapear a un recurso.|[ApiException](#schemaapiexception)|
|405|[Method Not Allowed](https://tools.ietf.org/html/rfc7231#section-6.5.5)|El metodo especificado en la solicitud no esta permitido para el recurso identificado por el URI de solicitud.|[ApiException](#schemaapiexception)|
|409|[Conflict](https://tools.ietf.org/html/rfc7231#section-6.5.8)|Conflicto entre el recurso a actualizar y el que se encuentra en el sistema.|[ApiException](#schemaapiexception)|
|429|[Too Many Requests](https://tools.ietf.org/html/rfc6585#section-4)|El usuario ha enviado demasiadas solicitudes en un periodo de tiempo determinado. Esto sera controlado en el API Management.|[ApiException](#schemaapiexception)|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|Se encontro una condicion inesperada que impidio cumplir con la solicitud.|[ApiException](#schemaapiexception)|

<aside class="success">
This operation does not require authentication
</aside>


[](#schemas)

# ➤ Schemas

<h2 id="tocS_RemittanceOrdersHeaders">RemittanceOrdersHeaders</h2>

<a id="schemaremittanceordersheaders"></a>
<a id="schema_RemittanceOrdersHeaders"></a>
<a id="tocSremittanceordersheaders"></a>
<a id="tocsremittanceordersheaders"></a>

```json
{
  "title": "RemittanceOrdersHeaders",
  "type": "object"
}

```

RemittanceOrdersHeaders

### Properties

*None*

<h2 id="tocS_Merchant">Merchant</h2>

<a id="schemamerchant"></a>
<a id="schema_Merchant"></a>
<a id="tocSmerchant"></a>
<a id="tocsmerchant"></a>

```json
{
  "title": "Merchant",
  "type": "object",
  "properties": {
    "merchantId": {
      "maxLength": 11,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Código asignado por BCP a cada Compañía."
    }
  }
}

```

Merchant

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|merchantId|string|false|none|Código asignado por BCP a cada Compañía.|

<h2 id="tocS_Currency">Currency</h2>

<a id="schemacurrency"></a>
<a id="schema_Currency"></a>
<a id="tocScurrency"></a>
<a id="tocscurrency"></a>

```json
{
  "title": "Currency",
  "type": "object",
  "properties": {
    "code": {
      "maxLength": 3,
      "minLength": 3,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Código de Tipo de moneda utilizada en la transacción.",
      "example": "USD"
    }
  }
}

```

Currency

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Código de Tipo de moneda utilizada en la transacción.|

<h2 id="tocS_Province">Province</h2>

<a id="schemaprovince"></a>
<a id="schema_Province"></a>
<a id="tocSprovince"></a>
<a id="tocsprovince"></a>

```json
{
  "title": "Province",
  "type": "object",
  "properties": {
    "description": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Descripción del departamento/provincia del ordenante.",
      "example": "MICHIGAN"
    }
  }
}

```

Province

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|description|string|false|none|Descripción del departamento/provincia del ordenante.|

<h2 id="tocS_Country">Country</h2>

<a id="schemacountry"></a>
<a id="schema_Country"></a>
<a id="tocScountry"></a>
<a id="tocscountry"></a>

```json
{
  "title": "Country",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Código del pais.",
      "example": "USA"
    },
    "description": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Descripción del pais.",
      "example": "Estados Unidos"
    }
  }
}

```

Country

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Código del pais.|
|description|string|false|none|Descripción del pais.|

<h2 id="tocS_Geolocation">Geolocation</h2>

<a id="schemageolocation"></a>
<a id="schema_Geolocation"></a>
<a id="tocSgeolocation"></a>
<a id="tocsgeolocation"></a>

```json
{
  "title": "Geolocation",
  "type": "object",
  "properties": {
    "province": {
      "title": "Province",
      "type": "object",
      "properties": {
        "description": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Descripción del departamento/provincia del ordenante.",
          "example": "MICHIGAN"
        }
      }
    },
    "country": {
      "title": "Country",
      "type": "object",
      "properties": {
        "code": {
          "type": "string",
          "description": "Código del pais.",
          "example": "USA"
        },
        "description": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Descripción del pais.",
          "example": "Estados Unidos"
        }
      }
    }
  }
}

```

Geolocation

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|province|[Province](#schemaprovince)|false|none|none|
|country|[Country](#schemacountry)|false|none|none|

<h2 id="tocS_Address">Address</h2>

<a id="schemaaddress"></a>
<a id="schema_Address"></a>
<a id="tocSaddress"></a>
<a id="tocsaddress"></a>

```json
{
  "title": "Address",
  "type": "object",
  "properties": {
    "summary": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Direccion detallada.",
      "example": "AV LOS PROCERES 345 URB FOVIPOL"
    },
    "phoneNumber": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Número de telefono.",
      "example": "+013132000"
    },
    "geolocation": {
      "title": "Geolocation",
      "type": "object",
      "properties": {
        "province": {
          "title": "Province",
          "type": "object",
          "properties": {
            "description": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Descripción del departamento/provincia del ordenante.",
              "example": "MICHIGAN"
            }
          }
        },
        "country": {
          "title": "Country",
          "type": "object",
          "properties": {
            "code": {
              "type": "string",
              "description": "Código del pais.",
              "example": "USA"
            },
            "description": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Descripción del pais.",
              "example": "Estados Unidos"
            }
          }
        }
      }
    }
  }
}

```

Address

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|summary|string|false|none|Direccion detallada.|
|phoneNumber|string|false|none|Número de telefono.|
|geolocation|[Geolocation](#schemageolocation)|false|none|none|

<h2 id="tocS_AddressType">AddressType</h2>

<a id="schemaaddresstype"></a>
<a id="schema_AddressType"></a>
<a id="tocSaddresstype"></a>
<a id="tocsaddresstype"></a>

```json
{
  "title": "AddressType",
  "type": "object",
  "properties": {
    "code": {
      "maxLength": 7,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Tipo de contacto Número de celular /correo.",
      "example": "CELULAR"
    }
  }
}

```

AddressType

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Tipo de contacto Número de celular /correo.|

<h2 id="tocS_ContactAddressesCreate">ContactAddressesCreate</h2>

<a id="schemacontactaddressescreate"></a>
<a id="schema_ContactAddressesCreate"></a>
<a id="tocScontactaddressescreate"></a>
<a id="tocscontactaddressescreate"></a>

```json
{
  "title": "ContactAddressesCreate",
  "type": "object",
  "properties": {
    "value": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Número de celular /correo.",
      "example": "+105927668437"
    },
    "addressType": {
      "title": "AddressType",
      "type": "object",
      "properties": {
        "code": {
          "maxLength": 7,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Tipo de contacto Número de celular /correo.",
          "example": "CELULAR"
        }
      }
    }
  }
}

```

ContactAddressesCreate

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|value|string|false|none|Número de celular /correo.|
|addressType|[AddressType](#schemaaddresstype)|false|none|none|

<h2 id="tocS_Sender">Sender</h2>

<a id="schemasender"></a>
<a id="schema_Sender"></a>
<a id="tocSsender"></a>
<a id="tocssender"></a>

```json
{
  "title": "Sender",
  "type": "object",
  "properties": {
    "senderId": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Doc. De identidad.",
      "example": "154852154"
    },
    "fullName": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Nombre y apellidos completos del ordenante.",
      "example": "RAMIREZ LOJA FREDY"
    },
    "address": {
      "title": "Address",
      "type": "object",
      "properties": {
        "summary": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Direccion detallada.",
          "example": "AV LOS PROCERES 345 URB FOVIPOL"
        },
        "phoneNumber": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Número de telefono.",
          "example": "+013132000"
        },
        "geolocation": {
          "title": "Geolocation",
          "type": "object",
          "properties": {
            "province": {
              "title": "Province",
              "type": "object",
              "properties": {
                "description": {
                  "maxLength": 35,
                  "minLength": 1,
                  "pattern": "[a-zA-Z0-9-_]*$",
                  "type": "string",
                  "description": "Descripción del departamento/provincia del ordenante.",
                  "example": "MICHIGAN"
                }
              }
            },
            "country": {
              "title": "Country",
              "type": "object",
              "properties": {
                "code": {
                  "type": "string",
                  "description": "Código del pais.",
                  "example": "USA"
                },
                "description": {
                  "maxLength": 35,
                  "minLength": 1,
                  "pattern": "[a-zA-Z0-9-_]*$",
                  "type": "string",
                  "description": "Descripción del pais.",
                  "example": "Estados Unidos"
                }
              }
            }
          }
        }
      }
    },
    "contactAddresses": {
      "type": "array",
      "description": "Lista de Direcciones del la persona.",
      "items": {
        "title": "ContactAddressesCreate",
        "type": "object",
        "properties": {
          "value": {
            "maxLength": 35,
            "minLength": 1,
            "pattern": "[a-zA-Z0-9-_]*$",
            "type": "string",
            "description": "Número de celular /correo.",
            "example": "+105927668437"
          },
          "addressType": {
            "title": "AddressType",
            "type": "object",
            "properties": {
              "code": {
                "maxLength": 7,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Tipo de contacto Número de celular /correo.",
                "example": "CELULAR"
              }
            }
          }
        }
      }
    },
    "cardAccountNumber": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Numero de Cuenta o tarjeta de banco de la persona que envia la remesa.",
      "example": "192836470549756311012"
    },
    "merchantSenderId": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Numero de identificacion del Sender.",
      "example": "70830409"
    },
    "birthDate": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Fecha de nacimiento.",
      "example": "12/12/12"
    },
    "birthCountry": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Pais de nacimiento.",
      "example": "Peru"
    }
  }
}

```

Sender

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|senderId|string|false|none|Doc. De identidad.|
|fullName|string|false|none|Nombre y apellidos completos del ordenante.|
|address|[Address](#schemaaddress)|false|none|none|
|contactAddresses|[[ContactAddressesCreate](#schemacontactaddressescreate)]|false|none|Lista de Direcciones del la persona.|
|cardAccountNumber|string|false|none|Numero de Cuenta o tarjeta de banco de la persona que envia la remesa.|
|merchantSenderId|string|false|none|Numero de identificacion del Sender.|
|birthDate|string|false|none|Fecha de nacimiento.|
|birthCountry|string|false|none|Pais de nacimiento.|

<h2 id="tocS_Beneficiary">Beneficiary</h2>

<a id="schemabeneficiary"></a>
<a id="schema_Beneficiary"></a>
<a id="tocSbeneficiary"></a>
<a id="tocsbeneficiary"></a>

```json
{
  "title": "Beneficiary",
  "type": "object",
  "properties": {
    "beneficiaryId": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Doc. De identidad.",
      "example": "154852154"
    },
    "fullName": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Nombre y apellidos completos del beneficiario.",
      "example": "Pablo Orladini Cevallos"
    },
    "address": {
      "title": "Address",
      "type": "object",
      "properties": {
        "summary": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Direccion detallada.",
          "example": "AV LOS PROCERES 345 URB FOVIPOL"
        },
        "phoneNumber": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Número de telefono.",
          "example": "+013132000"
        },
        "geolocation": {
          "title": "Geolocation",
          "type": "object",
          "properties": {
            "province": {
              "title": "Province",
              "type": "object",
              "properties": {
                "description": {
                  "maxLength": 35,
                  "minLength": 1,
                  "pattern": "[a-zA-Z0-9-_]*$",
                  "type": "string",
                  "description": "Descripción del departamento/provincia del ordenante.",
                  "example": "MICHIGAN"
                }
              }
            },
            "country": {
              "title": "Country",
              "type": "object",
              "properties": {
                "code": {
                  "type": "string",
                  "description": "Código del pais.",
                  "example": "USA"
                },
                "description": {
                  "maxLength": 35,
                  "minLength": 1,
                  "pattern": "[a-zA-Z0-9-_]*$",
                  "type": "string",
                  "description": "Descripción del pais.",
                  "example": "Estados Unidos"
                }
              }
            }
          }
        }
      }
    },
    "contactAddresses": {
      "type": "array",
      "description": "Lista de Direcciones del la persona.",
      "items": {
        "title": "ContactAddressesCreate",
        "type": "object",
        "properties": {
          "value": {
            "maxLength": 35,
            "minLength": 1,
            "pattern": "[a-zA-Z0-9-_]*$",
            "type": "string",
            "description": "Número de celular /correo.",
            "example": "+105927668437"
          },
          "addressType": {
            "title": "AddressType",
            "type": "object",
            "properties": {
              "code": {
                "maxLength": 7,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Tipo de contacto Número de celular /correo.",
                "example": "CELULAR"
              }
            }
          }
        }
      }
    }
  }
}

```

Beneficiary

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|beneficiaryId|string|false|none|Doc. De identidad.|
|fullName|string|false|none|Nombre y apellidos completos del beneficiario.|
|address|[Address](#schemaaddress)|false|none|none|
|contactAddresses|[[ContactAddressesCreate](#schemacontactaddressescreate)]|false|none|Lista de Direcciones del la persona.|

<h2 id="tocS_Account">Account</h2>

<a id="schemaaccount"></a>
<a id="schema_Account"></a>
<a id="tocSaccount"></a>
<a id="tocsaccount"></a>

```json
{
  "title": "Account",
  "type": "object",
  "properties": {
    "accountId": {
      "maxLength": 30,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Número de cuenta a depositar del cliente beneficiario",
      "example": "5434567891124625"
    }
  }
}

```

Account

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|accountId|string|false|none|Número de cuenta a depositar del cliente beneficiario|

<h2 id="tocS_DepositInformation">DepositInformation</h2>

<a id="schemadepositinformation"></a>
<a id="schema_DepositInformation"></a>
<a id="tocSdepositinformation"></a>
<a id="tocsdepositinformation"></a>

```json
{
  "title": "DepositInformation",
  "type": "object",
  "properties": {
    "account": {
      "title": "Account",
      "type": "object",
      "properties": {
        "accountId": {
          "maxLength": 30,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Número de cuenta a depositar del cliente beneficiario",
          "example": "5434567891124625"
        }
      }
    }
  }
}

```

DepositInformation

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|account|[Account](#schemaaccount)|false|none|none|

<h2 id="tocS_RemittanceOrdersRequest">RemittanceOrdersRequest</h2>

<a id="schemaremittanceordersrequest"></a>
<a id="schema_RemittanceOrdersRequest"></a>
<a id="tocSremittanceordersrequest"></a>
<a id="tocsremittanceordersrequest"></a>

```json
{
  "title": "RemittanceOrdersRequest",
  "type": "object",
  "properties": {
    "referenceId": {
      "maxLength": 16,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Clave de Referencia de cada envío.",
      "example": "1275900000000001"
    },
    "registerDate": {
      "maxLength": 19,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Fecha de envio",
      "example": "2019-10-21 00:00:00"
    },
    "amount": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Importe otorgado en la transacción",
      "format": "double",
      "example": 105.59
    },
    "amountPEN": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Importe otorgado en la transacción convertido a soles",
      "format": "double",
      "example": 390.683
    },
    "exchangeRate": {
      "maximum": 999999999,
      "minimum": 1,
      "type": "number",
      "description": "Tipo de cambio dolares a soles",
      "format": "double",
      "example": 3.7
    },
    "description": {
      "maxLength": 35,
      "minLength": 1,
      "pattern": "[a-zA-Z0-9-_]*$",
      "type": "string",
      "description": "Detalles de la orden.",
      "example": "PAGADOR BANCO DE CREDITO DEL PERU"
    },
    "merchant": {
      "title": "Merchant",
      "type": "object",
      "properties": {
        "merchantId": {
          "maxLength": 11,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Código asignado por BCP a cada Compañía."
        }
      }
    },
    "currency": {
      "title": "Currency",
      "type": "object",
      "properties": {
        "code": {
          "maxLength": 3,
          "minLength": 3,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Código de Tipo de moneda utilizada en la transacción.",
          "example": "USD"
        }
      }
    },
    "sender": {
      "title": "Sender",
      "type": "object",
      "properties": {
        "senderId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Nombre y apellidos completos del ordenante.",
          "example": "RAMIREZ LOJA FREDY"
        },
        "address": {
          "title": "Address",
          "type": "object",
          "properties": {
            "summary": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Direccion detallada.",
              "example": "AV LOS PROCERES 345 URB FOVIPOL"
            },
            "phoneNumber": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de telefono.",
              "example": "+013132000"
            },
            "geolocation": {
              "title": "Geolocation",
              "type": "object",
              "properties": {
                "province": {
                  "title": "Province",
                  "type": "object",
                  "properties": {
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del departamento/provincia del ordenante.",
                      "example": "MICHIGAN"
                    }
                  }
                },
                "country": {
                  "title": "Country",
                  "type": "object",
                  "properties": {
                    "code": {
                      "type": "string",
                      "description": "Código del pais.",
                      "example": "USA"
                    },
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del pais.",
                      "example": "Estados Unidos"
                    }
                  }
                }
              }
            }
          }
        },
        "contactAddresses": {
          "type": "array",
          "description": "Lista de Direcciones del la persona.",
          "items": {
            "title": "ContactAddressesCreate",
            "type": "object",
            "properties": {
              "value": {
                "maxLength": 35,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Número de celular /correo.",
                "example": "+105927668437"
              },
              "addressType": {
                "title": "AddressType",
                "type": "object",
                "properties": {
                  "code": {
                    "maxLength": 7,
                    "minLength": 1,
                    "pattern": "[a-zA-Z0-9-_]*$",
                    "type": "string",
                    "description": "Tipo de contacto Número de celular /correo.",
                    "example": "CELULAR"
                  }
                }
              }
            }
          }
        },
        "cardAccountNumber": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Numero de Cuenta o tarjeta de banco de la persona que envia la remesa.",
          "example": "192836470549756311012"
        },
        "merchantSenderId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Numero de identificacion del Sender.",
          "example": "70830409"
        },
        "birthDate": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Fecha de nacimiento.",
          "example": "12/12/12"
        },
        "birthCountry": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Pais de nacimiento.",
          "example": "Peru"
        }
      }
    },
    "beneficiary": {
      "title": "Beneficiary",
      "type": "object",
      "properties": {
        "beneficiaryId": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "maxLength": 35,
          "minLength": 1,
          "pattern": "[a-zA-Z0-9-_]*$",
          "type": "string",
          "description": "Nombre y apellidos completos del beneficiario.",
          "example": "Pablo Orladini Cevallos"
        },
        "address": {
          "title": "Address",
          "type": "object",
          "properties": {
            "summary": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Direccion detallada.",
              "example": "AV LOS PROCERES 345 URB FOVIPOL"
            },
            "phoneNumber": {
              "maxLength": 35,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de telefono.",
              "example": "+013132000"
            },
            "geolocation": {
              "title": "Geolocation",
              "type": "object",
              "properties": {
                "province": {
                  "title": "Province",
                  "type": "object",
                  "properties": {
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del departamento/provincia del ordenante.",
                      "example": "MICHIGAN"
                    }
                  }
                },
                "country": {
                  "title": "Country",
                  "type": "object",
                  "properties": {
                    "code": {
                      "type": "string",
                      "description": "Código del pais.",
                      "example": "USA"
                    },
                    "description": {
                      "maxLength": 35,
                      "minLength": 1,
                      "pattern": "[a-zA-Z0-9-_]*$",
                      "type": "string",
                      "description": "Descripción del pais.",
                      "example": "Estados Unidos"
                    }
                  }
                }
              }
            }
          }
        },
        "contactAddresses": {
          "type": "array",
          "description": "Lista de Direcciones del la persona.",
          "items": {
            "title": "ContactAddressesCreate",
            "type": "object",
            "properties": {
              "value": {
                "maxLength": 35,
                "minLength": 1,
                "pattern": "[a-zA-Z0-9-_]*$",
                "type": "string",
                "description": "Número de celular /correo.",
                "example": "+105927668437"
              },
              "addressType": {
                "title": "AddressType",
                "type": "object",
                "properties": {
                  "code": {
                    "maxLength": 7,
                    "minLength": 1,
                    "pattern": "[a-zA-Z0-9-_]*$",
                    "type": "string",
                    "description": "Tipo de contacto Número de celular /correo.",
                    "example": "CELULAR"
                  }
                }
              }
            }
          }
        }
      }
    },
    "depositInformation": {
      "title": "DepositInformation",
      "type": "object",
      "properties": {
        "account": {
          "title": "Account",
          "type": "object",
          "properties": {
            "accountId": {
              "maxLength": 30,
              "minLength": 1,
              "pattern": "[a-zA-Z0-9-_]*$",
              "type": "string",
              "description": "Número de cuenta a depositar del cliente beneficiario",
              "example": "5434567891124625"
            }
          }
        }
      }
    },
    "channel": {
      "type": "string",
      "description": "Canal para el abono.",
      "enum": [
        "ACCOUNT",
        "PHONE",
        "COUNTER"
      ]
    }
  }
}

```

RemittanceOrdersRequest

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|referenceId|string|false|none|Clave de Referencia de cada envío.|
|registerDate|string|false|none|Fecha de envio|
|amount|number(double)|false|none|Importe otorgado en la transacción|
|amountPEN|number(double)|false|none|Importe otorgado en la transacción convertido a soles|
|exchangeRate|number(double)|false|none|Tipo de cambio dolares a soles|
|description|string|false|none|Detalles de la orden.|
|merchant|[Merchant](#schemamerchant)|false|none|none|
|currency|[Currency](#schemacurrency)|false|none|none|
|sender|[Sender](#schemasender)|false|none|none|
|beneficiary|[Beneficiary](#schemabeneficiary)|false|none|none|
|depositInformation|[DepositInformation](#schemadepositinformation)|false|none|none|
|channel|string|false|none|Canal para el abono.|

#### Enumerated Values

|Property|Value|
|---|---|
|channel|ACCOUNT|
|channel|PHONE|
|channel|COUNTER|

<h2 id="tocS_Agency">Agency</h2>

<a id="schemaagency"></a>
<a id="schema_Agency"></a>
<a id="tocSagency"></a>
<a id="tocsagency"></a>

```json
{
  "title": "Agency",
  "type": "object",
  "properties": {
    "agencyId": {
      "type": "string",
      "description": "Código de agencia",
      "example": "000"
    }
  }
}

```

Agency

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|agencyId|string|false|none|Código de agencia|

<h2 id="tocS_Branch">Branch</h2>

<a id="schemabranch"></a>
<a id="schema_Branch"></a>
<a id="tocSbranch"></a>
<a id="tocsbranch"></a>

```json
{
  "title": "Branch",
  "type": "object",
  "properties": {
    "branchOfficeId": {
      "type": "string",
      "description": "Código de sucursal ",
      "example": "193"
    }
  }
}

```

Branch

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|branchOfficeId|string|false|none|Código de sucursal|

<h2 id="tocS_Status">Status</h2>

<a id="schemastatus"></a>
<a id="schema_Status"></a>
<a id="tocSstatus"></a>
<a id="tocsstatus"></a>

```json
{
  "title": "Status",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Estado de la Remesa ",
      "example": "ABONADO"
    },
    "description": {
      "type": "string",
      "description": "Descripción del estado de la Remesa ",
      "example": "Remesa disponible"
    }
  }
}

```

Status

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Estado de la Remesa|
|description|string|false|none|Descripción del estado de la Remesa|

<h2 id="tocS_BeneficiarySearchResponse">BeneficiarySearchResponse</h2>

<a id="schemabeneficiarysearchresponse"></a>
<a id="schema_BeneficiarySearchResponse"></a>
<a id="tocSbeneficiarysearchresponse"></a>
<a id="tocsbeneficiarysearchresponse"></a>

```json
{
  "title": "BeneficiarySearchResponse",
  "type": "object",
  "properties": {
    "beneficiaryId": {
      "type": "string",
      "description": "Doc. De identidad.",
      "example": "154852154"
    },
    "fullName": {
      "type": "string",
      "description": "Nombre y apellidos completos del beneficiario.",
      "example": "Pablo Orladini Cevallos"
    }
  }
}

```

BeneficiarySearchResponse

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|beneficiaryId|string|false|none|Doc. De identidad.|
|fullName|string|false|none|Nombre y apellidos completos del beneficiario.|

<h2 id="tocS_ApiException">ApiException</h2>

<a id="schemaapiexception"></a>
<a id="schema_ApiException"></a>
<a id="tocSapiexception"></a>
<a id="tocsapiexception"></a>

```json
{
  "title": "ApiException",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Codigo de error de Sistema",
      "example": "TL0001"
    },
    "description": {
      "type": "string",
      "description": "Descripcion del error de Sistema",
      "example": "Error al llamar al servicio"
    },
    "errorType": {
      "type": "string",
      "description": "Tipo de Error de Sistema",
      "example": "TECHNICAL"
    },
    "exceptionDetails": {
      "type": "array",
      "description": "Lista de detalles del error",
      "items": {
        "title": "ApiExceptionDetail",
        "type": "object",
        "properties": {
          "code": {
            "type": "string",
            "description": "Codigo de error del Detalle/Proveedor",
            "example": "MB0008"
          },
          "component": {
            "type": "string",
            "description": "Nombre del componente de falla",
            "example": "MB.CardInqV2"
          },
          "description": {
            "type": "string",
            "description": "Descripcion del Detalle",
            "example": "Codigo invalido para el canal"
          }
        },
        "description": "Datos del error técnico."
      }
    },
    "properties": {
      "type": "object",
      "properties": {},
      "description": "Lista de propiedades especiales."
    }
  },
  "description": "Datos del error de sistema."
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
  "title": "ApiExceptionDetail",
  "type": "object",
  "properties": {
    "code": {
      "type": "string",
      "description": "Codigo de error del Detalle/Proveedor",
      "example": "MB0008"
    },
    "component": {
      "type": "string",
      "description": "Nombre del componente de falla",
      "example": "MB.CardInqV2"
    },
    "description": {
      "type": "string",
      "description": "Descripcion del Detalle",
      "example": "Codigo invalido para el canal"
    }
  },
  "description": "Datos del error técnico."
}

```

ApiExceptionDetail

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|code|string|false|none|Codigo de error del Detalle/Proveedor|
|component|string|false|none|Nombre del componente de falla|
|description|string|false|none|Descripcion del Detalle|

<h2 id="tocS_RemittanceOrderSearchResponse">RemittanceOrderSearchResponse</h2>

<a id="schemaremittanceordersearchresponse"></a>
<a id="schema_RemittanceOrderSearchResponse"></a>
<a id="tocSremittanceordersearchresponse"></a>
<a id="tocsremittanceordersearchresponse"></a>

```json
{
  "title": "RemittanceOrderSearchResponse",
  "type": "object",
  "properties": {
    "remittanceOrderId": {
      "type": "string",
      "description": "Número Interno de la Operación en Remittance",
      "example": "9372834.0"
    },
    "registerDate": {
      "type": "string",
      "description": "Fecha y Hora de la operación",
      "example": "2019-10-20|19:00:00"
    },
    "status": {
      "title": "Status",
      "type": "object",
      "properties": {
        "code": {
          "type": "string",
          "description": "Estado de la Remesa ",
          "example": "ABONADO"
        },
        "description": {
          "type": "string",
          "description": "Descripción del estado de la Remesa ",
          "example": "Remesa disponible"
        }
      }
    },
    "beneficiary": {
      "title": "BeneficiarySearchResponse",
      "type": "object",
      "properties": {
        "beneficiaryId": {
          "type": "string",
          "description": "Doc. De identidad.",
          "example": "154852154"
        },
        "fullName": {
          "type": "string",
          "description": "Nombre y apellidos completos del beneficiario.",
          "example": "Pablo Orladini Cevallos"
        }
      }
    },
    "branch": {
      "title": "Branch",
      "type": "object",
      "properties": {
        "branchOfficeId": {
          "type": "string",
          "description": "Código de sucursal ",
          "example": "193"
        }
      }
    },
    "agency": {
      "title": "Agency",
      "type": "object",
      "properties": {
        "agencyId": {
          "type": "string",
          "description": "Código de agencia",
          "example": "000"
        }
      }
    },
    "terminalId": {
      "type": "string",
      "description": "Terminal",
      "example": "H984649"
    },
    "referenceSource": {
      "type": "string",
      "description": "Nombre del Canal",
      "example": "AGENTE"
    }
  }
}

```

RemittanceOrderSearchResponse

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|remittanceOrderId|string|false|none|Número Interno de la Operación en Remittance|
|registerDate|string|false|none|Fecha y Hora de la operación|
|status|[Status](#schemastatus)|false|none|none|
|beneficiary|[BeneficiarySearchResponse](#schemabeneficiarysearchresponse)|false|none|none|
|branch|[Branch](#schemabranch)|false|none|none|
|agency|[Agency](#schemaagency)|false|none|none|
|terminalId|string|false|none|Terminal|
|referenceSource|string|false|none|Nombre del Canal|

<h2 id="tocS_RemittanceOrderSearchExchangeRate">RemittanceOrderSearchExchangeRate</h2>

<a id="schemaremittanceordersearchexchangerate"></a>
<a id="schema_RemittanceOrderSearchExchangeRate"></a>
<a id="tocSremittanceordersearchexchangerate"></a>
<a id="tocsremittanceordersearchexchangerate"></a>

```json
{
  "type": "object",
  "properties": {
    "remittanceExchangeRate": {
      "type": "string",
      "description": "Número tipo cambio pizarra",
      "example": "3.71"
    }
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|remittanceExchangeRate|string|false|none|Número tipo cambio pizarra|

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

[](#portal-de-apis)

## ➤ Portal de APIs
El API se encuentra en el Portafolio de APIs en el siguiente link https://www.portalapisbcp.com/#/api-detail/_ID-PORTAL_

[](#diagramas-de-arquitectura)

## ➤ Diagramas de arquitectura


![Diagrama](/assets/images/diagrama.svg)

[](#deuda-tecnica)

## ➤ Deuda tecnica

[](#deuda-tecnica)

## ➤ Deuda tecnica

Este documento describe la deuda técnica identificada en el archivo `openapi.yaml`. La deuda técnica en un archivo OpenAPI puede tener un impacto significativo en la calidad de la documentación, el desarrollo de los servicios, y la integración con sistemas externos.

---


[](#1-estructura-general)

## ➤ **1. Estructura General**
### Problemas:
- **Inconsistencia en los esquemas de datos**:
  - Algunos modelos tienen propiedades no documentadas.
  - Faltan descripciones en varios parámetros.
- **Falta de organización en los endpoints**:
  - No hay una agrupación lógica de los recursos por contexto o dominio.

### Soluciones:
- Realizar una auditoría completa de los esquemas y agregar descripciones a todas las propiedades.
- Agrupar los endpoints en categorías más claras para mejorar la legibilidad.

---


[](#2-falta-de-descripciones-detalladas)

## ➤ **2. Falta de Descripciones Detalladas**
### Problemas:
- Muchos endpoints carecen de descripciones completas que expliquen el propósito y uso del recurso.
- Los códigos de respuesta HTTP no están documentados adecuadamente.

### Soluciones:
- Agregar descripciones detalladas a cada endpoint, método y código de respuesta.
- Utilizar ejemplos en los campos de respuesta y solicitud para proporcionar claridad adicional.

---


[](#3-inconsistencias-en-los-tipos-de-datos)

## ➤ **3. Inconsistencias en los Tipos de Datos**
### Problemas:
- Varias propiedades usan tipos genéricos como `string` cuando podrían ser más específicos (e.g., `date-time`, `integer`).
- Falta de validación en propiedades clave, como `minLength`, `maxLength` o `pattern`.

### Soluciones:
- Actualizar los tipos de datos para reflejar mejor los valores esperados.
- Implementar restricciones de validación para mejorar la robustez de los modelos.

---


[](#4-falta-de-versionamiento)

## ➤ **4. Falta de Versionamiento**
### Problemas:
- No se indica una versión en el archivo OpenAPI.
- Dificulta la gestión de cambios en la API a lo largo del tiempo.

### Soluciones:
- Agregar un campo `version` en la raíz del archivo OpenAPI.
- Implementar estrategias de versionamiento, como `/v1`, `/v2`, en los endpoints.

---


[](#5-cdigos-de-error-y-respuestas)

## ➤ **5. Códigos de Error y Respuestas**
### Problemas:
- Respuestas genéricas sin detalles sobre los posibles errores.
- No hay una lista consolidada de códigos de error.

### Soluciones:
- Crear una sección para documentar todos los códigos de error posibles.
- Agregar ejemplos de respuestas de error con mensajes claros.

---


[](#6-seguridad)

## ➤ **6. Seguridad**
### Problemas:
- Falta de definición de esquemas de autenticación (e.g., OAuth, API Key).
- No se detallan los scopes para los recursos protegidos.

### Soluciones:
- Agregar un esquema de seguridad en el archivo OpenAPI.
- Documentar los scopes necesarios para cada endpoint.

---


[](#7-herramientas-y-generacin-automtica)

## ➤ **7. Herramientas y Generación Automática**
### Problemas:
- No se utiliza una herramienta para validar automáticamente el archivo OpenAPI.
- El archivo no está optimizado para la generación de SDKs o clientes.

### Soluciones:
- Usar herramientas como [Swagger Validator](https://validator.swagger.io/) para validar la especificación.
- Refactorizar el archivo para mejorar su compatibilidad con generadores automáticos de clientes (e.g., Swagger Codegen, OpenAPI Generator).

---


[](#8-testing)

## ➤ **8. Testing**
### Problemas:
- Falta de integración entre el archivo OpenAPI y los tests automatizados.
- No hay contratos claros para los equipos de desarrollo y QA.

### Soluciones:
- Implementar pruebas de contrato utilizando herramientas como Postman o Newman.
- Asegurar que el archivo OpenAPI esté sincronizado con los tests de la API.

---


[](#conclusin)

## ➤ **Conclusión**
La deuda técnica en un archivo OpenAPI puede limitar su utilidad y la capacidad de escalar. Es crucial abordar estas áreas para mejorar la claridad, la robustez y la mantenibilidad de la especificación. Un archivo OpenAPI bien documentado y estructurado es fundamental para garantizar un desarrollo eficiente y una experiencia óptima para los consumidores de la API.
