---
description: "Automatically generated file. DO NOT MODIFY"
---

```cli

mgc users mail-folders message-rules create --user-id {user-id} --mail-folder-id {mailFolder-id} --body '{\
    "displayName": "From partner",      \
    "sequence": 2,      \
    "isEnabled": true,          \
    "conditions": {\
        "senderContains": [\
          "adele"       \
        ]\
     },\
     "actions": {\
        "forwardTo": [\
          {\
             "emailAddress": {\
                "name": "Alex Wilbur",\
                "address": "AlexW@contoso.onmicrosoft.com"\
              }\
           }\
        ],\
        "stopProcessingRules": true\
     }    \
}\
\
'

```