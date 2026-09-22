<h1 id="32e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**No.** Let $x_0=0$ and, for $0<|x|<1$, define

$$
\phi_n(x)=|x|^n,
$$

while

$$
\psi_0(x)=1+|x|^{1/2},
\qquad
\psi_n(x)=|x|^n\quad(n\geq1).
$$

Both families are asymptotic sequences, and $\psi_n\sim\phi_n$ for every $n$.

Take $f(x)=1$. It has the exact expansion

$$
f(x)\sim1\cdot\phi_0(x)+\sum_{n=1}^{\infty}0\cdot\phi_n(x).
$$

Suppose it had an expansion $f\sim\sum_{n\geq0}b_n\psi_n$. The order-zero condition forces $b_0=1$. At order one we would then require some constant $b_1$ such that

$$
1-\psi_0-b_1\psi_1
=-|x|^{1/2}-b_1|x|=o(|x|).
$$

After division by $|x|$, the left side is $-|x|^{-1/2}-b_1$, which cannot tend to zero. This contradiction proves that no such coefficients exist. Thus [termwise equivalent asymptotic scales need not preserve expansions](../../../../../../termwise-equivalent-asymptotic-scales-need-not-preserve-expansions.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32E](../../32e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
