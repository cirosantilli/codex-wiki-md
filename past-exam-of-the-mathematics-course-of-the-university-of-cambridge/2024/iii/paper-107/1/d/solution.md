<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [interior Schauder estimate](../../../../../../interior-schauder-estimate.md) is

$$
\boxed{\|u\|_{C^{2,\alpha}(B_{1/2})}
\leq C\left(\|u\|_{C^0(B_1)}+
\|f\|_{C^{0,\alpha}(B_1)}\right),}
$$

where $C$ depends only on $n$, $\alpha$, the ellipticity constant, and the stated coefficient bounds.

It is enough first to prove the estimate for the Hölder seminorm of $D^2u$. The [Interpolation inequality in Holder spaces](../../../../../../interpolation-inequality-in-holder-spaces.md) controls $Du$ and $D^2u$ by a small multiple of $[D^2u]_{\alpha}$ plus $\|u\|_0$; the small term is later absorbed. Freezing $a^{ij}$ at the centre of each ball and moving coefficient differences and lower-order terms to the right reduces the local estimate to

$$
r^{2+\alpha}[D^2u]_{\alpha;B_{r/2}}
\leq \varepsilon r^{2+\alpha}[D^2u]_{\alpha;B_r}
+C\left(\|u\|_{0;B_r}+r^2\|f\|_{0,\alpha;B_r}\right).
$$

Once this is known, the [Simon absorption lemma](../../../../../../simon-absorption-lemma.md) gives the desired estimate on $B_{1/2}$.

For completeness, prove the frozen-coefficient estimate by contradiction. If it failed, choose solutions $u_k$, points $x_k$, and scales $\rho_k\downarrow0$ at which the scale-invariant Hölder quotient is almost maximal. Let $q_k$ be the quadratic Taylor polynomial of $u_k$ at $x_k$ and define

$$
v_k(y)=
\frac{u_k(x_k+\rho_ky)-q_k(x_k+\rho_ky)}
{\rho_k^{2+\alpha}[D^2u_k]_{\alpha}}.
$$

Then $v_k(0)=Dv_k(0)=D^2v_k(0)=0$, the Hessians have uniformly bounded local $C^{0,\alpha}$ seminorms, and the normalization makes their oscillation nonzero on a fixed ball. The localized equation is

$$
\widetilde a_k^{ij}D_{ij}v_k=g_k,
$$

where the coefficient matrices converge locally uniformly to one constant positive-definite matrix and the given normalized error $g_k$ tends locally uniformly to zero.

The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) produces a locally $C^2$ convergent subsequence with limit $v$ satisfying a constant-coefficient elliptic equation on $\mathbb R^n$. A linear rotation and scaling turn it into a [harmonic function](../../../../../../harmonic-function.md). The normalization gives $D^2v(0)=0$ but a nonconstant Hessian, while maximality of the scaled quotient gives growth at most $C(1+|y|^{2+\alpha})$. Applying the [Liouville theorem](../../../../../../liouville-theorem.md) to derivatives shows that every second derivative is constant because $0<\alpha<1$. This contradicts the normalized Hessian oscillation. The frozen estimate follows, and interpolation plus absorption completes the proof.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
