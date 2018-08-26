{
  "info": {
    "name": "Steem get_active_votes",
    "_postman_id": "a88e264d-3c10-4098-9ea6-82556e0e5ed9",
    "description": "get_active_votes",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "926ba797-951d-41e0-9a58-e19497939cf3",
          "name": "get-active-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_active_witnesses",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_active_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99e9b4df-20ac-40fb-92ec-c39155e94ab4"
            }
          ]
        },
        {
          "id": "c67e2cde-6111-4de0-921a-036eb851d902",
          "name": "get-tags",
          "request": {
            "url": "http://api.steemjs.com/get_active_categories?after=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b6e658e-3dff-432b-919c-e1679f1e9bc7"
            }
          ]
        },
        {
          "id": "4fcb7a00-808f-4fe3-b0d5-cdbacf4a7740",
          "name": "get-active-votes",
          "request": {
            "url": "http://api.steemjs.com/get_active_votes?author=%7B%7D&permlink=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_active_votes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8393062-7542-4512-bad5-5570c5d5c8ae"
            }
          ]
        }
      ]
    }
  ]
}