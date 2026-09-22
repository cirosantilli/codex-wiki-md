<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We use the left internal-hom convention in which $[M,N]$ is right adjoint to $-\otimes_kM$, so its [evaluation morphism](../../../../../../evaluation-morphism.md) has domain $[M,N]\otimes_kM$. For a [Hopf algebra](../../../../../../hopf-algebra.md) over the [commutative ring](../../../../../../commutative-ring.md) $k$, take the full $k$-module

$$
[M,N]=\operatorname{Hom}_k(M,N)
$$

and give it the [internal hom for modules over a Hopf algebra](../../../../../../internal-hom-for-modules-over-a-hopf-algebra.md)

$$
\boxed{(h\cdot f)(u)=\sum h_{(1)}\cdot f(S(h_{(2)})\cdot u).}
$$

The [antipode](../../../../../../antipode.md) is an antihomomorphism, $S(hg)=S(g)S(h)$, so

$$
(h\cdot(g\cdot f))(u)=\sum h_{(1)}g_{(1)}\cdot f(S(g_{(2)})S(h_{(2)})\cdot u)=((hg)\cdot f)(u).
$$

The unit acts identically. Thus this is a left $H$-[module](../../../../../../module-mathematics.md).

The [evaluation morphism](../../../../../../evaluation-morphism.md) is $H$-linear. Using the [diagonal bialgebra action](../../../../../../diagonal-bialgebra-action.md) and the antipode identity,

$$
\sum(h_{(1)}\cdot f)(h_{(2)}\cdot u)=\sum h_{(1)}\cdot f(S(h_{(2)})h_{(3)}\cdot u)=h\cdot f(u).
$$

Now let $q:L\otimes_kM\to N$ be $H$-linear and define its ordinary curried map $\widehat q(\ell)(u)=q(\ell\otimes u)$. To see that it too is $H$-linear, compute

$$
\begin{aligned}
(h\cdot\widehat q(\ell))(u)&=\sum h_{(1)}\cdot q(\ell\otimes S(h_{(2)})\cdot u)\\
&=\sum q(h_{(1)}\cdot\ell\otimes h_{(2)}S(h_{(3)})\cdot u)\\
&=q(h\cdot\ell\otimes u)=\widehat q(h\cdot\ell)(u).
\end{aligned}
$$

Conversely, any $H$-linear map $L\to[M,N]$ uncurries to an $H$-linear map by the already established linearity of evaluation. The ordinary tensor–hom [adjunction](../../../../../../adjoint-functors.md) therefore restricts to a natural [bijection](../../../../../../bijection.md)

$$
\boxed{\operatorname{Hom}_H(L\otimes_kM,N)\cong\operatorname{Hom}_H(L,[M,N]).}
$$

Postcomposition by an $H$-linear map makes $[M,-]$ a [functor](../../../../../../functor.md). This proves that the category of left $H$-[modules](../../../../../../module-mathematics.md) is a [left closed monoidal category](../../../../../../left-closed-monoidal-category.md). **All modules are allowed; no inverse antipode or finite-dimensional dual is required.** Stating the tensor–hom convention explicitly avoids confusing this construction with the closure on the opposite side.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
