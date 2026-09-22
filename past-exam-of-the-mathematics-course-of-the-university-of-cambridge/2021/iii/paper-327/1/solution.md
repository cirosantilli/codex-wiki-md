<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [space of test functions](../../../../../space-of-test-functions.md) is

$$
\mathcal D(\mathbb R)=C_c^\infty(\mathbb R).
$$

A sequence $\varphi_m$ converges to $\varphi$ in $\mathcal D(\mathbb R)$ when all supports lie in one [compact set](../../../../../compact-space.md) $K$ and

$$
\sup_{x\in K}|\varphi_m^{(j)}(x)-\varphi^{(j)}(x)|\longrightarrow0
$$

for every [nonnegative integer](../../../../../natural-number.md) $j$. The [distribution](../../../../../distribution-mathematical-analysis.md) space $\mathcal D'(\mathbb R)$ is the [continuous dual space](../../../../../continuous-dual-space-split.md) of $\mathcal D(\mathbb R)$, and $u_m\to u$ in $\mathcal D'$ means

$$
\langle u_m,\varphi\rangle\longrightarrow\langle u,\varphi\rangle
$$

for every test function $\varphi$.

If a linear form $u$ is continuous, it clearly maps every [null sequence](../../../../../null-sequence.md) to a scalar sequence tending to zero. Conversely, suppose it has this sequential property. For each compact $K$, its restriction to the [Fréchet space](../../../../../frechet-space.md) $\mathcal D_K$ must be continuous: otherwise, for every $m$ one could choose $\varphi_m\in\mathcal D_K$ such that

$$
\max_{0\leq j\leq m}\|\varphi_m^{(j)}\|_\infty\leq\frac1m,
\qquad
|\langle u,\varphi_m\rangle|\geq1.
$$

Then $\varphi_m\to0$ in $\mathcal D$ but its images do not tend to zero, a contradiction. Continuity on every $\mathcal D_K$ is precisely continuity for the [strict inductive limit topology](../../../../../strict-inductive-limit-topology.md) of $\mathcal D$, so $u\in\mathcal D'$.

Use the convention $\tau_h\varphi(x)=\varphi(x-h)$. Translation and the [distributional derivative](../../../../../distributional-derivative.md) are defined by

$$
\langle\tau_hu,\varphi\rangle
=\langle u,\tau_{-h}\varphi\rangle,
\qquad
\langle u',\varphi\rangle=-\langle u,\varphi'\rangle.
$$

Translation, differentiation, and multiplication by $-1$ are continuous maps on $\mathcal D$, so these formulas define continuous linear functionals and hence distributions.

For fixed $\varphi$, the [difference quotient](../../../../../difference-quotient.md) satisfies

$$
\frac{\tau_h\varphi-\varphi}{h}\longrightarrow-\varphi'
\quad\text{in }\mathcal D.
$$

Therefore

$$
\left\langle\frac{\tau_{-h}u-u}{h},\varphi\right\rangle
=\left\langle u,\frac{\tau_h\varphi-\varphi}{h}\right\rangle
\longrightarrow-\langle u,\varphi'\rangle
=\langle u',\varphi\rangle,
$$

which proves $u'=\lim_{h\to0}(\tau_{-h}u-u)/h$ in $\mathcal D'$.

For $-1<\lambda<0$, integration by parts after subtracting the value at zero gives

$$
\boxed{
\langle(x_+^\lambda)',\varphi\rangle
=\int_0^\infty[\varphi(x)-\varphi(0)]\lambda x^{\lambda-1}\,dx}.
$$

The subtraction makes the integrand locally integrable at zero, and $x^\lambda\to0$ handles the other boundary.

The analogous [Hadamard finite-part integral](../../../../../hadamard-finite-part-integral.md) is

$$
\boxed{
\langle(\log x_+)',\varphi\rangle
=\int_0^1\frac{\varphi(x)-\varphi(0)}x\,dx
+\int_1^\infty\frac{\varphi(x)}x\,dx}.
$$

Indeed, integrating from $\varepsilon$ and combining the boundary term $\varphi(\varepsilon)\log\varepsilon$ with the divergent constant part of the integral gives this limit.

Because $x_+^\lambda$ is a [locally integrable function](../../../../../locally-integrable-function.md), its first distributional derivative has order at most one. It is not of order zero. Choose $\psi\in\mathcal D((0,1))$ with $\int_0^1\lambda t^{\lambda-1}\psi(t)\,dt\ne0$ and put $\psi_\varepsilon(x)=\psi(x/\varepsilon)$. The sup norms stay bounded while

$$
\langle(x_+^\lambda)',\psi_\varepsilon\rangle
=\varepsilon^\lambda
\int_0^1\lambda t^{\lambda-1}\psi(t)\,dt
$$

is unbounded as $\varepsilon\downarrow0$. This contradicts the local sup-norm estimate required of an [order-zero distribution](../../../../../order-zero-distribution.md). Hence $(x_+^\lambda)'$ has order exactly $\boxed{1}$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
