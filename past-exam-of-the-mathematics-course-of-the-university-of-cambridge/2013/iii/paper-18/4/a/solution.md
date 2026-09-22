<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [adjunction](../../../../../../adjoint-functors.md) $F\dashv G$ is a family of [bijections](../../../../../../bijection.md)

$$
\Phi_{A,B}:\mathcal D(FA,B)\xrightarrow{\sim}\mathcal C(A,GB)
$$

natural in both variables. Its [adjunction unit](../../../../../../unit-of-an-adjunction.md) and [adjunction counit](../../../../../../counit-of-an-adjunction.md) are $\eta_A=\Phi_{A,FA}(1_{FA})$ and $\varepsilon_B=\Phi^{-1}_{GB,B}(1_{GB})$. Naturality of the correspondence gives

$$
\Phi(u)=Gu\,\eta_A,\qquad \Phi^{-1}(v)=\varepsilon_BFv.
$$

For $f:A\to A'$, naturality in both variables evaluates $\Phi(Ff)$ in two ways, giving $GFf\,\eta_A=\eta_{A'}f$. Thus $\eta$ is a [natural transformation](../../../../../../natural-transformation.md); the dual calculation gives naturality of $\varepsilon$.

Applying the inverse correspondence to $\eta_A$ and the correspondence to $\varepsilon_B$ yields the [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md):

$$
\boxed{\varepsilon_{FA}F\eta_A=1_{FA},\qquad G\varepsilon_B\eta_{GB}=1_{GB}.}
$$

They express that transposing an [identity morphism](../../../../../../identity-morphism.md) and transposing back returns that identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
