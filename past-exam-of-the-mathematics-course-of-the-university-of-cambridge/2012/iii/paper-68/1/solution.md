<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $D_j=-i\partial_{x_j}$ and $\langle\xi\rangle=(1+|\xi|^2)^{1/2}$, so the [Fourier transform](../../../../../fourier-transform.md) of $P(D)u$ is $P(\xi)\widehat u(\xi)$. Write $P_N$ for the homogeneous degree-$N$ part. An [elliptic differential operator](../../../../../elliptic-differential-operator.md) has $P_N(\xi)\ne0$ for every real $\xi\ne0$. By [continuity](../../../../../continuous-function.md) on the [unit sphere](../../../../../unit-sphere.md), $m=\min_{|\omega|=1}|P_N(\omega)|>0$. The lower-degree terms are bounded by $C|\xi|^{N-1}$ for $|\xi|\geq1$, whence

$$
|P(\xi)|\geq m|\xi|^N-C|\xi|^{N-1}\geq\frac m2|\xi|^N\geq c\langle\xi\rangle^N
$$

for sufficiently large $|\xi|$. This proves the [high-frequency lower bound for an elliptic polynomial](../../../../../high-frequency-lower-bound-for-an-elliptic-polynomial.md). Degree zero just means a nonzero constant and has no [derivative](../../../../../derivative.md) gain.

With the Fourier convention in Question 3, the [Sobolev space](../../../../../sobolev-space-split.md) is

