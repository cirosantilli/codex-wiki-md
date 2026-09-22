# Occurs check

↑ **Parent:** [Type variable](type-variable.md)

The [occurs check](occurs-check.md) tests whether a [type variable](type-variable.md) occurs inside the expression proposed as its replacement during [type unification](type-unification.md). After discarding a trivial [equation](equation.md) such as $\alpha=\alpha$, solving $\alpha=\tau$ by a [type substitution](type-substitution.md) requires that $\alpha$ not occur in $\tau$. Thus $\alpha=\mathrm{int}\to\beta$ is permitted when $\alpha$ and $\beta$ are distinct, but $\alpha=\alpha\to\beta$ is rejected in our finite [simple type](simple-type.md) grammar.

There is a short reason for the rejection. If a finite replacement $T$ for $\alpha$ existed, with replacement $B$ for $\beta$, the [equation](equation.md) would become $T=T\to B$. The right side's [abstract syntax tree](abstract-syntax-tree.md) has one new arrow node plus the nodes of $T$ and $B$, so it has strictly more nodes than $T$. Equal finite type expressions cannot have different sizes. [Recursive types](recursive-type.md) are a different design: they explicitly describe self-reference and specify how it interacts with [typing judgments](typing-judgment.md).

## ↑ Ancestors (5)

1. [Type variable](type-variable.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Occurs check](occurs-check.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/10/b/solution.md)
- [Type unification](type-unification.md)
