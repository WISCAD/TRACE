## Copyright (c) 2014 Min Li,
## Wiscad Lab, Electrical and Computer Engineering,
## University of Wisconsin at Madison, USA.  
## Please do not distribute the files without the consent of the author.

The usage of the binary is ./trace [benchmark] [trace buffer width] [mode id] 
Please make sure when running the binary, there are as few other
processes running at the same time as possible. This is because our binary
is supposed to be using all available threads during execution (For our
setup, we are using 8 threads). We have found out that this can have great
impact on the reported runtime.

The output file has a suffix of ".out" and locates in the same directory as
the benchmarks.  It will contain the names of the signals that are
selected, and also print out the runtime spent for selection.

Note that when running the binary, it will first perform logic simulation
to generate initial values of the flipflops before the real selection
process begins. This portion of the binary should not be considered as a
part of the selection process, thus its runtime is not included in the
reported runtime.

Also note that the benchmarks are slightly modified from the original
ISCAS'89 benchmarks for the binary to read-in (This is because the parser
portion is some legacy code from my colleague which can not take the
original benchmarks.)  The only modification is the format of the
benchmarks, with all the gate types and topology of the benchmarks
unchanged.

For benchmarks that do not have control signals, the mode id should be set
to -1. For others including benchmarks S35932 and S38584, the mode id
always starts from 0. The ".assign" files which locate in the same
directory as the benchmarks show how to set the values of the control
signals to define each mode.
