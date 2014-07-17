### On LLVM ###

*LLVM*, low-level virtual machine, is a universal progrmming language
between high-level programming languages and assembly languages. The
syntax of LLVM *IR* is based on
[SSA](http://en.wikipedia.org/wiki/Static_single_assignment_form). On
IR a lot of analyses and optimizations are defined as *passes*.

## Installation ##

* Follow the installation [instruction](http://llvm.org/docs/GettingStarted.html#getting-started-quickly-a-summary).

## On Passes ##

* Read the pass [manual](http://llvm.org/docs/WritingAnLLVMPass.html). Experiment with `clang` and `opt` tools.

  + See the result of `opt -help` for passes.

* Read the pass [list](http://llvm.org/docs/Passes.html).

* Note that we will focus on `-O1` [optimizations](passes/O1.txt).

## On IR ##

* Read the IR [manual](http://llvm.org/docs/LangRef.html).
