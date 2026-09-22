# Reverse Polish notation

↑ **Parent:** [Expression notation](expression-notation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse_Polish_notation)

Place each operator after its operands. A binary application encodes its first subtree, then its second subtree, then the operator, a [postorder traversal](postorder-traversal.md). A [stack machine](stack-machine.md) evaluates the tokens in one pass, popping the right operand before the left one. Reversing a [Polish notation](polish-notation.md) token list also reverses operand order: prefix subtraction `- a b` would become `b a -` rather than the required `a b -`.

## ↑ Ancestors (4)

1. [Expression notation](expression-notation.md)
2. [Mathematical notation](mathematical-notation.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
