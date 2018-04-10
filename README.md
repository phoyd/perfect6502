# This fork
...adds a CMakeList.txt file, so this project can be imported to any IDE that supports CMake / is supported by CMake.

# perfect6502

*perfect6502* is a MOS 6502 CPU emulator that performs a simulation of the original NMOS 6502 netlist that was extracted by the [visual6502.org](http://www.visual6502.org/) project.

Consequently, *perfect6502* is
* *perfect*: It is not a reimplementation of the 6502, but a simulation of the original transistors. Its complete behavior, its internal state and its outputs are half-cycle exact.
* *slow*: Even though *perfect6502* is highly optimized C code, achieves only 1/150 of the speed of a 1 MHz 6502 on a high-end CPU of 2014.

*perfect6502* is useful for
* understanding and reverse engineering the 6502
* debugging 6502 emulators by running them side by side with *perfect6502*

## Usage

As a demonstration and as a performance/regression test, *perfect6502* is hooked up to [Commodore BASIC](http://en.wikipedia.org/wiki/Commodore_BASIC) (cbmbasic).

You can compile the project with

	$ make

and run it with

	$ ./cbmbasic

You should get the following output:

		**** COMMODORE 64 BASIC V2 ****
	
	 64K RAM SYSTEM  38911 BASIC BYTES FREE
	
	READY.

# Credits

*perfect6502* is is written by [Michael Steil](http://www.pagetable.com/) and derived from the JavaScript [visual6502](https://github.com/trebonian/visual6502) implementation by Greg James, Brian Silverman and Barry Silverman.

# Contributing

Further performance optimizations are gladly accepted.
