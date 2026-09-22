<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $M^2>0$ initially to avoid an infrared divergence. A [Schwinger parameterization](../../../../../schwinger-parameterization.md) and the Euclidean [Gaussian integral](../../../../../gaussian-integral.md) give, in the convergent range $0<\operatorname{Re}d<4$,

$$
\frac1{(k^2+M^2)^2}=\int_0^\infty dt\,t e^{-t(k^2+M^2)},\qquad \int\frac{d^dk}{(2\pi)^d}e^{-tk^2}=(4\pi t)^{-d/2}.
$$

Integration over $t$ supplies the [Gamma function](../../../../../gamma-function.md). Its [analytic continuation](../../../../../analytic-continuation.md) defines the answer in [dimensional regularization](../../../../../dimensional-regularization.md):

$$
\boxed{I_d(M^2)=\frac{\Gamma(2-d/2)}{(4\pi)^{d/2}}(M^2)^{d/2-2}.}
$$

Use $d=4-\epsilon$ near four dimensions and $d=6-\epsilon$ near six dimensions. The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) implies $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and $\Gamma(-1+\epsilon/2)=-2/\epsilon+O(1)$. Therefore

$$
\boxed{I_{4-\epsilon}(M^2)=\frac{2}{(4\pi)^2\epsilon}+O(1),\qquad I_{6-\epsilon}(M^2)=-\frac{2M^2}{(4\pi)^3\epsilon}+O(1).}
$$

Both are simple poles. Equivalently their residues as functions of $d$ are $-2/(4\pi)^2$ at $d=4$ and $2M^2/(4\pi)^3$ at $d=6$. The negative pole near six dimensions is a feature of [analytic continuation](../../../../../analytic-continuation.md); it is not a negative value of the original convergent positive integral. A massless zero-momentum integral is scaleless and cannot be used indiscriminately to extract these ultraviolet poles, because [dimensional regularization](../../../../../dimensional-regularization.md) then combines ultraviolet and infrared contributions.

For the following [Feynman diagrams](../../../../../feynman-diagram.md), specify the Euclidean [action](../../../../../action.md) and additive [counterterms](../../../../../counterterm.md) explicitly so their signs are unambiguous. The four-dimensional interaction is $\mu^\epsilon\lambda\phi^4/4!$, the six-dimensional interaction is $\mu^{\epsilon/2}g\phi^3/3!$, and the common free inverse [scalar propagator](../../../../../scalar-propagator.md) is $p^2+m^2$. Here $\epsilon=4-d$ or $6-d$, respectively. The factors of $\mu$ give dimensionless renormalized couplings and change no leading pole residues. The cubic Euclidean theory is treated as a formal perturbation expansion about its massive quadratic [scalar field theory](../../../../../scalar-field-theory-split.md); its real cubic potential is not bounded below.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
