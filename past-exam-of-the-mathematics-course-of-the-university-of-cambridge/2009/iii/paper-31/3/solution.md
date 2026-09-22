<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On the real line, **[Prohorov's theorem](../../../../../prokhorov-s-theorem.md)** states that a sequence of [probability measures](../../../../../probability-measure.md) is [uniformly tight](../../../../../uniform-tightness.md) if and only if every subsequence has a further subsequence converging weakly to a [probability measure](../../../../../probability-measure.md). Here [uniformly tight](../../../../../uniform-tightness.md) means that, for every $\varepsilon>0$, some compact interval contains mass at least $1-\varepsilon$ for every measure in the sequence. This is relative sequential compactness for [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md), not merely the existence of one convergent subsequence.

We first prove the [characteristic-function tail bound](../../../../../characteristic-function-tail-bound.md). Put $c_0=1-\sin1>0$. For $y\ne0$,

$$
\lambda\int_0^{1/\lambda}(1-\cos(uy))\,du=1-\frac{\sin(y/\lambda)}{y/\lambda}.
$$

At $y=0$ the expression is zero by continuity. If $|y|\ge\lambda$, the supplied elementary bound, with $t=|y|/\lambda$, makes it at least $c_0$. The integrand is nonnegative, so [Tonelli's theorem](../../../../../tonelli-theorem.md) yields

$$
c_0\mu(\{|y|\ge\lambda\})\le\int\lambda\int_0^{1/\lambda}(1-\cos(uy))\,du\,\mu(dy)=\lambda\int_0^{1/\lambda}(1-\operatorname{Re}\phi(u))\,du.
$$

Thus **one valid universal constant** is

$$
\boxed{C=(1-\sin1)^{-1}.}
$$

The estimate controls spatial tails using only the [characteristic function](../../../../../characteristic-function.md) near zero.

Apply it to each $\mu_n$. For fixed $\lambda$, pointwise convergence of the [characteristic functions](../../../../../characteristic-function.md) and the bound $|\phi_n|\le1$ allow [dominated convergence](../../../../../dominated-convergence-theorem.md) on the finite integration interval, giving

$$
\limsup_n\mu_n(\{|y|\ge\lambda\})\le C\lambda\int_0^{1/\lambda}(1-\operatorname{Re}\phi(u))\,du\le C\sup_{0\le u\le1/\lambda}(1-\operatorname{Re}\phi(u)).
$$

[Continuity of a characteristic function](../../../../../continuity-of-a-characteristic-function.md) and $\phi(0)=1$ make the last expression tend to zero as $\lambda\to\infty$. Given $\varepsilon>0$, choose $\lambda$ making it less than $\varepsilon/2$; then for all sufficiently large $n$, the preceding tail is less than $\varepsilon$. Enlarge the compact interval to handle the finitely many remaining [probability measures](../../../../../probability-measure.md). This proves **[uniform tightness](../../../../../uniform-tightness.md) of the whole sequence**.

By [Prohorov's theorem](../../../../../prokhorov-s-theorem.md), every subsequence has a further weakly convergent subsequence, say with limit $\nu$. The real and imaginary parts of $e^{iuy}$ are bounded continuous functions, so along that subsequence

$$
\int e^{iuy}\nu(dy)=\lim_n\phi_n(u)=\phi(u).
$$

The [uniqueness theorem for characteristic functions](../../../../../uniqueness-theorem-for-characteristic-functions.md) implies $\nu=\mu$. All subsequential weak limits are therefore $\mu$. If the original sequence failed to converge weakly to $\mu$, a bounded continuous test function and a subsequence would keep its integrals a fixed distance from the limiting integral; a further weakly convergent subsequence would contradict that. Hence

$$
\boxed{\mu_n\Rightarrow\mu.}
$$

This supplies the required proof of the [Lévy continuity theorem](../../../../../levy-continuity-theorem.md) in the stated case.

For the final request, **the printed $Q$ is not defined; the intended function is $\phi$**, the [characteristic function](../../../../../characteristic-function.md) of a summand. We prove that $\phi'(0)=ia$ without assuming integrability. Write $Y_n=S_n/n$. Independence gives $\mathbb E e^{iuY_n}=\phi(u/n)^n$. Moreover [convergence in probability](../../../../../convergence-in-probability.md) to $a$ implies uniform convergence of these [characteristic functions](../../../../../characteristic-function.md) on each bounded frequency interval: for $|u|\le T$ and $\delta>0$,

$$
\left|\mathbb E e^{iuY_n}-e^{iua}\right|\le T\delta+2\mathbb P(|Y_n-a|>\delta).
$$

First let $n\to\infty$, then $\delta\downarrow0$.

The potential logarithm-branch ambiguity needs to be resolved, not discarded. By continuity of $\phi$ near zero, its principal [complex logarithm](../../../../../complex-logarithm.md) is defined at $u/n$ for all $|u|\le1$ and all large $n$, with value zero at $u=0$. Also

$$
\Psi_n(u):=e^{-iau}\phi(u/n)^n\longrightarrow1
$$

uniformly on $[-1,1]$, so $\operatorname{Log}\Psi_n(u)\to0$ uniformly there. The two continuous logarithms differ by an integer multiple of $2\pi i$:

$$
n\operatorname{Log}\phi(u/n)-iau-\operatorname{Log}\Psi_n(u)\in2\pi i\mathbb Z.
$$

That integer is continuous in $u$ and zero at zero, hence identically zero. Consequently

$$
\sup_{|u|\le1}\bigl|n\operatorname{Log}\phi(u/n)-iau\bigr|\longrightarrow0.
$$

For arbitrary nonzero $h\to0$, take $n=\lfloor1/|h|\rfloor$ and $u=nh$. Eventually $1/2\le|u|\le1$, so dividing the preceding error by $u$ shows $\operatorname{Log}\phi(h)/h\to ia$. Exponentiating at zero proves **the derivative forced by the weak law**:

$$
\boxed{\phi'(0)=ia.}
$$

This is the [weak law forces a characteristic-function derivative](../../../../../weak-law-forces-a-characteristic-function-derivative.md) argument. Its estimates use bounded exponentials, not $\mathbb E|X_1|$. If $X_1$ is integrable, [dominated convergence](../../../../../dominated-convergence-theorem.md) permits differentiation inside the expectation and gives $\phi'(0)=i\mathbb EX_1$, so then $a=\mathbb EX_1$.

Absolute integrability is genuinely unnecessary. For an explicit [weak law without an absolute first moment](../../../../../weak-law-without-an-absolute-first-moment.md), take a symmetric variable with

$$
\mathbb P(|X|>x)=\frac1{x\log x}\quad(x\ge e),
$$

with mass $1-1/e$ at zero and no mass with $0<|X|<e$. This is a valid law: the specified tail decreases from $1/e$ to zero, and its derivative defines the continuous part beyond $e$. Its absolute first moment is infinite because $\int_e^\infty dx/(x\log x)=\infty$. For independent copies, set $Y_{n,j}=X_j\mathbf1_{\{|X_j|\le n\}}$. Symmetry gives $\mathbb EY_{n,j}=0$, and integration of the tail gives

$$
\mathbb EY_{n,j}^2\le2\int_0^n x\mathbb P(|X|>x)\,dx=O(n/\log n).
$$

For the last estimate, split the integral at $\sqrt n$; the initial part is $O(\sqrt n)$ and the remainder is at most $2n/\log n$, apart from a fixed initial constant. [Chebyshev's inequality](../../../../../chebyshev-inequality.md) now gives $n^{-1}\sum_{j\le n}Y_{n,j}\to0$ in probability. The probability that any truncation changes a summand is at most $n\mathbb P(|X|>n)=1/\log n\to0$, so $S_n/n\to0$ in probability although $\mathbb E|X|=\infty$. The derivative is zero, but the usual expectation of $X$ does not exist.

If either the positive or negative part is integrable, the finite weak-law limit does force full integrability. For example, if $\mathbb EX^-<\infty$, then $X\wedge A$ is integrable and its sample averages have the [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) limit $\mathbb E(X\wedge A)$. Since they are bounded above by the original averages, $\mathbb E(X\wedge A)\le a$ for every $A$. Letting $A\to\infty$ shows $\mathbb EX^+<\infty$. The symmetric argument handles the other one-sided hypothesis. The nonintegrable example necessarily has both one-sided expectations infinite.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
