# Tcl Stack Overflow Bug: Infinite Recursion in `badproc`

This repository demonstrates a common error in Tcl programming: infinite recursion leading to a stack overflow. The `bug.tcl` file contains a recursive procedure `badproc` with an incomplete base case, causing it to recursively call itself indefinitely.  The solution is shown in `bugSolution.tcl`

## How to reproduce

1.  Save the code in `bug.tcl`.
2.  Run the script using a Tcl interpreter (e.g., `tclsh bug.tcl`).

You'll observe a stack overflow error.

## Solution

The `bugSolution.tcl` file provides a corrected version of `badproc` with a proper base case to prevent infinite recursion.