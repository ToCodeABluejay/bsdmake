 
cmake_minimum_required(VERSION 3.0)  # CMake version check
project(bsdmake)                     # Create project
set(C_STANDARD 1)                    # Set C11 standard

add_link_options("-lbsd")
add_executable(make arch.c buf.c cond.c dir.c for.c hash_tables.c hash.c job.c lst.c main.c make.c parse.c proc.c shell.c str.c suff.c targ.c util.c var.c)
