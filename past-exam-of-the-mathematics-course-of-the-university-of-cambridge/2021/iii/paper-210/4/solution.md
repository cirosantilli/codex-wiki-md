<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [total variation distance](../../../../../total-variation-distance.md) is

$$
\operatorname{TV}(P,Q)=\sup_{A\in\mathcal A}|P(A)-Q(A)|.
$$

If $P\ll Q$, the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is

$$
D_{\mathrm{KL}}(P\Vert Q)
=\int\log\left(\frac{dP}{dQ}\right)dP.
$$

[Pinsker's inequality](../../../../../pinsker-s-inequality.md) states

$$
\operatorname{TV}(P,Q)
\leq\sqrt{\frac12D_{\mathrm{KL}}(P\Vert Q)}.
$$

The squared-loss [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) says that for two experiments $P_0,P_1$ with scalar parameters $\theta_0,\theta_1$,

$$
\inf_{\widehat\theta}\max_{j=0,1}
\mathbb E_j(\widehat\theta-\theta_j)^2
\geq
\frac{(\theta_1-\theta_0)^2}{8}
\{1-\operatorname{TV}(P_0,P_1)\}.
$$

Indeed, classify the data as $0$ when $\widehat\theta$ is closer to $\theta_0$ and as $1$ otherwise. On a classification error, the estimation error is at least $|\theta_1-\theta_0|/2$. The sum of the two testing error probabilities is at least $1-\operatorname{TV}(P_0,P_1)$. Averaging the two risks and then bounding their maximum proves the result.

Let $r=\lfloor\beta\rfloor$. The [Hölder class](../../../../../holder-class.md) $\mathcal H(\beta,L)$ on $[0,1]$ consists of functions with derivatives through order $r$ whose $r$th derivative is Hölder of order $\beta-r$ with constant $L$, with the standard integer-order convention.

Fix any $x_0\in[0,1]$. First compare the constant regression functions $m_0=0$ and $m_1=a$ with $a=c_0n^{-1/2}$. Both belong to every Hölder class under the seminorm convention, and the normal-product divergence is

$$
D_{\mathrm{KL}}(P_{m_1}\Vert P_{m_0})
=\frac12\sum_{i=1}^nm_1(x_i)^2
=\frac{c_0^2}{2}.
$$

Pinsker and Le Cam therefore give a lower bound $c/n$.

For the smoothness-dependent term, use the supplied smooth bump $\psi(u)=e^{-1/(1-u^2)}\mathbf1_{\{|u|\leq1\}}$, translated one-sidedly near a boundary when necessary, and compare

$$
m_0=0,\qquad
m_1(x)=a\psi\left(\frac{x-x_0}{h}\right).
$$

Choose its fixed normalization so that $m_1\in\mathcal H(\beta,L)$ whenever $a\leq c_1Lh^\beta$. The Gaussian divergence satisfies

$$
D_{\mathrm{KL}}(P_{m_1}\Vert P_{m_0})
=\frac12\sum_{i=1}^nm_1(x_i)^2
\leq Cna^2h.
$$

Take

$$
h\asymp(nL^2)^{-1/(2\beta+1)},
\qquad
a\asymp Lh^\beta,
$$

with the bandwidth and amplitude truncated at constants when this expression leaves $[0,1]$. Then the divergence remains bounded and

$$
|m_1(x_0)-m_0(x_0)|^2
\asymp
\min\left\{
\frac{L^{2/(2\beta+1)}}{n^{2\beta/(2\beta+1)}},1
\right\}.
$$

The same construction can be placed at every $x_0$, with a one-sided bump at the endpoints. Pinsker and Le Cam, combined with the constant alternatives, prove

$$
\boxed{
\inf_{x_0\in[0,1]}\inf_{\widehat\theta_n}
\sup_{m\in\mathcal H(\beta,L)}
\mathbb E\{\widehat\theta_n-m(x_0)\}^2
\geq c
\max\left\{
\frac1n,
\min\left(
\frac{L^{2/(2\beta+1)}}{n^{2\beta/(2\beta+1)}},1
\right)
\right\}},
$$

where $c>0$ depends only on $\beta$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
