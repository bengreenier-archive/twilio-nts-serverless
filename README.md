# twilio-nts (serverless)

A super-light frontend for the [Twilio NTS](https://www.twilio.com/docs/stun-turn) service.

## Why

The Twilio NTS service allows usage of Twilio Infrastructure for STUN/TURN communication over the web. In order to obtain access to the service, a caller must provide their Twilio SID and Authentication key, which can be used to obtain `iceServers` data. Since the SID and Authentication key are secrets, they cannot be included in client applications. Providing some lightweight logic that can be run serverside is one solution to grant client applications access to this data.

## How

Use the [serverless](https://serverless.com/) toolset to deploy the function logic from the `fn` directory of this project. Additional instructions can be found [in the inner README](./fn/README.md).

## License

MIT