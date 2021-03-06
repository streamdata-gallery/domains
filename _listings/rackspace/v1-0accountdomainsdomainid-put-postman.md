{
  "info": {
    "name": "Rackspace Update domain",
    "_postman_id": "a32a0da2-f204-4420-868e-3afad6c967c1",
    "description": "NoteThis call returns an asynchronous response. Refer to\nSynchronous and asynchronous responses\nfor more details and examples of the way that asynchronous responses work.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Limits",
      "item": [
        {
          "id": "71c7aa5a-01b1-4fd7-a610-659156990d2d",
          "name": "list-limits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limits for a specified account.The following examples show the requests and corresponding responses to list\nall limits for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8047fb7-a55f-4727-80c9-db71cdca4e4f"
            }
          ]
        },
        {
          "id": "e08cb8e9-fc03-4ed7-a552-f303b0b9ef49",
          "name": "show-limits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits/:type\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limits of a specified type for\nthe specified account.The following examples show the requests and corresponding responses to list\nall applicable limits of a specified type for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0ed056e-7635-4975-a8e4-dc2c7a5c90c0"
            }
          ]
        },
        {
          "id": "59baac64-5ffb-4ec9-bc79-872162641c15",
          "name": "list-limit-types",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits/types\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limit types for a specified account.The following examples show the requests and corresponding responses to list\nall limit types for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b86a0ac6-49bf-4736-991c-af1fb0335595"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "cc9fec49-22af-415b-a13b-1b961e32c3ff",
          "name": "list-domains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "These calls provide a list of all DNS domains manageable by a given account.\nThe resulting list is flat, and does not break the domains down hierarchically\nby subdomain. All representative domains are included in the list, even if a\ndomain is conceptually a subdomain of another domain in the list.Note"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fdd68d1-ee99-4b9f-b210-feeca3723e14"
            }
          ]
        },
        {
          "id": "9a3605fd-72df-4252-a224-7492e2051eed",
          "name": "update-domains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis call returns an asynchronous response, as described in\nSynchronous and asynchronous responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79cbac93-84e7-44ef-9142-6659af2711fd"
            }
          ]
        },
        {
          "id": "dc4aa41a-02f1-470d-add0-b738c77a0869",
          "name": "create-domain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis call returns an asynchronous response, See\nSynchronous and asynchronous responses\nfor more details and examples of the way that asynchronous responses work."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9e70f9c-acc9-451e-b90c-0e3c3f182005"
            }
          ]
        },
        {
          "id": "b0980054-7afc-4e8b-9af3-3f585a53be6f",
          "name": "delete-domains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis call returns an asynchronous response, as described in\nSynchronous and asynchronous responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fed26a24-3814-4e6e-adec-7862b84bb509"
            }
          ]
        },
        {
          "id": "8915a19a-4200-43de-875a-f1496ddcc0cf",
          "name": "search-domains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains/search\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "NoteFilter criteria may consist of:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a1ab191-063c-4865-b43e-5f6c54586608"
            }
          ]
        },
        {
          "id": "d095ac30-f6be-46b7-b6c6-3e6132fb3fba",
          "name": "list-domain-details-without-subdomains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains/:domainId\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "domainId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides the detailed output for a specified domain configured and\nassociated with an account. This call is not capable of returning details for a\ndomain that has been deleted.This call does not require a request body."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d829ed6c-9bf9-4297-8e9a-ef13b64eff0f"
            }
          ]
        },
        {
          "id": "12ef1682-fa9f-4d74-b7d7-c9f379deb868",
          "name": "update-domain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains/:domainId\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "domainId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis call returns an asynchronous response. Refer to\nSynchronous and asynchronous responses\nfor more details and examples of the way that asynchronous responses work."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d876cd48-24ce-414b-bd78-7be7aff711ba"
            }
          ]
        }
      ]
    }
  ]
}