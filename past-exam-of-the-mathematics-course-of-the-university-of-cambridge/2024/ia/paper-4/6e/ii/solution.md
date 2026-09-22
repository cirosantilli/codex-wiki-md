<h1 id="6e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $m,l$, set

$$
D_n=F_{n+l}F_{n+m}-F_nF_{n+m+l}.
$$

At $n=0$, $D_0=F_lF_m$. Applying the Fibonacci recurrence to every term and cancelling gives $D_{n+1}=-D_n$. Induction therefore proves

$$
\boxed{F_{n+l}F_{n+m}-F_nF_{n+m+l}
=(-1)^nF_mF_l}.
$$

Applying this identity to the relevant pairs of indices and using $F_{r+1}=F_r+F_{r-1}$ gives

$$
F_{j+k}^2-F_{j-k}^2=F_{2k}F_{2j}
$$

and

$$
F_{j+k+1}^2+F_{j-k}^2=F_{2k+1}F_{2j+1}.
$$

Thus, for $j\geq k\geq0$,

$$
\boxed{(F_{j+k}-F_{j-k})(F_{j+k}+F_{j-k})=F_{2k}F_{2j}}
$$

and

$$
\boxed{F_{j+k+1}^2+F_{j-k}^2=F_{2k+1}F_{2j+1}}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
