# Bandit Level 15 → Level 16

## Level goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

Helpful note: Getting “DONE”, “RENEGOTIATING” or “KEYUPDATE”? Read the “CONNECTED COMMANDS” section in the manpage.

## Commands used

openssl s_client -connect (localhost):(portnumber): connnecting to port using ssl/tls encryption

## Codes
```
bandit15@bandit:~$ openssl s_client -connect 127.0.0.1:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = SnakeOil
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = SnakeOil
verify return:1
---
Certificate chain
 0 s:CN = SnakeOil
   i:CN = SnakeOil
   a:PKEY: rsaEncryption, 4096 (bit); sigalg: RSA-SHA256
   v:NotBefore: Jun 10 03:59:50 2024 GMT; NotAfter: Jun  8 03:59:50 2034 GMT
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIFBzCCAu+gAwIBAgIUBLz7DBxA0IfojaL/WaJzE6Sbz7cwDQYJKoZIhvcNAQEL
BQAwEzERMA8GA1UEAwwIU25ha2VPaWwwHhcNMjQwNjEwMDM1OTUwWhcNMzQwNjA4
MDM1OTUwWjATMREwDwYDVQQDDAhTbmFrZU9pbDCCAiIwDQYJKoZIhvcNAQEBBQAD
ggIPADCCAgoCggIBANI+P5QXm9Bj21FIPsQqbqZRb5XmSZZJYaam7EIJ16Fxedf+
jXAv4d/FVqiEM4BuSNsNMeBMx2Gq0lAfN33h+RMTjRoMb8yBsZsC063MLfXCk4p+
09gtGP7BS6Iy5XdmfY/fPHvA3JDEScdlDDmd6Lsbdwhv93Q8M6POVO9sv4HuS4t/
jEjr+NhE+Bjr/wDbyg7GL71BP1WPZpQnRE4OzoSrt5+bZVLvODWUFwinB0fLaGRk
GmI0r5EUOUd7HpYyoIQbiNlePGfPpHRKnmdXTTEZEoxeWWAaM1VhPGqfrB/Pnca+
vAJX7iBOb3kHinmfVOScsG/YAUR94wSELeY+UlEWJaELVUntrJ5HeRDiTChiVQ++
wnnjNbepaW6shopybUF3XXfhIb4NvwLWpvoKFXVtcVjlOujF0snVvpE+MRT0wacy
tHtjZs7Ao7GYxDz6H8AdBLKJW67uQon37a4MI260ADFMS+2vEAbNSFP+f6ii5mrB
18cY64ZaF6oU8bjGK7BArDx56bRc3WFyuBIGWAFHEuB948BcshXY7baf5jjzPmgz
mq1zdRthQB31MOM2ii6vuTkheAvKfFf+llH4M9SnES4NSF2hj9NnHga9V08wfhYc
x0W6qu+S8HUdVF+V23yTvUNgz4Q+UoGs4sHSDEsIBFqNvInnpUmtNgcR2L5PAgMB
AAGjUzBRMB0GA1UdDgQWBBTPo8kfze4P9EgxNuyk7+xDGFtAYzAfBgNVHSMEGDAW
gBTPo8kfze4P9EgxNuyk7+xDGFtAYzAPBgNVHRMBAf8EBTADAQH/MA0GCSqGSIb3
DQEBCwUAA4ICAQAKHomtmcGqyiLnhziLe97Mq2+Sul5QgYVwfx/KYOXxv2T8ZmcR
Ae9XFhZT4jsAOUDK1OXx9aZgDGJHJLNEVTe9zWv1ONFfNxEBxQgP7hhmDBWdtj6d
taqEW/Jp06X+08BtnYK9NZsvDg2YRcvOHConeMjwvEL7tQK0m+GVyQfLYg6jnrhx
egH+abucTKxabFcWSE+Vk0uJYMqcbXvB4WNKz9vj4V5Hn7/DN4xIjFko+nREw6Oa
/AUFjNnO/FPjap+d68H1LdzMH3PSs+yjGid+6Zx9FCnt9qZydW13Miqg3nDnODXw
+Z682mQFjVlGPCA5ZOQbyMKY4tNazG2n8qy2famQT3+jF8Lb6a4NGbnpeWnLMkIu
jWLWIkA9MlbdNXuajiPNVyYIK9gdoBzbfaKwoOfSsLxEqlf8rio1GGcEV5Hlz5S2
txwI0xdW9MWeGWoiLbZSbRJH4TIBFFtoBG0LoEJi0C+UPwS8CDngJB4TyrZqEld3
rH87W+Et1t/Nepoc/Eoaux9PFp5VPXP+qwQGmhir/hv7OsgBhrkYuhkjxZ8+1uk7
tUWC/XM0mpLoxsq6vVl3AJaJe1ivdA9xLytsuG4iv02Juc593HXYR8yOpow0Eq2T
U5EyeuFg5RXYwAPi7ykw1PW7zAPL4MlonEVz+QXOSx6eyhimp1VZC11SCg==
-----END CERTIFICATE-----
subject=CN = SnakeOil
issuer=CN = SnakeOil
---
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 2103 bytes and written 373 bytes
Verification error: self-signed certificate
---
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 4096 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 18 (self-signed certificate)
---
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: CAB85069500AE7525FF203C1423737466CAA7FAD8D4D93100D40B64D984DAFEE
    Session-ID-ctx: 
    Resumption PSK: E563C6B24A7F6BD73241D7853E7469210E9184D6A27D693259ACEA4F3ED8341D67420F49595DB3E1A26671BB2E962E77
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - 39 7f 7d 4b b0 0c 6e f0-c8 95 e4 ba 4b ca 04 b3   9.}K..n.....K...
    0010 - 66 32 1e ed 62 5c 0b c4-90 3a 52 99 ce 47 64 0d   f2..b\...:R..Gd.
    0020 - 8d 97 85 b9 f8 79 83 cf-a9 9e 48 3f c3 fa b9 27   .....y....H?...'
    0030 - 0b 18 fc c3 5e 6a fa 88-03 0c b3 35 66 ec 87 79   ....^j.....5f..y
    0040 - 24 8d fd b7 34 3f ff c0-5e d1 99 89 93 1a 2e 43   $...4?..^......C
    0050 - d1 b0 12 9a 25 f5 1c 20-84 25 f5 0a 15 2c 16 dc   ....%.. .%...,..
    0060 - 97 2f 95 f2 82 fc 1f 66-4a 27 00 30 49 44 ed 58   ./.....fJ'.0ID.X
    0070 - 46 46 2a 5a fe 8e 7b 35-98 c9 26 ec 4a a0 09 4c   FF*Z..{5..&.J..L
    0080 - 8f ee 6f e9 2f 03 4f e0-ea f0 6a 28 da 03 77 9c   ..o./.O...j(..w.
    0090 - 7b 31 5a 33 bd 05 70 c5-f9 71 39 a5 ec e7 79 81   {1Z3..p..q9...y.
    00a0 - 27 88 e8 9f 4c 65 47 28-a3 f4 8f 1b ab fd ef ec   '...LeG(........
    00b0 - 68 3d 4a 66 59 12 f8 6d-6a 0a 5d 9b 49 d0 c3 3b   h=JfY..mj.].I..;
    00c0 - 97 0a 64 48 fb f8 92 d4-85 f8 8e 03 df 9e 06 d8   ..dH............
    00d0 - fc cf 44 93 19 fc b7 07-2e 07 5b af 8e e2 1b a8   ..D.......[.....

    Start Time: 1754215422
    Timeout   : 7200 (sec)
    Verify return code: 18 (self-signed certificate)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 8BA1ADF9D7C8EB91B404BD90D893895EE6E617E2795191A3A7378BE80F7BCE53
    Session-ID-ctx: 
    Resumption PSK: 7322C773BCE9A51647724D01F1C0DD16ED5ED290CBCC5B1DAB648E8B3F01D70004A0640C3A33AADE77FB677AAE1407B4
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - 39 7f 7d 4b b0 0c 6e f0-c8 95 e4 ba 4b ca 04 b3   9.}K..n.....K...
    0010 - c3 c6 16 5b 0d 0f a1 6d-c1 c2 f9 29 8f 89 fd 90   ...[...m...)....
    0020 - 4f 1b 13 6d 77 a3 c9 aa-ff f2 f0 e8 ae d8 46 74   O..mw.........Ft
    0030 - 16 02 6f 60 ce a4 45 c4-2c 42 e4 5e f0 73 d0 b1   ..o`..E.,B.^.s..
    0040 - f6 3b 17 7b 09 41 b9 2c-dc c1 89 e0 f5 cb 28 66   .;.{.A.,......(f
    0050 - 77 77 bc 7e 63 73 91 3c-81 9e 79 5e b5 ce 3f 5e   ww.~cs.<..y^..?^
    0060 - e4 a4 ed 88 6d f4 db 30-00 f1 81 be b4 b1 d3 da   ....m..0........
    0070 - bb e7 fa d9 92 c7 d4 f6-56 a2 db 73 d1 e5 ca 4f   ........V..s...O
    0080 - f3 80 62 6f 6e 60 fc cc-a6 45 52 cf 8b 10 41 1d   ..bon`...ER...A.
    0090 - 35 41 c6 7d bc 01 7e 63-4b 79 9c cc 09 9f 1b 15   5A.}..~cKy......
    00a0 - c1 94 b3 c6 87 db 7f 43-f9 bd 09 56 01 a4 74 d7   .......C...V..t.
    00b0 - 2f 5a 5a da cd af a2 4d-c7 58 18 49 67 bc 32 f7   /ZZ....M.X.Ig.2.
    00c0 - 7e 1d 20 6f 77 9a 95 87-7e d5 eb f4 25 42 41 87   ~. ow...~...%BA.
    00d0 - 0f b0 df 68 0a a9 44 8d-ff d1 77 5e 8d 3e d0 eb   ...h..D...w^.>..

    Start Time: 1754215422
    Timeout   : 7200 (sec)
    Verify return code: 18 (self-signed certificate)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
Correct!
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

closed
