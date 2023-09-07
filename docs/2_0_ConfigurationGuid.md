### Environment Variables
| Variable                 | Type | What it does                                                |NOTES|
| ------------------------ | ---- | ---------------------------------------------- |-|
| SET_NON_REVOKED          | bool | if True, the `non_revoked` attributed  will be added to each of the present-proof request `requested_attribute` and `requested_predicate` with 'from=0' and'to=`int(time.time())`||
| USE_OOB_PRESENT_PROOF    | bool | if True, the present-proof request will be provided as a an [out of band](https://github.com/hyperledger/aries-rfcs/tree/main/features/0434-outofband) invitation with a [present-proof](https://github.com/hyperledger/aries-rfcs/tree/main/features/0037-present-proof) request inside. If False, the present-proof request will be use the [service-decorator](https://github.com/hyperledger/aries-rfcs/tree/main/features/0056-service-decorator)|**TRUE:** BC Wallet supports our OOB Message with a minor glitch, BiFold, Lissi, Trinsic, and Estatus all read the QR code as 'Invalid' **FALSE:** Works with|
| LOG_WITH_JSON            | bool | If True, logging output should printed as JSON if False it will be pretty printed.| Default behavior will print as JSON. |
| LOG_TIMESTAMP_FORMAT     | string | determines the timestamp formatting used in logs | Default is "iso" |
| LOG_LEVEL                | "DEBUG", "INFO", "WARNING", or "ERROR" | sets the minimum log level that will be printed to standard out| Defaults to DEBUG |
