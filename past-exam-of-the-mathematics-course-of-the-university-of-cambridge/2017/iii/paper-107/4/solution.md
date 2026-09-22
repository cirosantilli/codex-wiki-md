<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the paper's classical norm convention: $|u|_{2;U}$ is the [derivative supremum norm](../../../../../derivative-supremum-norm.md) through order two, not an $L^2$ norm. Write $H(u;U)=[D^2u]_{\alpha;U}$ and $Q(u,f)=|u|_{2;B_1}+|f|_{0,\alpha;B_1}$, where the latter is the full [Hölder norm](../../../../../holder-norm.md) of the forcing.

Fix $0<\delta<1$. If the asserted estimate failed, rescaling the functions by their global [Hessian matrix](../../../../../hessian-matrix.md) [Hölder seminorm](../../../../../holder-seminorm.md) would produce $u_j,f_j$ with

$$
H(u_j;B_1)=1,\qquad H(u_j;B_{1/2})>\delta+jQ(u_j,f_j).
$$

In particular $Q(u_j,f_j)\to0$. Choose $x_j,y_j\in B_{1/2}$ for which

$$
|D^2u_j(y_j)-D^2u_j(x_j)|>\tfrac\delta2|y_j-x_j|^\alpha.
$$

The [supremum norm](../../../../../supremum-norm.md) of $D^2u_j$ tends to zero, so $r_j=|y_j-x_j|\to0$. Let $P_j$ be the quadratic [Taylor polynomial](../../../../../taylor-polynomial.md) of $u_j$ at $x_j$, and define

$$
U_j(z)=\frac{u_j(x_j+r_jz)-P_j(x_j+r_jz)}{r_j^{2+\alpha}}.
$$

The domains contain $B_{1/(2r_j)}$, and $U_j,DU_j,D^2U_j$ vanish at zero. Moreover

$$
[D^2U_j]_{\alpha}\leq1,\qquad
\Delta U_j(z)=r_j^{-\alpha}\bigl(f_j(x_j+r_jz)-f_j(x_j)\bigr).
$$

The right side is bounded by $[f_j]_\alpha|z|^\alpha$ and tends to zero locally uniformly. The normalized [Hessian matrix](../../../../../hessian-matrix.md) bound controls $|D^2U_j(z)|\leq|z|^\alpha$; integration along line segments then bounds $DU_j,U_j$ on every compact [Euclidean ball](../../../../../euclidean-ball.md). [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) and a [diagonal subsequence argument](../../../../../diagonal-subsequence-argument.md) give convergence in $C^2$ on compact subsets to an entire [harmonic function](../../../../../harmonic-function.md) $U$, with $[D^2U]_{\alpha;\mathbb R^n}\leq1$ and $D^2U(0)=0$.

After a further subsequence $z_j=(y_j-x_j)/r_j\to z_*$ with $|z_*|=1$. The normalization ensures $|D^2U(z_*)|\geq\delta/2$. But each second derivative of $U$ is harmonic and has finite global [Hölder seminorm](../../../../../holder-seminorm.md) with exponent below one. The supplied Liouville theorem makes each derivative constant; it is the globally Hölder case of the [polynomial-growth Liouville theorem for harmonic functions](../../../../../polynomial-growth-liouville-theorem-for-harmonic-functions.md). Its value at zero makes it zero, a contradiction. This [blow-up compactness proof of an interior Schauder estimate](../../../../../blow-up-compactness-proof-of-an-interior-schauder-estimate.md) establishes

$$
\boxed{H(u;B_{1/2})\leq\delta H(u;B_1)+C_{n,\alpha,\delta}Q(u,f).}
$$

To absorb the term on the larger [Euclidean ball](../../../../../euclidean-ball.md), rescale this estimate to [Euclidean balls](../../../../../euclidean-ball.md) contained in $B_s$. For $1/2\leq r<s<1$, pairs separated by less than $(s-r)/2$ are controlled in a [Euclidean ball](../../../../../euclidean-ball.md) centred at their first point; farther pairs are controlled directly by $\|D^2u\|_\infty$. Thus

$$
H(u;B_r)\leq\delta H(u;B_s)+C_\delta(s-r)^{-2-\alpha}Q(u,f).
$$

This is the covering step in the [Simon absorption lemma](../../../../../simon-absorption-lemma.md). Take $r_j=1-2^{-j-1}$ and fix $\delta<2^{-2-\alpha}$. Iterating makes the remainder $\delta^jH(u;B_{r_j})$ tend to zero, since the global seminorm is finite; the error terms form a convergent geometric series. Consequently

$$
\boxed{[D^2u]_{\alpha;B_{1/2}}\leq C_{n,\alpha}\bigl(|u|_{2;B_1}+|f|_{0,\alpha;B_1}\bigr).}
$$

For the requested failure of the weaker estimate, take $u_m=m^{-2}\sin(mx_1)$ and $f_m=-\sin(mx_1)$. The [derivative supremum norm](../../../../../derivative-supremum-norm.md) $|u_m|_2$ and $\|f_m\|_\infty$ remain bounded, but comparison at $0$ and $\pi e_1/(2m)$, both in $B_{1/2}$ for large $m$, gives

$$
\boxed{[D^2u_m]_{\alpha;B_{1/2}}\geq(2m/\pi)^\alpha\longrightarrow\infty.}
$$

This proves the [necessity of Hölder forcing for Schauder estimates](../../../../../necessity-of-holder-forcing-for-schauder-estimates.md). Every member of the sequence is smooth; failure comes from the increasing frequency, not from any lack of individual regularity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 107](../../paper-107-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
