# Type system

↑ **Parent:** [Programming language](programming-language.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_system)

A [type system](type-system.md) assigns types to program expressions and supplies rules governing their use. A type constrains permitted operations: in our teaching [programming language](programming-language.md), `int` admits [integer](integer.md) addition, `bool` supplies `true` and `false` for conditions, and a [function type](function-type.md) specifies an argument type and a result type. Storage as [bits](bit.md) alone does not explain these distinctions; the [type system](type-system.md) determines whether an expression can serve as an argument, a condition or an operand.

A [typing judgment](typing-judgment.md) $\Gamma\vdash e:\tau$ says that expression $e$ has type $\tau$ under the assumptions in the [typing context](typing-context.md) $\Gamma$. For example,

$$
\Gamma=\{x:\mathrm{int},y:\mathrm{int}\},\qquad \Gamma\vdash x+y:\mathrm{int}.
$$

The assumptions give each operand type `int`; the addition rule then gives the sum type `int`. Changing $y$ to type `bool` prevents this derivation. Our teaching [programming language](programming-language.md) has distinct `int` and `bool` types and no implicit conversions between them.

The conditional rule requires a Boolean condition and the same type for both branches:

$$
\frac{\Gamma\vdash c:\mathrm{bool}\qquad\Gamma\vdash e_1:\tau\qquad\Gamma\vdash e_2:\tau}{\Gamma\vdash\mathrm{if}\ c\ \mathrm{then}\ e_1\ \mathrm{else}\ e_2:\tau}.
$$

Thus `if true then 1 else 2` has type `int`, while `if true then 1 else false` is rejected: its branches would require $\tau=\mathrm{int}$ and $\tau=\mathrm{bool}$ simultaneously. Even a branch that will not execute is checked by this rule. This is a rule of this particular [type system](type-system.md); a different [programming language](programming-language.md) can choose different rules. [Software Foundations, Programming Language Foundations, Type Systems: typing relation](https://softwarefoundations.cis.upenn.edu/plf-current/Types.html)

The useful feature is compositional reasoning: after checking the parts, a rule explains how to check the whole. The [function type](function-type.md) diagram shows this for a call. [Type inference](type-inference.md) can discover the required types automatically, and [type variables](type-variable.md) let one express relationships that recur across many concrete types. The result is both a practical early error detector and a small, readable derivation explaining why an expression fits its intended use.

The guarantee depends on the rules and execution model. [Type safety](type-safety.md) can exclude specified failures such as adding a Boolean or calling an [integer](integer.md) as a function. It does not by itself establish every desired runtime property or guarantee that execution terminates. A [type system](type-system.md) that permits unrestricted recursion can accept a computation that runs forever; [exception handling](exception-handling.md) also needs its own account of permitted outcomes.

**Table of contents**

- [Simple type](simple-type.md)
- [Typing judgment](typing-judgment.md)
  - [Typing context](typing-context.md)
- [Type safety](type-safety.md)
- [Type inference](type-inference.md)
  - [Type unification](type-unification.md)
- [Type variable](type-variable.md)
  - [Type substitution](type-substitution.md)
  - [Type scheme](type-scheme.md)
  - [Occurs check](occurs-check.md)
- [Recursive type](recursive-type.md)
- [Function type](function-type.md)
- [Parametric polymorphism](parametric-polymorphism.md)
- [Hindley-Milner type system](hindley-milner-type-system.md)
  - [Algorithm W](algorithm-w.md)
  - [Let polymorphism](let-polymorphism.md)

## ↑ Ancestors (3)

1. [Programming language](programming-language.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Abstract syntax tree](abstract-syntax-tree.md)
- [Programming language](programming-language.md)
- [Programming language semantics](programming-language-semantics.md)
- [Type system](type-system.md)
- [Typing judgment](typing-judgment.md)
