1. Optional Strings
2. Lack of proper type system
3. Lack of ADTs
4. iota
5. init being run _at import time_

to investigate:
1. That the runtime being async-only basically prevents cache-locality guarantees?
2. threading/structured concurrency
3. Error Handling
4. Generics not implemented for methods