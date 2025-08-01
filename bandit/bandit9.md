# Bandit Level 8 → Level 9

## Level goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Commands used

cat ./~ | sort | uniq -c

| sort: reading sorted content
| uniq: reading without duplications
-c: reading frequency of the duplications

## Codes
```
bandit8@bandit:~$ ls -al
total 56
drwxr-xr-x   2 root    root     4096 Jul 28 19:04 .
drwxr-xr-x 150 root    root     4096 Jul 28 19:06 ..
-rw-r--r--   1 root    root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root    root     3851 Jul 28 18:47 .bashrc
-rw-r-----   1 bandit9 bandit8 33033 Jul 28 19:04 data.txt
-rw-r--r--   1 root    root      807 Mar 31  2024 .profile
andit8@bandit:~$ cat ./data.txt | sort | uniq -c
     10 066lBi8GrHITCQmvVAgMOdGGXrXhYmmO
     10 1nd1ZEdrz8EVgTAhESS7YsDyI1E4PtOc
     10 20XnpTGhJBb02GfFqE4sjppp3x8Blgm9
     10 25FT2cKAXqhJMyu8cqM2pbf5FYY7gN94
     10 267mL9kWCxYUXxhys9LQRHczQ89P5YW7
     10 2PtTb4F4paPri3QZTfKmYOAxhKZpUIxG
     10 3BgiHoJavqX59KpAIzjiagq0m7F6ydUf
     10 3PQlZY41x29QXhn0gjPVY8yWD6zN5WdV
     10 3w7lF0V81O3pHyjJAPiFOSMWxTGGFTzX
      1 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
     10 4DxVWvawXAV8a5CK3Wm9yGmAxO6BLvk6
     10 53fOHmS11iKcejxYjdFxOZgiHJqp9T0v
     10 5AwD5xDyAjxHdDXJ7Gyf2g6zFYfPHefT
     10 5HmULkMNHOXr1xH6RCkEAvCaQP2g29k7
     10 5MdKmCVlBnk2d9SCYffmScP88lKrkyc1
     10 6JZcaNjEmxR14s8fZDEJjVwGVHD7lFI1
     10 7YpPFQoUC7HyBcFxsXcT0d2obrHoNd0G
     10 8Hk7k1njsVs3b1rPIAEwAAKcbxcPss6D
     10 8TR2DGBoyR0qpcHNG5jWzAQXlxsBehzY
     10 9DY2Gf2qK4qWjccH9wVo69b7cQ5GkftZ
     10 9SttX3md6zNW7ICpFrTIbN9jZMFnvCaL
     10 9y4uRoVWgUs5ZXuDSoS7aMqoR5hoBDgD
     10 A8JkVr1ZzrVD9CRVw87FjMYdYF4ImKU7
     10 AajWJYFT9ez1VHiiZuStKbndQypKtP9X
     10 AXlj0FbR9MNzWo3NMAH5e7csP52E8fhn
     10 bjJbZPaXFdSRHaFQtirngDKrFsCTxk9T
     10 bx7wP9t2ntFb0X9JndpIs43AOboyayzV
     10 C2N3mxjm6ONkR8F5RXMOgKnCx77dkuL5
     10 doMcY7qNOloZl01DLVsWpWGbjfa0kyBR
     10 E1wLzPiqSrUHXw1C2Bl6HQd8XXx6Jvfo
     10 eDSrVcOppYCFEXTxo15nhrBeo4nP9rwR
     10 eu8piYivriPNyAvyV9Xoi0Cj1oMnMuMd
     10 fqTSWDqrpl6Q7mOX1rQoDZfBeQ9SXJmB
     10 fYfAGsObkfXoqaEVSA9ID1BPmfaM69Bj
     10 fZKMhplhLfUqK9IWSVoYRRe8OjiLTqNu
     10 G495trqJ23E6mHetfFB2pnE79O1LJJTC
     10 geVQgqRTOsCVnmlVDOUajHUtZcySRHBz
     10 GycpMb3cVTZqXYmyi8qL9fXNM87yuR9W
     10 HNvz2OnwwbEBHqucx45hExsoeBPuNuRE
     10 HRtmLAceOrjNzn9UUQvwkQuSSSGUas1G
     10 HzlrgP2RRR09y328QxmuOCsTBuEQb73l
     10 i18t9nzEDRskKOG0BozSjROHxINZb2Nc
     10 I3NYAtIBEMQvfbeKiZ05OhhqyTv2RjRM
     10 ii39r81X6y1DvRQpfG52I2v7dkmwF3Le
     10 IjZAd9BYAlcTV1wHPYoU8bXAUylJccUE
     10 IOGgcr9BAB0Safu2kZq0yDiC9QmS0xKv
     10 Iw4JIVVJX38LgWp3fVzkUorLPkhcqM3d
     10 JEgVfmJ84eDcR9UntG0lJWY3PGUkehr0
     10 jHEFEdOrsKHUijfhipvktNDfcFDqiXWu
     10 JjSOzziUVAs6HIPOdrthXrwz8d0E0ebH
     10 kq3h7Xh7tMvdSBxHTno0Irdsjl3to0bT
     10 KQufzUBpuGFEDjCmCsbtO7sYDRSdV9Df
     10 kRVDHIhJBu13LGQdWsVdzomORSSZ3oR3
     10 LciQNDsIKGjNiDt82UMrgRTCOVXN64qz
     10 lWewCujU8r1DbzjFyWDdwTOjIkDO5fll
     10 m1GO4enhmpKPd0D62ao9rWnnO7zEb02i
     10 M5nNu2Sfdq1IiGapChKtgIQwjmx4bbDg
     10 MlQdBdzYgXYjvVLTbf6qmLqgIkDsjjKy
     10 N4PR1dYxHIGNixiOqR8vpszJ6N49FbNS
     10 NnaKhCmKdQtfzDIAH46EZLybMXEEP6eS
     10 NNh2GspZ1ah71G9aL2lMSQAxrnNP9YGP
     10 NSNcI7e4lZAQ1yjlUo75jwm7LL6uLlOZ
     10 nvXl8TKrN9KITfB3pLhLwDhJN5WxZwW5
     10 o1YkQCqOImdLFJltX8u8Do41KKz5Zuw3
     10 oM9itQAoBzjECcgjiEZEe6LRRaNS0F74
     10 pDRJDcEsj2kKAsIloqj5IsLu03WoONks
     10 PegfBPLTL0s34wmbFKHgvtxFlg1Zya9X
     10 pGn9cE76plMmRbiUzU1i8g1syq1KBguj
     10 ph97K1tAYF8M9qFocCtcf3LO42Vfx5Mg
     10 PimRmvbk118SkZVwYX0gYGMqX3INJg9N
     10 PnAQqLCsdxln9EQTFq71SsfQoIMYEEwi
     10 R2BvXLsu7CqrtxM4lMJWopIMcQe2047i
     10 r9fBFHH41cMCOBt7J0FzTMu6qhmyg1ju
     10 RUs2Okiu4bGLq6HxnBGv9IZxAQVC9l60
     10 sEXslgWis0Suwriod0dNxIWqSmnqAOUM
     10 SGtTJSj4kHd5erHCXFzXvjovoo3WmLIW
     10 Tu5a1R96ai8FxKeWNlW1tIX6UivhxpEj
     10 ULDVyjUg855EaXgTTYxvBukYz8DBF38b
     10 UxjrID9PjOVAnuRHt0z7jwsqH3aAuZy0
     10 vG39S3TGEOoISRtKfW5xrA0W7P3ZTLyD
     10 vHNAonNEx718zpVQdC4WdCnpPJ8dS7FT
     10 VYlunIwjTif5D2XI4IsZepOO0spVRPed
     10 wBfRTfExtsDGa97WfMGYhKM8U2ILGRUO
     10 wlghJurXHGBgTOAo356YtAI1LWSMNU8B
     10 WNbqCnVMsILfKr8txYpqjLgVuz366ItL
     10 xPT4qs1lMe4klHPWKAwadx7bFPlMfJjk
     10 Xu9ndxMWUj399FjOm8vnUIHRefkcZTm6
     10 XufULFiOZWAHsAxw0bIUQGrZZFyBRlZL
     10 xvzd4OuwULNXOeO5vdEmANd79ZfH1m3N
     10 xX8oppP2KrmOxChaKTYTeLX8UcT6nMy6
     10 y2RjNkRsECKdnVbfIjtJhXeQD4zzD0GQ
     10 Y7dk31MFwgvGjktCYp5WYUb0jNdW5q0m
     10 Y9lurOacbjhKLxFrcydP5Q1Sa8rg5y1d
     10 yTUoZZUAb9Ch4diXoeOY2O8Lpnjkvaa3
     10 Yuqk70e0QW8aQEaKeL5txWEu5rH9wrYZ
     10 Z3MUMFcijOnqv6AGX5WwpvskxnUP1lMr
     10 zglHBytS12CgnJagxIaAPiONayRUoPit
     10 ZhFnLbKximlzN3fxwn9FyCe95jQfP59p
     10 ZIzWAFrqO0tReQ07ZzWMpRrAnWLfldEj
     10 ZO25yUpC8UtUCb00m8nV0IOd8jAMVbKG
     10 Zv7u476GCUK7sALpeoPeq3fzbua4a84I
