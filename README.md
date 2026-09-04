# MiniDB

A concurrent, crash-proof embedded database engine, built from scratch to
demonstrate core Operating Systems and DBMS concepts.

## Building

```
mkdir build
cd build
cmake -G "MinGW Makefiles" ..
cmake --build .
./minidb.exe
```

If everything is set up correctly, minidb.exe runs a threading sanity
check and prints "Environment OK - threads + mutex working correctly."
