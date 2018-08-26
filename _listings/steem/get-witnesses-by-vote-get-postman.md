{
  "info": {
    "name": "Steem get_witnesses_by_vote",
    "_postman_id": "a9e14fdd-4a65-49ea-8b36-1270ab6508b4",
    "description": "get_witnesses_by_vote",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "56153e91-3c05-4607-a85a-5c594cb7f270",
          "name": "get-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses?witnessIds=%7B%7D",
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
            "description": "get_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "325bdd6d-75e7-4578-bfa6-7a3e086467df"
            }
          ]
        },
        {
          "id": "587fb1d9-bf25-49c6-8aed-102249ab9105",
          "name": "get-witnesses-by-vote",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses_by_vote?from=%7B%7D&limit=%7B%7D",
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
            "description": "get_witnesses_by_vote"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d547e81-8a6a-41ac-a757-7affe9c8790c"
            }
          ]
        }
      ]
    }
  ]
}