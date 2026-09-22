# Trace-generated maximal-period linear-feedback sequence

↑ **Parent:** [Linear-feedback shift register](linear-feedback-shift-register.md)

Let $K=\mathbb F_{2^d}$, let $\alpha$ generate $K^\times$, and let $T:K\to\mathbb F_2$ be nonzero linear with [nondegenerate bilinear form](nondegenerate-bilinear-form.md) $(x,y)\mapsto T(xy)$. If the [minimal polynomial](minimal-polynomial.md) of $\alpha$ is $P(X)=X^d+\sum_{j<d}c_jX^j$, then $x_n=T(\alpha^n)$ satisfies

$$
x_{n+d}=\sum_{j<d}c_jx_{n+j},
$$

so it is produced by an LFSR of length at most $d$. Its period is exactly $2^d-1$: any period $r$ would imply $T((\alpha^r-1)y)=0$ for every $y\in K$, hence $\alpha^r=1$ by nondegeneracy.

## ↑ Ancestors (6)

1. [Linear-feedback shift register](linear-feedback-shift-register.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/12i/c/ii/solution.md)
