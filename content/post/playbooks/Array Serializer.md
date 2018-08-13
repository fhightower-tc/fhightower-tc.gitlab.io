

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "Json Path 1" app
- **body:** used in the "Find and Replace 1" app
- **queryparam:** used in the "Value Lookup 1" app
- **body:** used in the "Logger 1" app

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **triggerForThisPlaybook:** `https://sandbox.threatconnect.com/api/playbook/402b2179-b9a1-4085-9e6b-2604fb015b3d`
- **errorMessage:** `Request to #App:14487:link!String failed: #App:14488:http.status_code!String . Make sure this link is correct and that the playbook related to this link is turned on.`
- **errorMessage:** `Request to #App:14482:triggerForThisPlaybook!String failed: #App:14486:http.status_code!String . Make sure this link is correct (it should be the trigger link for this playbook).`
