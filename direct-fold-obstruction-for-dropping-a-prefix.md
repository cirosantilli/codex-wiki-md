# Direct fold obstruction for dropping a prefix

↑ **Parent:** [List fold](list-fold.md)

Suppose a [predicate](predicate.md) accepts some $u$ and rejects some $v$. Dropping its initial accepted [list prefix](prefix-of-a-list.md) maps both the empty [list](list-abstract-data-type.md) and the singleton $u$ to the empty [list](list-abstract-data-type.md), but maps the extensions by $v$ to different [lists](list-abstract-data-type.md). A direct [list fold](list-fold.md) cannot do this: its combining [function](function-split.md) receives the same head and the same folded-tail summary in both cases. This is an instance of the [fold factorisation criterion](fold-factorisation-criterion.md). An auxiliary [list fold](list-fold.md) retaining more information followed by projection is not ruled out.

## ↑ Ancestors (5)

1. [List fold](list-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
