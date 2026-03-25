Systems Programming in C

This collection includes three C projects focused on memory management, file and directory processing, and shell implementation. Together, they build on core systems programming concepts such as dynamic memory allocation, linked lists, recursion through directories, parsing, process creation, redirection, pipes, and command execution. These projects reflect hands-on experience with low-level programming in C and operating-system style functionality.

Project 1: Custom Memory Allocator

This project implements a custom version of malloc and free using a linked-list-based memory manager. It tracks allocated and free memory blocks, supports coalescing adjacent free blocks, and includes multiple test programs for validating correctness, error handling, memory leaks, and allocation behavior under stress. The project helped strengthen my understanding of pointers, heap layout, memory safety, and allocator design.
	1.	mymalloc.c: Implements the custom memory allocation and deallocation logic.
	2.	mymalloc.h: Header file containing allocator definitions and function declarations.
	3.	testmymalloc.c: Basic test program for checking standard allocation and free behavior.
	4.	memtest.c: Additional memory testing for allocator correctness.
	5.	memgrind.c: Stress test program that repeatedly allocates and frees memory in different patterns.
	6.	allocatepatterntest.c: Verifies that separately allocated blocks do not overwrite one another.
	7.	leakdetector.c: Test program that intentionally creates leaks for debugging and validation.
	8.	errortest.c: Tests incorrect or invalid memory operations to confirm proper error handling.
	9.	Makefile: Build instructions for compiling the allocator and test programs.

Project 2: Recursive Word Counter

This project processes text files and directories to build a word-frequency list using a dynamically allocated linked list. It recursively traverses directories, reads valid .txt files, parses words character by character, counts duplicates, and sorts the final output by frequency and lexicographic order. This project demonstrates file handling, recursion, linked-list manipulation, dynamic strings, and input validation in C.
	1.	words.c: Main program that processes files and directories, extracts words, stores counts, and prints sorted results.
	2.	Makefile: Build instructions for compiling the word counter.
	3.	test/: Folder of sample input files and directory structures used for testing recursion, formatting, duplicates, long words, and invalid inputs.

Project 3: Custom Unix-Style Shell

This project implements a simplified Unix-style shell in C that supports interactive and batch mode execution. It includes built-in commands such as cd, pwd, which, and exit, along with support for command execution, redirection, pipes, and wildcard expansion. The project highlights process control, parsing, file descriptor management, and shell-style command interpretation.
	1.	mysh.c: Main shell implementation supporting interactive mode, batch mode, built-ins, redirection, pipes, and wildcard handling.
	2.	Makefile: Build instructions for compiling the shell.
	3.	basic_test.sh: Script for testing core shell functionality.
	4.	builtins.sh: Script for testing built-in shell commands.
	5.	redirection.sh: Script for testing input/output redirection behavior.
	6.	input.txt: Sample batch input file for shell testing.
	7.	input2.txt: Additional batch input file for testing commands.
	8.	input3.txt: Additional shell input file for command testing.
	9.	test1.txt: Sample text file used in shell command tests.
	10.	test2.txt: Sample text file used for sorting or redirection tests.
	11.	test3.txt: Sample file used in shell output tests.
	12.	test6.txt: Additional input file used in shell command testing.
	13.	sorted.txt: Output or reference file used to verify shell command results.
