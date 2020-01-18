By Roker2

## libfpservice.so

Need to change to CMP X1, X0

CMP X1, X0 = 3F 00 00 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                 | Patch place | Patch status (patched or not) |
| :----------------------- | :---------- | :---------------------------- |
| android::notifyClient    | 1B410       | yes                           |
| android::notifyClient    | 1B414       | yes                           |
| android::notifyClient    | 1B418       | yes                           |
| android::notifyClient    | 1B420       | yes                           |
| android::postData2Client | 1C644       | no                            |
| android::postData2Client | 1C648       | no                            |
| android::postData2Client | 1C64C       | no                            |
| android::postData2Client | 1C654       | no                            |

2 functions, 8 patch places