<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $K(u,f)=\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\alpha}(B_1)}$; the paper's $|u|_{2;B_1}$ denotes a $C^2$ norm, not an $L^2$ norm. We use a [blow-up compactness proof of an interior Schauder estimate](../../../../../blow-up-compactness-proof-of-an-interior-schauder-estimate.md). If the estimate failed for fixed $\delta>0$, normalization would produce

$$
[D^2u_j]_{\alpha;B_{1/2}}=1,\qquad [D^2u_j]_{\alpha;B_1}<\delta^{-1},
\qquad K(u_j,f_j)\to0.
$$

Choose $x_j,y_j\in B_{1/2}$ with $d_j=|y_j-x_j|$ and $|D^2u_j(y_j)-D^2u_j(x_j)|\geq\tfrac12d_j^\alpha$. Since $\|D^2u_j\|_\infty\to0$, necessarily $d_j\to0$. Subtract the quadratic [Taylor polynomial](../../../../../taylor-polynomial.md) $P_j$ at $x_j$ and set

$$
w_j(z)=\frac{u_j(x_j+d_jz)-P_j(x_j+d_jz)}{d_j^{2+\alpha}}.
$$

The domains expand to $\mathbb R^n$. At zero, $w_j,Dw_j,D^2w_j$ vanish; the [Hölder seminorm](../../../../../holder-seminorm.md) of $D^2w_j$ is at most $\delta^{-1}$. Integration along segments gives uniform $C^{2,\alpha}$ bounds on each fixed ball. Also

$$
\Delta w_j(z)=\frac{f_j(x_j+d_jz)-f_j(x_j)}{d_j^\alpha}\to0
$$

locally uniformly, since $[f_j]_\alpha\to0$. By [compact embedding of Hölder spaces](../../../../../compact-embedding-of-holder-spaces.md) and a diagonal subsequence, $w_j$ converges locally in $C^{2,\beta}$ to an entire [harmonic function](../../../../../harmonic-function.md) $w$, with $[D^2w]_\alpha\leq\delta^{-1}$ and $D^2w(0)=0$. The unit vectors $(y_j-x_j)/d_j$ have a convergent subsequence; its limit $e$ satisfies $|D^2w(e)|\geq1/2$.

Each second derivative of $w$ is an entire [harmonic function](../../../../../harmonic-function.md) with finite global [Hölder seminorm](../../../../../holder-seminorm.md). The supplied [polynomial-growth Liouville theorem for harmonic functions](../../../../../polynomial-growth-liouville-theorem-for-harmonic-functions.md), at growth exponent $\alpha<1$, makes it constant, and its value at zero makes it zero. This contradicts the nonzero Hessian at $e$, proving the estimate with the small $\delta$ term.

To remove that term, rescale the estimate to all contained balls and apply the [Simon absorption lemma](../../../../../simon-absorption-lemma.md). Explicitly, with $d(x)=1-|x|$ and $d_{xy}=\min(d(x),d(y))$, define

$$
M=\sup_{x\ne y\in B_1}d_{xy}^{2+\alpha}
\frac{|D^2u(x)-D^2u(y)|}{|x-y|^\alpha}.
$$

For $|x-y|<d_{xy}/8$, apply the rescaled estimate on $B_{d(x)/2}(x)$; its larger-ball seminorm is controlled by $M$ because all points there have boundary distance at least $d(x)/2$. For more separated pairs use $2\|D^2u\|_\infty$. The result is $M\leq C_0\delta M+C_\delta K(u,f)$. Choose $C_0\delta<1/2$ and use $d_{xy}\geq1/2$ on $B_{1/2}$ to obtain

$$
\boxed{[D^2u]_{\alpha;B_{1/2}}
\leq C(n,\alpha)\bigl(\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\alpha}(B_1)}\bigr).}
$$

The forcing's [Hölder seminorm](../../../../../holder-seminorm.md) cannot be discarded. For integers $k\to\infty$, take

$$
\boxed{u_k(x)=k^{-2}\sin(kx_1),\qquad f_k(x)=-\sin(kx_1).}
$$

Their $C^2$ and forcing supremum norms stay bounded, but the $11$ entry of the [Hessian matrix](../../../../../hessian-matrix.md) differs by two at $x_1=\pm\pi/(2k)$, giving $[D^2u_k]_{\alpha;B_{1/2}}\geq2(k/\pi)^\alpha\to\infty$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 107](../../paper-107-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
