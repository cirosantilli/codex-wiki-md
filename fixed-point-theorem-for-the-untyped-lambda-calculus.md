# Fixed-point theorem for the untyped lambda calculus

↑ **Parent:** [Fixed-point combinator](fixed-point-combinator.md)

Every lambda term $F$ has a fixed point: the term

$$
X=(\lambda x.F(xx))(\lambda x.F(xx))
$$

satisfies $X\equiv_\beta F(X)$. Equivalently, a [fixed-point combinator](fixed-point-combinator.md) such as

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx))
$$

satisfies $YF\equiv_\beta F(YF)$ for every $F$.

## ↑ Ancestors (9)

1. [Fixed-point combinator](fixed-point-combinator.md)
2. [Combinator](combinator.md)
3. [Untyped lambda calculus](untyped-lambda-calculus.md)
4. [Lambda calculus](lambda-calculus.md)
5. [Computability theory](computability-theory.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-120/3/b/solution.md)
