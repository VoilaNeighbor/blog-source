# Testing IO-Heavy Code

IO-bound code has been traditionally perceived as "hard to test", due to its
rich interactions with the environment. The conclusion is proven to be false
with the advent of event-driven programming, where messy inputs or outputs are
unified under the concept of "events". An event-driven architecture operates
around typed packages of data. With this reified IO type, not only the tests
are easier, but the program structure is cleaner with lower-level IO details
decoupled from logic applied on the data.

Streaming can be a bit complex for the event model. However, most of IO code
today uses buffers. A streaming app can instead send events in segments,
emulating the effect of a batch writer, aka buffering writer. Since the
upper-level logic has more information to decide a way to split the packages,
theoretically, it could even outperform buffering stream writers in some cases!