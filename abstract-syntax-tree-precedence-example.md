# Abstract syntax tree precedence example

↑ **Parent:** [Abstract syntax tree](abstract-syntax-tree.md)

Consider [Python](python-programming-language.md) programs `x=2+3*4` and `x=(2+3)*4`. [Operator precedence](operator-precedence.md) places [multiplication](multiplication.md) inside the right operand of [addition](addition.md) in the first [abstract syntax tree](abstract-syntax-tree.md). The parentheses instead place [addition](addition.md) inside the left operand of [multiplication](multiplication.md) in the second. Their right-hand sides evaluate to $2+(3\cdot4)=14$ and $(2+3)\cdot4=20$. No rule that simply reads all operators left to right would recover both structures. [Python language reference, section 6.17, multiplicative operators bind more tightly than additive operators](https://docs.python.org/3.14/reference/expressions.html#operator-precedence)

<a id="image-abstract-syntax-tree-precedence"></a>
![](abstract-syntax-tree-precedence.png)

**[Figure 59](#image-abstract-syntax-tree-precedence). Two abstract syntax trees for variable assignment: operator precedence gives `x=2+3*4` the value $14$, while parentheses give `x=(2+3)*4` the value $20$**.

These are schematic views of [Python](python-programming-language.md) trees: `Module` is omitted, and the `Add`/`Mult` and `Store` markers are written inside their owning nodes. In the actual schema, `BinOp` has `left`, `op` and `right` fields; `Assign` has a list of `targets` and a `value`. `Name(id='x', ctx=Store())` marks the name as a [variable assignment](variable-assignment.md) target. Reading `x` in a [program expression](program-expression.md) instead uses `Load`. A [variable assignment](variable-assignment.md) is a statement, not an [equation](equation.md) asserting that two values are equal. [CPython 3.14, Parser/Python.asdl: Module, Assign, BinOp, Constant, Name and expr\_context constructors](abstract-syntax-schema-for-cpython-3-14.md)

A restricted recursive evaluator can follow those fields. It accepts only [integer](integer.md) [literal values](literal-value.md) and binary [addition](addition.md), [subtraction](subtraction.md) and [multiplication](multiplication.md); the surrounding [variable assignment](variable-assignment.md) remains a separate action. Using `type(value) is int` excludes Boolean constants, even though [Python](python-programming-language.md) treats `bool` as a subclass of `int`.

```
import ast

OPS = {ast.Add: lambda a, b: a + b,
       ast.Sub: lambda a, b: a - b,
       ast.Mult: lambda a, b: a * b}

def evaluate(node):
    if isinstance(node, ast.Constant) and type(node.value) is int:
        return node.value
    if isinstance(node, ast.BinOp) and type(node.op) in OPS:
        return OPS[type(node.op)](evaluate(node.left), evaluate(node.right))
    raise ValueError("outside the integer-expression language")

for source in ("x=2+3*4", "x=(2+3)*4"):
    tree = ast.parse(source, optimize=0)
    statement = tree.body[0]
    print(statement.targets[0].id, evaluate(statement.value))
# x 14
# x 20
```

The [children in a rooted tree](child-in-a-rooted-tree.md) have ordered roles: `left` and `right` cannot be interchanged. For [subtraction](subtraction.md), `8-3` gives $5$ while `3-8` gives $-5$. [Operator associativity](operator-associativity.md) also matters: `8-3-1` parses as `(8-3)-1`, giving $4$, whereas `8-(3-1)` gives $6$. Here the syntax groups operators to the left; this does not assert the mathematical [associativity](associative-property.md) of [subtraction](subtraction.md). [Operator precedence](operator-precedence.md) determines grouping, rather than a general permission to reorder execution. For example, [Python](python-programming-language.md) evaluates the calls in `f()+g()*h()` in the order `f`, `g`, `h`, although the [multiplication](multiplication.md) result must be ready before the outer [addition](addition.md). [Python language reference, sections 6.16 and 6.17: left-to-right evaluation and left grouping of additive operators](https://docs.python.org/3.14/reference/expressions.html#evaluation-order)

## ↑ Ancestors (4)

1. [Abstract syntax tree](abstract-syntax-tree.md)
2. [Programming language](programming-language.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
