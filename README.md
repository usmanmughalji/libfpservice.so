By Roker2

## libfpservice.so

Need to change to CMP X1, X0

CMP X1, X0 = 3F 00 00 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                 | Patch place | Patch status (patched or not) |
| :----------------------- | :---------- | :---------------------------- |
| android::notifyClient    | 16F04       | yes                           |
| android::notifyClient    | 16F08       | yes                           |
| android::notifyClient    | 16F0C       | yes                           |
| android::notifyClient    | 16F14       | yes                           |
| android::postData2Client | 1C644       | yes                           |
| android::postData2Client | 1C648       | yes                           |
| android::postData2Client | 1C64C       | yes                           |
| android::postData2Client | 1C654       | yes                           |

2 functions, 8 patch places
