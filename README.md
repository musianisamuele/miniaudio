This is a fork of the miniaudio library that is used as a submodule and will
NOT be updated. If I have time I will remove some of the features as they are
not needed. __All credits go to the original author__

## Miniaudio
miniaudio is a library written in C with no dependencies except the standard 
library and should compile clean on all major compilers without the need to 
install any additional development packages. All major desktop and mobile platforms
are supported.

## Building

Do the following in one source file:
```c
#define MINIAUDIO_IMPLEMENTATION
#include "miniaudio.h"
```
If you get errors about undefined references to `__sync_val_compare_and_swap_8`, 
`__atomic_load_8`, etc. you need to link with `-latomic`.
