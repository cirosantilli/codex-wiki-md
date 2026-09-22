# Complete development of a lambda term

↑ **Parent:** [Parallel beta reduction](parallel-beta-reduction.md)

Define $x^\bullet=x$, $(\lambda x.M)^\bullet=\lambda x.M^\bullet$, and develop an application by contracting its root when that root is syntactically a [beta-redex](beta-redex.md): $((\lambda x.M)N)^\bullet=M^\bullet[x:=N^\bullet]$. Otherwise $(MN)^\bullet=M^\bullet N^\bullet$. Newly created root redexes need not be contracted. Induction with the substitution lemma proves that if $M\Rightarrow N$, then $N\Rightarrow M^\bullet$. Thus any two parallel reducts share this reduct.

## ↑ Ancestors (9)

1. [Parallel beta reduction](parallel-beta-reduction.md)
2. [Beta reduction](beta-reduction.md)
3. [Untyped lambda calculus](untyped-lambda-calculus.md)
4. [Lambda calculus](lambda-calculus.md)
5. [Computability theory](computability-theory.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-87/1/solution.md)
