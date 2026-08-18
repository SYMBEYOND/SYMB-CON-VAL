# SYMB-FER T10 Size Measurement Register

Test: T10 Bounded Size and Attention Budget  
Fixture version: v0.1  
Measurement date: 2026-08-12 MDT

Measurements use the generated UTF-8 packet bytes exactly as packaged. Words are whitespace-delimited counts from `wc -w`. Lines are reported by `wc -l`.

| Level | Noise blocks | Lines | Words | Bytes | SHA-256 |
|---|---:|---:|---:|---:|---|
| L1 | 20 | 199 | 1,559 | 13,403 | `7083747abff48a92999647ca3fe94d0f8a0e8e4fbdafa943a9e55b22621c58d6` |
| L2 | 100 | 771 | 6,527 | 56,095 | `a5b9535e6de3b44b483b39e536c35e896a151caf44b69517d285cbfe353b2792` |
| L3 | 300 | 2,203 | 18,987 | 163,111 | `903bd278b8228a5dfb58c34dbc1ddc6ef78da53b152e71c2217746adaf24b586` |
| L4 | 700 | 5,067 | 43,907 | 377,143 | `b029877e8618861db1dcf1da4f5913aced791f660022009c61353eab7c8104de` |

## Enforcement rule

The fully passing attention budget is the exact byte and word size of the largest consecutively tested level that scores `PASS` with no critical failure. `PASS_WITH_PATCH` and `FAIL` do not extend that budget.

If L1 fails, no safe minimum is established. If L4 passes, the result is a lower bound of at least 377,143 bytes and 43,907 whitespace-delimited words for this fixture and receiver environment only. It is not evidence of unlimited attention.

Token counts are intentionally not governing because tokenizer behavior varies across providers and models.
