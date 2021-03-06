# X509 and Certificates Schema

Data about X509 and Certificates. These would commonly be found in TLS/SSL connections, smart card certificates, kerberos requests, code signing of PE's and executables, etc...

This document is a work in progress, but is a foundational start there is included. Specifically the main foundations of certificate information is already in here.

## Data Fields

|       Standard Name      |          Type            |         Description      |      Sample Value        |
|--------------------------|--------------------------|--------------------------|--------------------------|
| certificate_hash_md5 | string | MD5 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `6A255BEBF3DBCD13585538ED47DBAFD7` |
| certificate_hash_sha1 | string | SHA1 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `B0BF5AC2E81BBF597FAD5F349FEEB32CAC449FA2` |
| certificate_hash_sha256 | string | SHA256 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `4668BB2223FFB983A5F1273B9E3D9FA2C5CE4A0F1FB18CA5C1B285762020073C` |
| certificate_issuer | string | Information about the CA that issued the certificate | `CN=neu5ron.local,OU=Admin` |
| certificate_subject | string | Information about the CA that issued the certificate | `CN=natetoken,OU=Admin,DC=neu5ron,DC=local` |
| certificate_serial_number | string | Serial number, this is chosen by the CA (certificate authority) which issued the certificate. Therefore this can relatively be arbritary if the CA does not follow a standard or is malicious. | `5157550` |
| dst_certificate_hash_md5 | string | MD5 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `6A255BEBF3DBCD13585538ED47DBAFD7` |
| dst_certificate_hash_sha1 | string | SHA1 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `B0BF5AC2E81BBF597FAD5F349FEEB32CAC449FA2` |
| dst_certificate_hash_sha256 | string | SHA256 hash representation of the entire, computed, certificate. Also known as fingerprint or thumbprint | `4668BB2223FFB983A5F1273B9E3D9FA2C5CE4A0F1FB18CA5C1B285762020073C` |
| dst_certificate_issuer | string | Information about the CA that issued the certificate | `CN=trcodoretur.4Arentthetifth.viajes,OU=Is.ow pandme,O=Pthemide Fteiosie PSU,L=Nicosia,C=CY` |
| dst_certificate_serial_number | string | Serial number, this is chosen by the CA (certificate authority) which issued the certificate. Therefore this can relatively be arbritary if the CA does not follow a standard or is malicious. | `5157550` |
| dst_certificate_subject | string | Information about the servers certificate itself | `CN=trcodoretur.4Arentthetifth.viajes,OU=Is.ow pandme,O=Pthemide Fteiosie PSU,L=Nicosia,C=CY` |