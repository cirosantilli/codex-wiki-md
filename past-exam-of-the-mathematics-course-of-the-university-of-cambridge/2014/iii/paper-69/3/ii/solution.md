<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a consistent number $n$ of vertices, with $z_{n+1}=z_1$, and set $m_j=(z_j+z_{j+1})/2$, $h_j=(z_{j+1}-z_j)/2$. Pull back the [one-form](../../../../../../one-form.md) to $z_j(s)=m_j+sh_j$. Since $dz=h_jds$ and $d\bar z=\bar h_jds$, the side integrand is

$$
\boxed{W_j(s,\lambda)=e^{-i\beta[\lambda(m_j+sh_j)-(\bar m_j+s\bar h_j)/\lambda]}
\left[h_ju_z-\bar h_ju_{\bar z}
+i\beta(\lambda h_j+\bar h_j/\lambda)u\right]_{z=m_j+sh_j}.}
$$

For counterclockwise traversal, put $\ell_j=|h_j|$ and let $q_j=\partial_nu$ be the outward [normal derivative](../../../../../../normal-derivative.md), while $g_j=u|_{S_j}$ is the [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md). The outward unit normal is $-ih_j/\ell_j$ in complex notation. Therefore $h_ju_z-\bar h_ju_{\bar z}=i\ell_jq_j$, and

$$
\boxed{W_j=i e^{-i\beta[\lambda(m_j+sh_j)-(\bar m_j+s\bar h_j)/\lambda]}
\left[\ell_jq_j(s)+\beta(\lambda h_j+\bar h_j/\lambda)g_j(s)\right].}
$$

There is no tangential-derivative term: it cancels in this particular [one-form](../../../../../../one-form.md). The [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) and $dW=0$ now give the polygonal [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
\boxed{\sum_{j=1}^n\int_{-1}^1W_j(s,\lambda)\,ds=0,\qquad\lambda\ne0.}
$$

The same zero identity holds with every side traversed clockwise, but then $h_ju_z-\bar h_ju_{\bar z}=-i\ell_jq_j$ for outward normals. One must change this sign consistently rather than mix the two orientations.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
