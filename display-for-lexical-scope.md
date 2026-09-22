# Display for lexical scope

↑ **Parent:** [Call stack](call-stack.md)

A table of [pointers](pointer-computer-programming.md) supporting direct access to active lexical environments without traversing a [static chain](static-chain.md). A conventional display is indexed by lexical level; a procedure-indexed alternative keeps the newest activation of each procedure and saves and restores the previous table entry on entry and return.

For direct calls under [lexical scope](lexical-scope.md), the executing activation's [static chain](static-chain.md) contains the newest surviving activations of its enclosing procedures. This follows by [mathematical induction](mathematical-induction.md) on calls and returns: a direct call inherits a suffix of the caller's chain, and a return restores the previous chain after intervening activations finish. With [procedural parameters](procedural-parameter.md), a passed [programming closure](closure-computer-programming.md) can instead refer to an older still-active enclosing activation, so simply consulting the newest-activation table is insufficient.

## ↑ Ancestors (5)

1. [Call stack](call-stack.md)
2. [Stack (data structure)](stack-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/2/e/solution.md)