$$
\boxed{H^s(\mathbb R^n)=\{u\in\mathcal S':\langle\xi\rangle^s\widehat u\in L^2\},\qquad\|u\|_{H^s}^2=(2\pi)^{-n}\int\langle\xi\rangle^{2s}|\widehat u(\xi)|^2d\xi.}
$$

The condition includes that the weighted transform is represented by an $L^2$ function. For open $X$, the [Local Sobolev space](../../../../../local-sobolev-space.md) consists of $u\in\mathcal D'(X)$ for which $\chi u$, extended by zero, belongs to $H^s(\mathbb R^n)$ for every $\chi\in C_c^\infty(X)$. We use the elementary [Sobolev multiplication by a smooth cutoff](../../../../../sobolev-multiplication-by-a-smooth-cutoff.md) fact for every real $s$. It follows from Fourier [convolution](../../../../../convolution.md) with the rapidly decreasing $\widehat\chi$, the weighted inequality $\langle\xi\rangle^s\lesssim\langle\xi-\eta\rangle^{|s|}\langle\eta\rangle^s$, and the $L^1*L^2\to L^2$ [convolution](../../../../../convolution.md) bound.

For a [compactly supported distribution](../../../../../compactly-supported-distribution.md), [continuity](../../../../../continuous-function.md) on [test functions](../../../../../test-function.md) supported in a fixed compact neighborhood gives finite order: for some integer $M$,

$$
|\langle u,\varphi\rangle|\leq C\max_{|\alpha|\leq M}\sup_K|\partial^\alpha\varphi|.
$$

Insert a compact smooth [cutoff function](../../../../../cutoff-function.md) equal to one near the support, times $e^{-ix\cdot\xi}$. The resulting [Fourier transform](../../../../../fourier-transform.md) is smooth and satisfies $|\widehat u(\xi)|\leq C'\langle\xi\rangle^M$. The [distribution](../../../../../distribution-mathematical-analysis.md) is also tempered by this same finite-order bound. Thus

$$
\boxed{u\in H^t(\mathbb R^n)\quad\text{whenever }t<-M-n/2.}
$$

Indeed the square of the weighted bound is integrable exactly when $2(t+M)<-n$. This is [negative Sobolev regularity of a compactly supported distribution](../../../../../negative-sobolev-regularity-of-a-compactly-supported-distribution.md).

We next prove local regularity by a [high-frequency reciprocal parametrix kernel](../../../../../high-frequency-reciprocal-parametrix-kernel.md), including its off-diagonal smoothing property. Choose $\psi\in C_c^\infty(\mathbb R^n)$ equal to one on a ball containing all real zeros of $P$, and put $b(\xi)=(1-\psi(\xi))/P(\xi)$, defining it smoothly as zero in the inner ball. Differentiation of the reciprocal and the elliptic lower bound give

$$
|\partial_\xi^\alpha b(\xi)|\leq C_\alpha\langle\xi\rangle^{-N-|\alpha|}.
$$

The [Fourier multiplier](../../../../../fourier-multiplier.md) $E=b(D)$ maps $H^s$ to $H^{s+N}$ by its zeroth-order bound, and

$$
EP(D)=P(D)E=1-R,\qquad R=\psi(D).
$$

The kernel $K=\mathcal F^{-1}b$ is smooth away from the origin: for $x\ne0$, repeatedly integrate by parts using $e^{ix\cdot\xi}=(i|x|^2)^{-1}x\cdot\partial_\xi e^{ix\cdot\xi}$. After sufficiently many integrations, the differentiated symbol is integrable. For any desired $x$ [derivative](../../../../../derivative.md), repeat the argument with the additional [polynomial](../../../../../polynomial-split.md) $\xi^\beta$. A large-radius [cutoff function](../../../../../cutoff-function.md) justifies each step and its removal uniformly on compact sets away from zero. Thus [convolution](../../../../../convolution.md) by $K$ carries a [compactly supported distribution](../../../../../compactly-supported-distribution.md) to a smooth function at points separated from its support. Also $R$ carries a [compactly supported distribution](../../../../../compactly-supported-distribution.md) to a [Schwartz function](../../../../../schwartz-function.md), because $\psi\widehat u$ is smooth with compact support.

For a target compact set in $X$, choose $\chi\in C_c^\infty(X)$ equal to one on a neighborhood of it. Then $\chi u$ and $[P(D),\chi]u$ have compact support, and the commutator is supported where [derivatives](../../../../../derivative.md) of $\chi$ occur, away from the target. The [parametrix](../../../../../parametrix.md) identity gives

$$
\chi u=E[\chi P(D)u]+E[[P(D),\chi]u]+R(\chi u).
$$

The first term is in $H^{s+N}$ since $\chi P(D)u\in H^s$. The other two terms are smooth near the target by the proved kernel property. Since the target was arbitrary,

$$
\boxed{P(D)u\in H^s_{\mathrm{loc}}(X)\Longrightarrow u\in H^{s+N}_{\mathrm{loc}}(X).}
$$

This proof does not discard the [cutoff function](../../../../../cutoff-function.md) commutator; it places its support away from the set where regularity is sought.

For the final [polynomial](../../../../../polynomial-split.md), select a multi-index $\alpha_0$ with $|\alpha_0|=N$ and $\partial^{\alpha_0}Q$ a nonzero constant. The derivative-ratio hypothesis immediately gives $|Q(\xi)|\geq c|\xi|^{\delta N}$ at large frequency. In particular $Q$ has no real zero there. For $N>0$, its degree bound also forces $\delta\leq1$. Differentiating $1/Q$ gives products of ratios $\partial^\beta Q/Q$, whose total [derivative](../../../../../derivative.md) order is $|\alpha|$. Hence the corresponding high-frequency reciprocal satisfies

$$
|\partial_\xi^\alpha b_Q(\xi)|\leq C_\alpha\langle\xi\rangle^{-\delta N-\delta|\alpha|}.
$$

Its multiplier maps $H^s$ to $H^{s+\delta N}$. Its kernel is still smooth off zero: each frequency [integration by parts](../../../../../integration-by-parts.md) now lowers the order by $\delta$, so more iterations may be needed, but $\delta>0$ supplies arbitrarily much decay. The same separated-support commutator identity applies without a change. The [derivative-ratio Sobolev gain for a polynomial operator](../../../../../derivative-ratio-sobolev-gain-for-a-polynomial-operator.md) is therefore

$$
\boxed{Q(D)u\in H^s_{\mathrm{loc}}(X)\Longrightarrow u\in H^{s+\delta N}_{\mathrm{loc}}(X).}
$$

Simply estimating the commutator by its differential order would lose this sharper gain; the off-diagonal kernel argument uses the full derivative-ratio hypothesis.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
