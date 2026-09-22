<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep $Z=e^{iW}$, define the mean [scalar field](../../../../../../scalar-field.md) $\varphi(x)=\delta W/\delta J(x)$, and locally invert the source-field relation. The [quantum effective action](../../../../../../effective-action.md) is the [Legendre transform](../../../../../../convex-conjugate.md)

$$
\boxed{\Gamma[\varphi]=W[J]-\int d^dx\,J(x)\varphi(x),\qquad\frac{\delta\Gamma}{\delta\varphi(x)}=-J(x).}
$$

Its value at zero source is expanded around $\varphi_0=\langle\phi\rangle$, which need not vanish. The kernels $\Gamma^{(n)}=\delta^n\Gamma/\delta\varphi^n|_{\varphi_0}$ are the [one-particle-irreducible vertices](../../../../../../one-particle-irreducible-vertex.md), with the Minkowski diagram vertex factor $i\Gamma^{(n)}$. A [one-particle-irreducible Feynman diagram](../../../../../../one-particle-irreducible-feynman-diagram.md) remains connected after any one internal line is cut. [Amputation of external propagators](../../../../../../amputation-of-external-propagators.md) removes the full two-point functions on its external legs. For higher-point connected graphs amputation alone need not remove internal [one-particle-reducible Feynman diagrams](../../../../../../one-particle-reducible-feynman-diagram.md); the derivatives of $\Gamma$ select precisely the irreducible kernels.

To derive the three-point relation, use condensed indices that include spacetime integration. Put $D_{ij}=W_{,ij}=iG_{2,ij}^c$ and $K=\Gamma^{(2)}$. Differentiating $\Gamma_{,i}=-J_i$ gives $K_{ia}D_{aj}=-\delta_{ij}$, so $K=-D^{-1}$. A further derivative, using $\delta D_{ab}/\delta\varphi_k=W_{,ab\ell}(D^{-1})_{\ell k}$ and the derivative of an inverse, gives

$$
\Gamma^{(3)}_{ijk}=(D^{-1})_{ia}(D^{-1})_{jb}(D^{-1})_{kc}W_{,abc}.
$$

Since $W^{(3)}=-G_3^c$ and $D^{-1}=-i(G_2^c)^{-1}$, the [three-point amputation in the connected-action convention](../../../../../../three-point-amputation-in-the-connected-action-convention.md) is

$$
\boxed{i\Gamma^{(3)}_{ijk}=\int da\,db\,dc\,(G_2^c)^{-1}_{ia}(G_2^c)^{-1}_{jb}(G_2^c)^{-1}_{kc}G_{3,abc}^c.}
$$

Equivalently, attach a full [two-point correlation function](../../../../../../two-point-correlation-function.md) to each leg of $i\Gamma^{(3)}$ to reconstruct $G_3^c$. The connected functions are evaluated at the same zero-source background. The displayed factors of $i$ follow from the declared Minkowski convention; Euclidean generating functionals redistribute these factors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
