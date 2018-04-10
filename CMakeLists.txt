cmake_minimum_required(VERSION 2.6)
project (perfect6502)
configure_file(cbmbasic.bin cbmbasic.bin COPYONLY)
add_executable(cbmbasic perfect6502.c netlist_sim.c cbmbasic.c readdir.c runtime.c runtime_init.c plugin.c console.c emu.c)
