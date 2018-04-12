# User Object

## Data Fields

| field name | field type | description |
|--------|---------|-------|
| user_name | string | The name of the user that executed the action in the event |
| user_domain | string | The name of the domain the user that executed the action in the event belongs to |
| user_logon_id | integer | Logon ID of the user that executed the action in the event |
| user_sid | integer | SID of user that executed the action in the event |
| user_terminal_session_id | string | Session ID. Usually 0 for system and 1 for the first interactive session |
| user_reporter_name | string | The name of the user that reported the event |
| user_reporter_domain | string | The name of the domain the user that reported the event belongs to |
| user_reporter_logon_id | integer | Logon ID of the user that reported the event |
| user_target_name | string | The name of the user being impersonated or called by the main user in the event |
| user_target_domain | string | The name of the user being impersonated or called by the main user in the event belongs to |
| user_target_logon_id | integer | Logon ID of the user being impersonated or called by the main user in the event |