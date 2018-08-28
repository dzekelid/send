{
  "info": {
    "name": "AWS Simple Notification Service API Publish",
    "_postman_id": "55b664ce-bbc7-430a-94f0-1f4bcee833ba",
    "description": "Sends a message to all of a topic's subscribed endpoints.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "0d2390cf-12ee-43f8-a14b-20303792d0a8",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.member.N=ActionName.member.N&AWSAccountId.member.N=AWSAccountId.member.N&Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a statement to a topic's access control policy, granting access for the specified AWS accounts to the specified actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e69e4d9-272e-4a42-96df-3b8275f1915e"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "099112b1-407c-4c8f-bf7b-de2a499c3534",
          "name": "checkIfPhoneNumberIsOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=CheckIfPhoneNumberIsOptedOut?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7869869-c51c-4dcd-94a9-5814041d509d"
            }
          ]
        },
        {
          "id": "f76ad0e4-6e24-4fd5-85af-12ede71e154f",
          "name": "listPhoneNumbersOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=ListPhoneNumbersOptedOut?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddcb74fe-6965-4a14-906f-6a187b363a9b"
            }
          ]
        },
        {
          "id": "d534562f-7fa1-41fc-ab11-cf516598ad3c",
          "name": "optInPhoneNumber",
          "request": {
            "url": "http://example.com/api/?Action=OptInPhoneNumber?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to opt in a phone number that is opted out, which enables you to resume sending SMS messages to the number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a46ddf28-1256-4955-ad03-fc0f336c42cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "4c495644-aff6-4a6d-9937-8c5b27e071b7",
          "name": "confirmSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSubscription?AuthenticateOnUnsubscribe=AuthenticateOnUnsubscribe&Token=Token&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an endpoint owner's intent to receive messages by validating the token sent to the\n      endpoint by an earlier Subscribe action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75819e7d-0a75-4226-9fb0-af524bd6ad8a"
            }
          ]
        },
        {
          "id": "b5aaf2c2-2b15-4202-aa3c-e4ec7c89d1b3",
          "name": "getSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSubscriptionAttributes?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78f7e85e-282a-42e9-9816-b6272ae052a2"
            }
          ]
        },
        {
          "id": "8af1653e-9623-4dd9-999a-f19edf51ac2c",
          "name": "listSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptions?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "438b0837-7bdd-4489-a92b-3d2e861d077b"
            }
          ]
        },
        {
          "id": "967475af-ccdc-40bd-a32f-f8be6e427ab7",
          "name": "listSubscriptionsByTopic",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptionsByTopic?NextToken=NextToken&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the subscriptions to a specific topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ff9771a-0193-4354-8ade-4e95f4ec201f"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "c83408f4-c174-4c90-a4b4-76370eb3257b",
          "name": "createPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformApplication?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&Name=Name&Platform=Platform",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a platform application object for one of the supported push notification services,\n      such as APNS and GCM, to which devices and mobile apps may register."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9c8b019-e8b5-4c54-ac61-59337498b46b"
            }
          ]
        },
        {
          "id": "df10116a-25ec-4fb1-b40b-0f058b3cdfa3",
          "name": "deletePlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeletePlatformApplication?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a platform application object for one of the supported push notification services,\n      such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f8364c8-322c-447a-960c-697af7051298"
            }
          ]
        },
        {
          "id": "a8d62e14-6092-4550-860a-21ccf35a2d7c",
          "name": "getPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetPlatformApplicationAttributes?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attributes of the platform application object for the supported push\n      notification services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbd6beb5-86fd-4e58-891a-0e9f2eb2cdb2"
            }
          ]
        },
        {
          "id": "05c2a5b4-d860-4e28-9d7d-0226e89bec3e",
          "name": "listPlatformApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListPlatformApplications?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the platform application objects for the supported push notification services, such as\n      APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb991b98-183c-4dc2-bcaa-4cce08caffd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "bcd85dce-8ce9-4f1e-adc2-686cfd7988d5",
          "name": "createPlatformEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformEndpoint?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&CustomUserData=CustomUserData&PlatformApplicationArn=PlatformApplicationArn&Token=Token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint for a device and mobile app on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f570b54e-54db-4379-8b6f-55f5e35e9a60"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "68ab4f17-5e50-4c3c-82bb-cc6228475371",
          "name": "createTopic",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopic?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a topic to which notifications can be published."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad69f753-9f80-475b-87ff-73afe623414c"
            }
          ]
        },
        {
          "id": "a321e62b-48e0-40d6-afd3-96bcc7a83590",
          "name": "deleteTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopic?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a topic and all its subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "993db5b7-0957-4e83-88b8-57a4d6b35d24"
            }
          ]
        },
        {
          "id": "0f3b780c-2c49-41ec-9652-be86f9c12c2f",
          "name": "getTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetTopicAttributes?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e830231-05af-4541-817e-4c6e252e70f6"
            }
          ]
        },
        {
          "id": "7a6f1645-c9a3-4f31-bfe8-61d109fb9add",
          "name": "listTopics",
          "request": {
            "url": "http://example.com/api/?Action=ListTopics?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea25272d-cdb4-42a3-ab41-52db5088721a"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "65106264-5c5b-4131-a0eb-cfa35abcce9d",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the endpoint for a device and mobile app from Amazon SNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b95ac1f-c352-4ab9-8241-d852fbabfc0e"
            }
          ]
        },
        {
          "id": "3e8b5894-a143-481c-b79e-60ddde49a13c",
          "name": "getEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetEndpointAttributes?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the endpoint attributes for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ff03bd6-e1c5-44f9-b59c-3f058d62878f"
            }
          ]
        },
        {
          "id": "712997ee-b046-43e8-bcb3-6baec33b2871",
          "name": "listEndpointsByPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=ListEndpointsByPlatformApplication?NextToken=NextToken&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the endpoints and endpoint attributes for devices in a supported push notification\n      service, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa001b83-a4fb-4610-83a0-2b85ce5ab2a4"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "8d855909-d4a8-4d14-bc89-04cf2daf2a24",
          "name": "getSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSMSAttributes?attributes.member.N=attributes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the settings for sending SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31d728b6-5a33-4c5a-9a2d-cde035fde44d"
            }
          ]
        }
      ]
    },
    {
      "name": "Publish",
      "item": [
        {
          "id": "2a515b7e-3134-4abd-862d-ecc0620e9d3c",
          "name": "publish",
          "request": {
            "url": "http://example.com/api/?Action=Publish?Message=Message&MessageAttributes\n            , MessageAttributes.entry.N.Name (key), MessageAttributesentry.N.Value (value)=MessageAttributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20MessageAttributes.entry.N.Name%20%28key%29%2C%20MessageAttributesentry.N.Value%20%28value%29&MessageStructure=MessageStructure&PhoneNumber=PhoneNumber&Subject=Subject&TargetArn=TargetArn&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all of a topic's subscribed endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72c922fd-1fe4-4c80-bdaf-cdd89b0fc350"
            }
          ]
        }
      ]
    }
  ]
}