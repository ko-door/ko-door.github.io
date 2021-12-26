---
title: "#pragma once"
categories:
- c/c++
- update
---

## #pragma once

~~~ cpp
#pragma once
~~~

`#pragma once`  is for multiple-include optimization.\\
After the first `#include` of the file with the '#pragama once' directive, the compiler won't open and read the file again.

## include guards

~~~ cpp
#ifndef __HEADER_H__
#define __HEADER_H__
...
#endif
~~~

`#pragma once` is not a standard, so some compilers won't support it. \\
However, it is faster than include guards because the file with include guards should be opened and checked by the compiler.

## Reference

[once pragma | Microsoft Docs](https://en.wikipedia.org/wiki/Pragma_once)\\
[pragma once - Wikipedia](https://docs.microsoft.com/en-us/cpp/preprocessor/once?view=msvc-170)
