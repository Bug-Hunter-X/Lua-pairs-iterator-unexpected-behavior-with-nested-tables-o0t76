# Lua pairs Iterator Issue with Nested Tables

This repository demonstrates a potential issue with Lua's `pairs` iterator when dealing with nested tables that are modified during iteration. The code in `bug.lua` recursively iterates through a nested table.  Under certain circumstances (especially if the table structure is changed within the loop), the iterator might behave unexpectedly, skipping elements or even causing an infinite loop. The `bugSolution.lua` offers one method to avoid this problem.

## How to Reproduce

1. Clone this repository.
2. Run `bug.lua`. The output might not be what's expected because of the iterator's behavior.
3. Examine `bugSolution.lua` for a possible solution and compare the output.