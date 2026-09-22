<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The [first isomorphism theorem for groups](../../../../../first-isomorphism-theorem.md) states that for a [group homomorphism](../../../../../group-homomorphism.md) $f:G\to Q$,

$$
G/\ker f\cong\operatorname{im}f.
$$

The map $g\ker f\mapsto f(g)$ is well defined because two representatives differ by an element of the kernel; it is a surjective homomorphism onto the image and is injective because $f(g)=e$ exactly when $g\in\ker f$.

For $n_i\in N$ and $h_i\in H$, normality of $N$ gives

$$
(n_1h_1)(n_2h_2)=n_1(h_1n_2h_1^{-1})h_1h_2\in NH,
$$

and $(nh)^{-1}=h^{-1}n^{-1}h\,h^{-1}\in NH$. Hence $NH$ is a subgroup. Also $N\cap H\trianglelefteq H$, since conjugation by $H$ preserves both $N$ and $H$, and $N\trianglelefteq NH$ because $NH\leq G$.

Apply the first isomorphism theorem to $f:H\to NH/N$, $f(h)=hN$. Its kernel is $N\cap H$, and it is surjective because $nhN=hN$. Therefore

$$
\boxed{H/(N\cap H)\cong NH/N}.
$$

If $K,H\trianglelefteq G$, then $KH$ is a normal subgroup: it is a subgroup by the calculation above, and $g(KH)g^{-1}=(gKg^{-1})(gHg^{-1})=KH$. Without normality a product need not be a subgroup. In $S_3$, take $H=\langle(12)\rangle$ and $K=\langle(23)\rangle$. The set $KH$ has four elements, so it cannot be a subgroup of the six-element group by [Lagrange's theorem for finite groups](../../../../../lagrange-s-theorem.md).

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
