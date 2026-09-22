<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the degree-$d$ [projective hypersurface](../../../../../../projective-hypersurface.md) $X_d$ be defined by the homogeneous polynomial $F$. Multiplication by $F$ identifies its ideal sheaf with $\mathcal O_{\mathbb P^n}(-d)$, giving the [ideal-sheaf sequence of a projective hypersurface](../../../../../../ideal-sheaf-sequence-of-a-projective-hypersurface.md)

$$
0\longrightarrow\mathcal O_{\mathbb P^n}(-d)
\xrightarrow{\cdot F}\mathcal O_{\mathbb P^n}
\longrightarrow i_*\mathcal O_{X_d}\longrightarrow0.
$$

In particular, the kernel in the question is $\mathcal O_{\mathbb P^n}(-d)$.

For $n=2$, additivity of the [Euler characteristic](../../../../../../euler-characteristic.md) in this short exact sequence and the line-bundle formula

$$
\chi(\mathbb P^2,\mathcal O(m))=\binom{m+2}{2}
$$

give

$$
h^0(X_d,\mathcal O_{X_d})-h^1(X_d,\mathcal O_{X_d})
=\chi(\mathcal O_{X_d})
=1-\binom{2-d}{2}
=1-\frac{(d-1)(d-2)}2.
$$

Here $H^2(X_d,\mathcal O_{X_d})=0$ by the preceding cohomological-dimension argument. Moreover $H^0(\mathbb P^2,\mathcal O(-d))=H^1(\mathbb P^2,\mathcal O(-d))=0$ for $d>0$, so the long exact sequence gives $H^0(X_d,\mathcal O_{X_d})\cong k$. Consequently

$$
h^1(X_d,\mathcal O_{X_d})=\frac{(d-1)(d-2)}2,
$$

which is the [genus-degree formula](../../../../../../genus-degree-formula.md) for a projective plane curve.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
