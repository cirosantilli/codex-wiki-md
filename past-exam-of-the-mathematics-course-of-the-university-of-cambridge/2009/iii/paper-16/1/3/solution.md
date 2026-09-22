<h1 id="1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The space is the [mapping torus](../../../../../../mapping-torus.md) of the [antipodal map](../../../../../../antipodal-map.md) $A:S^n\to S^n$. For $n\geq1$, its [mapping degree](../../../../../../degree-of-a-continuous-mapping.md) is $\delta=(-1)^{n+1}$: $A$ is the restriction of $-I$ on $\mathbb R^{n+1}$, whose determinant is $(-1)^{n+1}$. The [Wang sequence](../../../../../../wang-sequence.md) gives

$$
0\longrightarrow\operatorname{coker}(1-A_*:H_j(S^n)\to H_j(S^n))\longrightarrow H_j(T_A)\longrightarrow\ker(1-A_*:H_{j-1}(S^n)\to H_{j-1}(S^n))\longrightarrow0.
$$

The kernel terms are free abelian, so these short exact sequences split as groups. On $H_0(S^n)$ the map is the identity, and on $H_n(S^n)$ it is multiplication by $\delta$. For $n\geq2$ this gives

$$
\boxed{H_j(T_A;\mathbb Z)=\begin{cases}
\mathbb Z,&j=0,1,\\
\mathbb Z,&n\text{ odd and }j=n,n+1,\\
\mathbb Z/2,&n\text{ even and }j=n,\\
0,&\text{otherwise}.
\end{cases}}
$$

At $n=1$, both contributions to degree one are present, giving $H_0=H_2=\mathbb Z$ and $H_1=\mathbb Z^2$, with all other groups zero. At $n=0$, the antipodal map exchanges the two points of $S^0$, and the two cylinder intervals join into a single circle; thus $H_0=H_1=\mathbb Z$ and higher groups vanish. These are the [homology of the antipodal sphere mapping torus](../../../../../../homology-of-the-antipodal-sphere-mapping-torus.md) cases.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
