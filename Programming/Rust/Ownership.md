# Stack
As a data structure, a stack is a first in last out data structure like a stack of plates. In terms of memory, data is pushed onto the stack as the program runs, and popped off when no longer needed. All data stored on the stack must have a known, fixed sized (for example array, NOT vectors). Data with an unknown size at compile time or a size that might change must be stored on the heap.
# Heap
The heap is a less organized data structure. When data is put on the heap, a certain amount is requested. The memory allocator finds an empty spot on the heap that is big enough, marks it as in use, and returns a pointer to that location. This is called allocating. The pointer is a known fixed size, so the pointer can be stored on the stack, but the actual data it points to is on the heap. The main purpose of `ownership` is to efficiently manage data on the heap.
# Rules
- Each value in Rust has an `owner`.
- There can only be one `owner` at a time.
- When the `owner` goes out of scope, the value will be dropped.