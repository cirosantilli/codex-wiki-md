<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The induced [internal hom for modules over a Hopf algebra](../../../../../../internal-hom-for-modules-over-a-hopf-algebra.md) on $\operatorname{Hom}_k(H,H)$ is

$$
(h\cdot T)(x)=\sum h_{(1)}T(S(h_{(2)})x),
$$

where both occurrences of $H$ have their left regular action. If $T$ is a morphism of left $H$-[modules](../../../../../../module-mathematics.md), then

$$
(h\cdot T)(x)=\sum h_{(1)}S(h_{(2)})T(x)=\varepsilon(h)T(x).
$$

So every such morphism is an [invariant vector of a module over a Hopf algebra](../../../../../../invariant-vector-of-a-module-over-a-hopf-algebra.md).

For the converse, a calculation valid for every $k$-linear $T$ is

$$
\sum(h_{(1)}\cdot T)(h_{(2)}x)=\sum h_{(1)}T(S(h_{(2)})h_{(3)}x)=hT(x).
$$

If $T$ is invariant, its left-hand side is instead $\sum\varepsilon(h_{(1)})T(h_{(2)}x)=T(hx)$. Hence $T(hx)=hT(x)$ for all $h,x$, which is precisely the [R-module homomorphism](../../../../../../module-homomorphism.md) condition.

In fact an endomorphism of the left regular [module](../../../../../../module-mathematics.md) is determined by $a=T(1)$ and has $T(x)=xa$. Conversely each right multiplication map is left $H$-linear. **Thus the invariant space has the explicit description**

$$
\boxed{\operatorname{Hom}_k(H,H)^H=\operatorname{End}_H(H)=\{R_a:x\mapsto xa\mid a\in H\}.}
$$

As a [vector space](../../../../../../vector-space-split.md) it is isomorphic to $H$, and under composition its algebra is the [opposite algebra](../../../../../../opposite-algebra.md) $H^{\mathrm{op}}$. No dimension or semisimplicity hypothesis is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
