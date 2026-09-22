<h1 id="a/3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $q=\eta=1$, $J_*$ has [eigenvectors](../../../../../../eigenvector.md) $(1,1)$ and $(1,-1)$ with [eigenvalues](../../../../../../eigenvalue.md) $-1$ and $-1/3$. The Neumann spatial modes are $\cos(j\pi x/L)$, $j=0,1,\ldots$. Combining each with those two reaction directions gives temporal rates

$$
-1-(j\pi/L)^2,\qquad-1/3-(j\pi/L)^2.
$$

Every linear perturbation therefore decays at least as fast as $e^{-t/3}$. The slowest mode is the spatially uniform antisymmetric change of the two [biological populations](../../../../../../population-biology.md). Thus

$$
\boxed{m-2/3=O(e^{-t/3}),\qquad n-2/3=O(e^{-t/3}).}
$$

Small nonlinear perturbations have the same bound, not just a formal mode calculation. In one spatial dimension take sufficiently small smooth Neumann data, or small data in a norm such as $H^1$ that controls quadratic products. The linear semigroup decays at rate $1/3$, and the nonlinear remainder is quadratic. Standard small-data variation-of-constants estimates first give decay $e^{-ct}$ for any fixed $c<1/3$. Choose $1/6<c<1/3$; then the remainder is $O(e^{-2ct})$, and its Duhamel convolution with $e^{-(t-s)/3}$ is $O(e^{-t/3})$ because $2c>1/3$. This sharpens the preliminary bound to the displayed rate. Special initial data with no slow-mode component may decay faster, but the general estimate cannot be improved uniformly.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
