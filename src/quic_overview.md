# QUIC overview

QUIC is a new, multi-stream, connection based transport protocol that uses UDP protocol under the hood.

All QUIC RFC and drafts are available on [IETF Datatracker].
At this moment there are four RFC and a lot of drafts.
* [RFC 8999] - describes properties of QUIC that are common to all versions of the protocol
* [RFC 9000] - main RFC that describes QUIC protocol
* [RFC 9001] - describes TLS integration with QUIC
* [RFC 9002] - describes QUIC loss detection and congestion control mechanisms

Main features of QUIC:
* integration with TLS - QUIC is by default integrated with TLS 1.3.
Thanks to this the time needed for establishing a connection can be significantly reduced.
On the other hand there is no posibility to send unecrypted data over QUIC at this moment.
* streams - QUIC is a multi-stream protocol.
Stream is an ordered sequence of bytes - it is byte oriented not message oriented.
Each QUIC connection can have multiple streams.
There can be unidirectional and bidirectional streams.
Thanks to this feature QUIC is not affected by head of line blocking problem.
* 




[IETF Datatracker]: https://datatracker.ietf.org/wg/quic/documents
[RFC 8999]: https://datatracker.ietf.org/doc/rfc8999
[RFC 9000]: https://datatracker.ietf.org/doc/rfc9000
[RFC 9001]: https://datatracker.ietf.org/doc/rfc9001
[RFC 9002]: https://datatracker.ietf.org/doc/rfc9002

