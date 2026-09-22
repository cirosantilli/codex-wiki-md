# Solvability of an affine rank-one vector equation

↑ **Parent:** [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)

Let $a,b,c\in\mathbb R^n$, with $c\ne0$. The equation $x=a+(b\cdot x)c$ is the [linear system](system-of-linear-equations.md) $(I-cb^T)x=a$, a [rank-one matrix update](rank-one-matrix-update.md) of the [identity matrix](identity-matrix.md). Every solution has $x=a+\lambda c$. Substitution reduces the entire problem to

$$
\lambda(1-b\cdot c)=b\cdot a.
$$

If $b\cdot c\ne1$, there is one solution, $x=a+c(b\cdot a)/(1-b\cdot c)$. If $b\cdot c=1$ and $b\cdot a=0$, every $\lambda\in\mathbb R$ works and the solution set is the [straight line](straight-line.md) $a+\mathbb Rc$. If $b\cdot c=1$ and $b\cdot a\ne0$, there is no solution.

The first reduction follows directly from the original equation in any dimension. In three dimensions it can also be obtained by taking the [cross product](cross-product.md) with $c$, giving $(x-a)\times c=0$. The singular denominator therefore represents two different possibilities, inconsistency or a family of solutions, and must not simply be discarded as an undefined formula.

## ↑ Ancestors (8)

1. [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
2. [Sherman–Morrison formula](sherman-morrison-formula.md)
3. [Matrix inverse](matrix-inverse-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/15/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/11/b/i/solution.md)
