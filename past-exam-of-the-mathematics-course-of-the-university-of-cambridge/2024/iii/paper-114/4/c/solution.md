<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\alpha=pa+qb$. In the [Gysin sequence of a sphere bundle](../../../../../../gysin-sequence-of-a-sphere-bundle.md) for the oriented circle bundle $S(E_\alpha)\to S^2\times S^2$, multiplication by $\alpha$ is

$$
\mathbb Z\longrightarrow\mathbb Z^2,qquad1\longmapsto(p,q),
$$

in degrees $0$ to $2$, and

$$
\mathbb Z^2\longrightarrow\mathbb Z,qquad(u,v)\longmapsto qu+pv,
$$

in degrees $2$ to $4$. If $\alpha\neq0$ and $d=\gcd(|p|,|q|)$, taking the relevant kernels and cokernels gives

$$
\boxed{H^i(S(E_\alpha);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,3,5,\\
\mathbb Z\oplus\mathbb Z/d,&i=2,\\
\mathbb Z/d,&i=4,\\
0,&\text{otherwise}.
\end{cases}}
$$

When $\alpha=0$, the bundle is trivial and the groups in degrees $0$ through $5$ have ranks $1,1,2,2,1,1$, respectively. These are precisely the groups recorded in [integral cohomology of a circle bundle over a product of two spheres](../../../../../../integral-cohomology-of-a-circle-bundle-over-a-product-of-two-spheres.md).

The additive cohomology for nonzero $\alpha$ depends only on $d$. On the other hand, part (a) shows that the homeomorphism group acts on $(p,q)$ only by signed permutations. For example, $(1,0)$ and $(1,1)$ both have $d=1$, so their sphere bundles have isomorphic additive cohomology, but no signed permutation carries one Euler class to the other. The cohomology therefore does not determine the homeomorphism-group orbit of $\alpha$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
