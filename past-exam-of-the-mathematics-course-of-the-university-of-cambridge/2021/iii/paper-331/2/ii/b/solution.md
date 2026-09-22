<h1 id="2/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $T=\varepsilon t$ and expand

$$
\frac1R=\frac1{R_c+\varepsilon^2}
=-f'(0)-\varepsilon^2f'(0)^2+O(\varepsilon^4).
$$

At order $\varepsilon^2$, the assumptions $f''(0)=0$ and the orthogonality normalization leave a homogeneous equation for $u_2$ with no forcing, hence $\boxed{u_2=0}$.

At order $\varepsilon^3$, project the equation onto the null mode $\sin z$. Since

$$
\frac{\int_0^\pi\sin^4z\,dz}{\int_0^\pi\sin^2z\,dz}=\frac34,
$$

the [Fredholm solvability condition](../../../../../../../fredholm-solvability-condition.md) obtained directly from the definitions printed in the question is

$$
\boxed{
\frac{d^2A}{dT^2}
=f'(0)^2A-\frac18f'''(0)A^3}.
$$

The paper asks for $A/f'(0)^2$ in place of $f'(0)^2A$, but that coefficient is incompatible with $R_c=-1/f'(0)$ and $\varepsilon^2=R-R_c$: differentiating $1/R$ at $R_c$ gives $-1/R_c^2=-f'(0)^2$. Thus the displayed target appears to contain a reciprocal typo. It would agree with the expansion only under a correspondingly rescaled definition of the small parameter.

The imposed orthogonality of every $u_j$, $j\geq2$, removes the freedom to transfer a multiple of $\sin z$ between $A$ and the higher-order terms.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
