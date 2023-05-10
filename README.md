# CDPworkshop
Cloudera Data Flow workshop. All the required password will be provided during the workshop


https://18.142.122.96:8443/auth/realms/workshop-asean/protocol/saml/clients/samlclient 

username: workshop0xx
pass: 


##schema registry: 

{
  "name": "syslog",
  "type": "record",
  "namespace": "com.cloudera",
  "fields": [
    {
      "name": "priority",
      "type": "int"
    },
    {
      "name": "severity",
      "type": "int"
    },
    {
      "name": "facility",
      "type": "int"
    },
    {
      "name": "version",
      "type": "int"
    },
    {
      "name": "timestamp",
      "type": "long"
    },
    {
      "name": "hostname",
      "type": "string"
    },
    {
      "name": "body",
      "type": "string"
    },
    {
      "name": "appName",
      "type": "string"
    },
    {
      "name": "procid",
      "type": "string"
    },
    {
      "name": "messageid",
      "type": "string"
    },
    {
      "name": "structuredData",
      "type": {
        "name": "structuredData",
        "type": "record",
        "fields": [
          {
            "name": "SDID",
            "type": {
              "name": "SDID",
              "type": "record",
              "fields": [
                {
                  "name": "eventId",
                  "type": "string"
                },
                {
                  "name": "eventSource",
                  "type": "string"
                },
                {
                  "name": "iut",
                  "type": "string"
                }
              ]
            }
          }
        ]
      }
    }
  ]
}
