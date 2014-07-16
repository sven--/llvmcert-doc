### On Passes ###

* You can check the passes for `-O1` by:
```llvm-as < /dev/null | opt -O1 -disable-output -debug-pass=Arguments```

* Passes registers *dependency* in `PassManager` and `clang`, `opt` tools respect the registered dependency.

  + Thus you can freely give options to `opt` without worrying about correctness on dependency.

