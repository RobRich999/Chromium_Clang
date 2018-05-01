# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker and now using the Polly "high-level loop and data-locality optimizer" for LLVM, starting with build revision 551871.

About polyhedral optimization in general:

http://polyhedral.info/

About the Polly optimizer:

http://polly.llvm.org/

Link to latest build release:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v68.0.3416.0-r554843-win64

The latest build release includes the following LLVM and Polly configuration options:

"-mllvm", "-adce-remove-loops",  
"-mllvm", "-addr-sink-new-phis",  
"-mllvm", "-addr-sink-new-select",  
"-mllvm", "-aggressive-ext-opt",  
"-mllvm", "-combiner-global-alias-analysis",  
"-mllvm", "-condsider-local-interval-cost",  
"-mllvm", "-costmodel-reduxcost",  
"-mllvm", "-da-delinearize",  
"-mllvm", "-enable-aa-sched-mi",  
"-mllvm", "-enable-cond-stores-vec",  
"-mllvm", "-enable-deferred-spilling",  
"-mllvm", "-enable-implicit-null-checks",  
"-mllvm", "-enable-interleaved-mem-accesses",  
"-mllvm", "-enable-ipra",  
"-mllvm", "-enable-local-reassign",  
"-mllvm", "-enable-misched",  
"-mllvm", "-loop-prefetch-writes",  
"-mllvm", "-force-precise-rotation-cost",  
"-mllvm", "-regbankselect-greedy",  
"-mllvm", "-vectorizer-maximize-bandwidth",  
"-mllvm", "-polly",  
"-mllvm", "-polly-detect-profitability-min-per-loop-insts=40",  
"-mllvm", "-polly-invariant-load-hoisting",  
"-mllvm", "-polly-optree-normalize-phi",  
"-mllvm", "-polly-precise-fold-accesses",  
"-mllvm", "-polly-precise-inbounds",  
"-mllvm", "-polly-run-dce",  
"-mllvm", "-polly-vectorizer=stripmine",  
"-Xclang", "-Rpass-analysis=polly",  

The V8 JavaScript engine includes the added Polly configuration option:

"-mllvm", "-polly-delicm-max-ops=0",

Additional features of the build include modified compiler optimizations including whole-program analysis and cross-module optimization using "full" link time optimization (LTO) via build configuration modifications.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.
