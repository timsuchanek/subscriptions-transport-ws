# Changelog

### vNEXT

- ...

### v0.4.0

- Don't throw in the server on certain unsub messages. 
[PR #54](https://github.com/apollostack/subscriptions-transport-ws/pull/54)
- Moved typings to `@types/graphql`.
[PR #60](https://github.com/apollostack/subscriptions-transport-ws/pull/60)

### v0.3.1

- Server now passes back subscriptionManager errors encountered during publish.
[PR #42](https://github.com/apollostack/subscriptions-transport-ws/pull/42)

### v0.3.0

- (SEMVER-MINOR) Bump graphql-subscriptions dependency to ^0.2.0 which changes the setupFunctions format
- Fix missing unsubscription from first (id = 0) subscription

### v0.2.6

- Add `reconnect` and `reconnectionAttempts` options to the constructor which will enable reconnection with exponential backoff.

### v0.2.5

- Pass WebSocketRequest to onSubscribe to support reading HTTP headers when creating a subscription

### v0.2.4

- Server reports back an error on an unparsable client message
- Server reports back an error on an unsupported client message type
- Fix intermittent failure in timeout test case
- Standardize server and client errors handling to always create an array of errors with a message property
