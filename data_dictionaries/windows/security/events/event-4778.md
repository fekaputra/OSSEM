# Event ID 4778: A session was reconnected to a Window Station

## Description

This event is generated when a user reconnects to an existing Terminal Services session, or when a user switches to an existing desktop using Fast User Switching.

* This event also generates when user reconnects to virtual host Hyper-V Enhanced Session, for example.

[MS Source](https://github.com/MicrosoftDocs/windows-itpro-docs/blob/master/windows/security/threat-protection/auditing/event-4778.md)

## Event Log Illustration & Event XML

[MS Source](https://github.com/MicrosoftDocs/windows-itpro-docs/blob/master/windows/security/threat-protection/auditing/event-4778.md)

## Data Dictionary

|	Standard Name	| Field Name |	Type	|	Description	|	Sample Value	|
|	----------------	|	----------------	|	----------------	|	----------------	|	----------------	|
|	user_name	|	AccountName	|	string	|	the name of the account for which the session was reconnected	|	ladmin	|
|	user_domain	|	AccountDomain	|	string	|	subject’s domain or computer name	|	CONTOSO	|
|	user_logon_id	|	LogonID	|	integer	|	hexadecimal value that can help you correlate this event with recent events that might contain the same Logon ID	|	0x1e01f6	|
|	session_name	|	SessionName	|	string	|	the name of the session to which the user was reconnected	|	RDP-Tcp\#6	|
|	src_host_name	|	ClientName	|	string	|	computer name from which the user was reconnected. Has “Unknown” value for console session.	|	WIN81	|
|	src_ip_addr	|	ClientAddress	|	ip	|	IP address of the computer from which the user was reconnected	|	10.0.0.100	|