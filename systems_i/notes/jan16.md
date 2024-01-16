# Lecture 4 - Storage Class, Scope, and Linkage

## Main Memory
Memory addresses range from 0-0xffffffffffffffff (possibly shorter or further depending on system architecture).  

Main Memory |
:---: |
Boot Block |
Operating System |
Application Programs |
Read Only Memory |
Heap and/or memory accessed via malloc() |
Other |
Stack |

## Concepts and Terms
 - Storage class - 4 types
    - determines the type of storage and the lifetime of the storage associated with a variable, and the variable's initialization (if any)
    - `static`
    - `automatic` (or auto)
    - `register`
    - `external` (really linkage, not storage)
    - These have nothing to do with C++ classes
 - Storage `scope` - 4 types
    - determines the region of a program in which a variable can be accessed
    - `block`
    - `file`
    - `prototype`
    - `function` (very limited use, we won't cover)
 - Storage `linkage` - 3 types
    - for a given name, linkage determines whether the same name in a different file refers to the same variable or function, or some different variable or function
    - `internal`
    - `external`
    - `none`
 - `process` - A group of functions that work together to perform a particular job

### Storage Class
 - `static`
    - static values are on the heap
    - the slowest of the bunch
    - they maintain the last value they were assigned until the program completes
        - when the static keyword is in a block, it changes the variable's `class`
        - when the static keyword is outside all blocks, it changes the `linkage`
 - `automatic`
    - automatic values are on the runtime stack
    - these are considerably faster than heap values
    - these values become inaccessible as soon as execution leaves the block
 - `register`
    - register values are stored inside of registers on the processor
    - this is the fastest, but it only works when the processor has the open space

### Storage Scope
 - `block`
    - if it is declared inside of a block, it is scoped inside that block
    - this means the variable can be referenced by name in that block
 - `file`
    - anything defined outside of all blocks
 - `prototype`
    - applies to any variable given in a function prototype
    - these variables have no memory class or linkage
    - it does NOT apply to the function name, which always has file scope

### Linkage Types
Linkage determines how multiple occurrences of a file scope identifier with the same name are treated. Scope and linkage are related, but not the same.
 - `none` for anything declared inside of a block and for prototype scope variables
 - `internal` for all references to this variable being inside the same file, applies to variables with the `static` keyword
 - `extern` for when you want to access a variable from another file