<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It is useful to regulate the number of modes first, so the [functional integral](../../../../../../functional-measure.md) identities reduce to ordinary [integration by parts](../../../../../../integration-by-parts.md). Let $C$ be the Gaussian covariance, $F=C^{-1}$, $W=e^{-S_1}$ and put a dot for $\Lambda\partial_\Lambda$. The matrix identity $\dot F=-F\dot C F$ gives

$$
\dot e^{-S_0}=\frac12(F\phi)^T\dot C(F\phi)e^{-S_0}.
$$

The second field derivative of the Gaussian is

$$
\partial_a\partial_b e^{-S_0}
=[(F\phi)_a(F\phi)_b-F_{ab}]e^{-S_0}.
$$

Hence, after two [integrations by parts](../../../../../../integration-by-parts.md),

$$
\dot Z=\int d\phi\,e^{-S_0}\left[\dot W+\frac12\dot C_{ab}\partial_a\partial_bW\right]
+\frac12\operatorname{Tr}(F\dot C)Z.
$$

The imposed flow makes the bracket vanish. The remaining trace is independent of the fields and only changes the Gaussian normalization. Since the free Gaussian normalization is $\mathcal N=(\det(2\pi C))^{1/2}$, $\dot{\log\mathcal N}=\operatorname{Tr}(F\dot C)/2$. Therefore

$$
\boxed{\Lambda\partial_\Lambda(Z/\mathcal N)=0.}
$$

Equivalently, $Z$ is cutoff independent after discarding the stated overall rescaling. This is the [Gaussian covariance differentiation identity](../../../../../../gaussian-covariance-differentiation-identity.md) behind the [Polchinski equation](../../../../../../polchinski-equation.md).

With the Fourier convention above and functional derivatives satisfying $\delta\widetilde\phi(p)/\delta\widetilde\phi(q)=\delta^{(4)}(p-q)$, contraction with $\dot C$ becomes $\int d^4p\,(2\pi)^4\dot C_\Lambda(p)\delta^2/[\delta\widetilde\phi(p)\delta\widetilde\phi(-p)]$. Thus **the numerator $(2\pi)^4$ in the printed flow is consistent with this derivative convention**; it must not be changed independently of the convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
