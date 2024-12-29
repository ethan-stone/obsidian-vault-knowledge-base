# Scalar Types
- These represent a single value.
- There are four primary scalar types.
	- Integers
	- Floating-point numbers
	- Booleans
	- Characters
## Integers
- There are signed and unsigned integers.
- Signed integers means it can be positive or negatives.
- Unsigned integers means it is always positive.
- `u32` means an unsigned integer type with 32 bits. So this is any integer between `0` and `2^32 - 1` inclusive.
- `i32` means a signed integer type with 32 bits. So this is any integer between `-(2^31)` to `2^31 - 1` inclusive.
- Generally an unsigned variant can store `0` to `2^n - 1` inclusive and a signed variant can store `-(2^n-1)` to `2^31 - 1` inclusive.