# Scalar Types
- These represent a single value.
- There are four primary scalar types.
	- Integers
	- Floating-point numbers
	- Booleans
	- Characters
## Integer Types
- There are signed and unsigned integers.
- Signed integers means it can be positive or negatives.
- Unsigned integers means it is always positive.
- `u32` means an unsigned integer type with 32 bits. So this is any integer between `0` and `2^32 - 1` inclusive.
- `i32` means a signed integer type with 32 bits. So this is any integer between `-(2^31)` to `2^31 - 1` inclusive.
- Generally an unsigned variant can store `0` to `2^n - 1` inclusive and a signed variant can store `-(2^(n-1))` to `2^(n-1) - 1` inclusive.

| Length  | Signed  | Unsigned |
| ------- | ------- | -------- |
| 8-bit   | `i8`    | `u8`     |
| 16-bit  | `i16`   | `u16`    |
| 32-bit  | `i32`   | `u32`    |
| 64-bit  | `i64`   | `u64`    |
| 128-bit | `i128`  | `u128`   |
| arch    | `isize` | `usize`  |
## Floating Point Types
- There are two floating-point types. `f32` and `f64`. The difference is simply 32 bit vs 64 bit.
- `f64` is the default because it is more precise and there is negligible performance difference between `f32` and `f64` on modern cpu's.