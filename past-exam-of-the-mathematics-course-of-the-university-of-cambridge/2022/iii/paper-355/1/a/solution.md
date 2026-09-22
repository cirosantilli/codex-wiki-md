<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Monge representation](../../../../../../monge-representation.md), $ds=dx+O(h_x^2)$ and the signed curvature is $\kappa=h_{xx}+O(h_x^2h_{xx})$. To quadratic order,

$$
E[h]=\frac A2\int_0^L(h_{xx}-\kappa_0)^2dx.
$$

Two integrations by parts give

$$
\delta E=A\left[(h_{xx}-\kappa_0)\delta h_x-h_{xxx}\delta h\right]_0^L
+A\int_0^Lh_{xxxx}\delta h\,dx.
$$

Thus a filament with free ends has zero bending moment and shear force,

$$
\boxed{h_{xx}(0,t)=h_{xx}(L,t)=\kappa_0,
\qquad h_{xxx}(0,t)=h_{xxx}(L,t)=0,}
$$

and the local [Stokesian dynamics of an elastic filament](../../../../../../stokesian-dynamics-of-an-elastic-filament.md) is

$$
\boxed{\zeta h_t=-Ah_{xxxx}.}
$$

With $X=x/L$, $H=h/L$, and $\tau=At/(\zeta L^4)$, the dimensionless problem is

$$
H_\tau=-H_{XXXX},
\qquad H_{XX}=\kappa_0L,
\qquad H_{XXX}=0
$$

at $X=0,1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
