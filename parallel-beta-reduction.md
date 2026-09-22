# Parallel beta reduction

↑ **Parent:** [Beta reduction](beta-reduction.md)

Parallel [beta reduction](beta-reduction.md) permits simultaneous reduction in the body of a [lambda abstraction](lambda-abstraction.md) and both sides of an application, together with $(\lambda x.M)N\Rightarrow M'[x:=N']$ when $M\Rightarrow M'$ and $N\Rightarrow N'$. Variables reduce to themselves. Its [capture-avoiding substitution](capture-avoiding-substitution.md) lemma is $M\Rightarrow M',\ N\Rightarrow N'\Rightarrow M[x:=N]\Rightarrow M'[x:=N']$. Its transitive closure equals ordinary finite beta reduction, while its one-step diamond property yields the [Church-Rosser theorem](church-rosser-theorem.md).

**Table of contents**

- [Complete development of a lambda term](complete-development-of-a-lambda-term.md)

## ↑ Ancestors (8)

1. [Beta reduction](beta-reduction.md)
2. [Untyped lambda calculus](untyped-lambda-calculus.md)
3. [Lambda calculus](lambda-calculus.md)
4. [Computability theory](computability-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-87/1/solution.md)
