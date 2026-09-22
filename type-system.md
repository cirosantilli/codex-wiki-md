# Type system

↑ **Parent:** [Programming language](programming-language-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_system)

A [type system](type-system.md) assigns types to program expressions and supplies rules governing their use. A type constrains permitted operations: in our teaching [programming language](programming-language-split.md), `int` admits [integer](integer-split.md) addition, `bool` supplies `true` and `false` for conditions, and a [function type](function-type.md) specifies an argument type and a result type. Storage as [bits](bit.md) alone does not explain these distinctions; the [type system](type-system.md) determines whether an expression can serve as an argument, a condition or an operand.

A [typing judgment](typing-judgment.md) $\Gamma\vdash e:\tau$ says that expression $e$ has type $\tau$ under the assumptions in the [typing context](typing-context.md) $\Gamma$. For example,

$$
\Gamma=\{x:\mathrm{int},y:\mathrm{int}\},\qquad \Gamma\vdash x+y:\mathrm{int}.
$$

The assumptions give each operand type `int`; the addition rule then gives the sum type `int`. Changing $y$ to type `bool` prevents this derivation. Our teaching [programming language](programming-language-split.md) has distinct `int` and `bool` types and no implicit conversions between them.

The conditional rule requires a Boolean condition and the same type for both branches:

$$
\frac{\Gamma\vdash c:\mathrm{bool}\qquad\Gamma\vdash e_1:\tau\qquad\Gamma\vdash e_2:\tau}{\Gamma\vdash\mathrm{if}\ c\ \mathrm{then}\ e_1\ \mathrm{else}\ e_2:\tau}.
$$

Thus `if true then 1 else 2` has type `int`, while `if true then 1 else false` is rejected: its branches would require $\tau=\mathrm{int}$ and $\tau=\mathrm{bool}$ simultaneously. Even a branch that will not execute is checked by this rule. This is a rule of this particular [type system](type-system.md); a different [programming language](programming-language-split.md) can choose different rules. [Software Foundations, Programming Language Foundations, Type Systems: typing relation](https://softwarefoundations.cis.upenn.edu/plf-current/Types.html)

The useful feature is compositional reasoning: after checking the parts, a rule explains how to check the whole. The [function type](function-type.md) diagram shows this for a call. [Type inference](type-inference.md) can discover the required types automatically, and [type variables](type-variable.md) let one express relationships that recur across many concrete types. The result is both a practical early error detector and a small, readable derivation explaining why an expression fits its intended use.

The guarantee depends on the rules and execution model. [Type safety](type-safety.md) can exclude specified failures such as adding a Boolean or calling an [integer](integer-split.md) as a function. It does not by itself establish every desired runtime property or guarantee that execution terminates. A [type system](type-system.md) that permits unrestricted recursion can accept a computation that runs forever; [exception handling](exception-handling.md) also needs its own account of permitted outcomes.

**Table of contents**

- [Monomorphic type](monomorphic-type.md)
- [Data type](data-type.md)
  - [Unit type](unit-type.md)
- [Type guard](type-guard.md)
- [Kind (type theory)](kind-type-theory.md)
- [Type constructor](type-constructor.md)
- [Algebraic data type](algebraic-data-type.md)
  - [Tagged union](tagged-union.md)
  - [Data constructor](data-constructor.md)
- [Programming language polymorphism](programming-language-polymorphism.md)
- [Ad hoc polymorphism](ad-hoc-polymorphism.md)
- [Boolean data type](boolean-data-type.md)
- [Haskell type class](haskell-type-class.md)
  - [Eq type class](eq-type-class.md)
  - [Haskell Ord class](haskell-ord-class.md)
- [Variance-position rule](variance-position-rule.md)
- [Path-dependent type](path-dependent-type.md)
- [Runtime type](runtime-type.md)
- [Static type](static-type.md)
- [Subtyping](subtyping.md)
  - [Lower type bound](lower-type-bound.md)
  - [Upper type bound](upper-type-bound.md)
    - [F-bounded polymorphism](f-bounded-polymorphism.md)
  - [Supertype](supertype.md)
  - [Subtype polymorphism](subtype-polymorphism.md)
  - [Behavioral subtyping](behavioral-subtyping.md)
- [Type signature](type-signature.md)
  - [Return type](return-type.md)
- [Type synonym](type-synonym.md)
- [Simple type](simple-type.md)
- [Typing judgment](typing-judgment.md)
  - [Typing context](typing-context.md)
- [Type safety](type-safety.md)
- [Type inference](type-inference.md)
  - [Principal type](principal-type.md)
  - [Type unification](type-unification.md)
- [Type variable](type-variable.md)
  - [Type substitution](type-substitution.md)
  - [Type scheme](type-scheme.md)
  - [Occurs check](occurs-check.md)
- [Recursive type](recursive-type.md)
- [Function type](function-type.md)
  - [Procedure type](procedure-type.md)
    - [Procedural parameter](procedural-parameter.md)
  - [Function subtyping variance](function-subtyping-variance.md)
- [Parametric polymorphism](parametric-polymorphism.md)
  - [Generic method](generic-method.md)
  - [Polymorphic type](polymorphic-type.md)
  - [Type parameter](type-parameter.md)
    - [Type argument](type-argument.md)
  - [Contravariant type parameter](contravariant-type-parameter.md)
  - [Covariant type parameter](covariant-type-parameter.md)
    - [Covariance failure for a mutable collection](covariance-failure-for-a-mutable-collection.md)
  - [Type variance](type-variance.md)
- [Hindley-Milner type system](hindley-milner-type-system.md)
  - [Hindley-Milner type inference](hindley-milner-type-inference.md)
  - [Algorithm W](algorithm-w.md)
  - [Let polymorphism](let-polymorphism.md)

## ↑ Ancestors (3)

1. [Programming language](programming-language-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Abstract syntax tree](abstract-syntax-tree.md)
- [Compiler](compiler.md)
- [Programming language](programming-language-split.md)
- [Programming language semantics](programming-language-semantics.md)
- [Type system](type-system.md)
- [Typing judgment](typing-judgment.md)
