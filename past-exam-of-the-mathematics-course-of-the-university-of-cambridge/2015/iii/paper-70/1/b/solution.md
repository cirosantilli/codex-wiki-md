<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unknown [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) can be removed by the [Fokas method](../../../../../../fokas-method.md). Evaluate the [global relation for the half-line free Schrodinger equation](../../../../../../global-relation-for-the-half-line-free-schrodinger-equation.md) at $-k$:

$$
e^{ik^2t}\widehat q(-k,t)=\widehat q_0(-k)-kG_0(k,t)-iG_1(k,t).
$$

Consequently $kG_0-iG_1=2kG_0-\widehat q_0(-k)+e^{ik^2t}\widehat q(-k,t)$. In the representation from part (a), the last term has integral $\int_{\partial D_+}e^{ikx}\widehat q(-k,t)dk=0$, by the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) and [Jordan lemma](../../../../../../jordan-s-lemma.md). It is analytic in the upper half-plane, and the exponential decays on the closing first-quadrant arc. Hence an expression involving only the given data is

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-ik^2t}\widehat q_0(k)dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-ik^2t}\left[2kG_0(k,t)-\widehat q_0(-k)\right]dk.}
$$

One may replace $t$ by $T$ in the upper limit defining $G_0$: the contribution of boundary times $s>t$ closes to zero in $D_+$, since $e^{-ik^2(t-s)}$ then decays there. Using $t$ makes causality transparent.

For an explicit proof of [uniform convergence](../../../../../../uniform-convergence.md), it is useful to apply [boundary lifting](../../../../../../boundary-lifting.md) before inversion. Set $h(x)=e^{-x}$, $c=g_0(0)$, $w_0(x)=q_0(x)-ch(x)$, and

$$
S_0(k)=\int_0^\infty\sin(kx)w_0(x)dx,\qquad H(k)=\int_0^\infty\sin(kx)h(x)dx=\frac{k}{1+k^2},\qquad f(t)=ig_0(t)-g_0'(t).
$$

The compatibility condition gives $w_0(0)=0$. The [Fourier sine transform](../../../../../../fourier-sine-transform.md) of $w=q-g_0h$ satisfies $S_t+ik^2S=Hf$, with initial value $S_0$. The [integrating factor](../../../../../../integrating-factor.md) therefore gives the equivalent representation

$$
\boxed{q(x,t)=g_0(t)e^{-x}+\frac2\pi\int_0^\infty\sin(kx)\left[e^{-ik^2t}S_0(k)+\frac{k}{1+k^2}\int_0^t e^{-ik^2(t-s)}f(s)ds\right]dk.}
$$

This last integral is **absolutely and uniformly convergent for $x\geq0$, $0\leq t\leq T$** under concrete sufficient hypotheses $w_0,w_0',w_0''\in L^1$, decay of the boundary terms, and $g_0\in C^2[0,T]$. Indeed, two [integrations by parts](../../../../../../integration-by-parts.md) give $|S_0(k)|\leq\|w_0''\|_1/k^2$ for $k\geq1$. Another [integration by parts](../../../../../../integration-by-parts.md), this time in $s$, gives

$$
\left|\int_0^t e^{-ik^2(t-s)}f(s)ds\right|\leq\frac{2\|f\|_\infty+T\|f'\|_\infty}{k^2}.
$$

Thus the initial term is uniformly $O(k^{-2})$ and the forcing term uniformly $O(k^{-3})$. For $0<k<1$, use $|S_0(k)|\leq\|w_0\|_1$ and the bounded time integral. An integrable majorant proves the claimed [uniform convergence](../../../../../../uniform-convergence.md) and permits evaluation at both boundaries.

At $t=0$, [Fourier sine inversion](../../../../../../fourier-sine-inversion.md) gives $q(x,0)=ce^{-x}+w_0(x)=q_0(x)$. At $x=0$, the integral vanishes, giving $q(0,t)=g_0(t)$, including the compatible corner. To verify the equation, note that $h''=h$ and the transformed equation implies

$$
iw_t+w_{xx}=-(ig_0'+g_0)h.
$$

Adding the lifted part gives $iq_t+q_{xx}=0$. Under the stated smoothness, this holds classically in the interior; differentiated spectral integrals can first be Gaussian-regularized, or read in the sine-transform $L^2$ sense and then identified with the smooth solution. Uniform convergence of $q$ itself does not require claiming uniform convergence of every differentiated integral at the corner.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
