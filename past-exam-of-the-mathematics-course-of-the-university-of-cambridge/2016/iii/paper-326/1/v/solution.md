<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [Volterra integration operator](../../../../../../volterra-operator.md) is injective and has dense range. Its [range of the Volterra integration operator](../../../../../../range-of-the-volterra-integration-operator.md) is $\{f\in H^1(0,1):f(0)=0\}$, and its [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) is differentiation on this domain. Thus the error estimate for $K^\dagger f$ implicitly requires $f(0)=0$, in addition to the printed $H^2$ assumption. For an arbitrary $H^2$ function the same calculation bounds error against $f'$, but that function need not be in $\mathcal D(K^\dagger)$.

Put $a=(1-\alpha)/2$, $b=(1+\alpha)/2$ and $h=\alpha/2$. The three stencils are forward, [central finite differences](../../../../../../central-finite-difference.md), and backward on $[0,a)$, $[a,b)$ and $[b,1]$, respectively. All shifted evaluation points lie in $[0,1]$. For $g\in L^2(0,1)$, apply $|A-B|^2\leq2(|A|^2+|B|^2)$ and change variables in each of the six evaluation terms. The resulting integration intervals are

$$
[\alpha,b],\quad[0,a],\quad[1/2,1/2+\alpha],\quad[1/2-\alpha,1/2],\quad[b,1],\quad[a,1-\alpha].
$$

Pair $[0,a]$ with $[a,1-\alpha]$, $[\alpha,b]$ with $[b,1]$, and the two middle intervals. Each pair has disjoint interiors, so almost every point is counted at most three times. This [overlap multiplicity bound for piecewise difference operators](../../../../../../overlap-multiplicity-bound-for-piecewise-difference-operators.md) proves

$$
\|R_\alpha g\|_2^2\leq\frac6{\alpha^2}\|g\|_2^2,\qquad \|R_\alpha\|\leq\frac{\sqrt6}{\alpha}.
$$

For the bias on the middle interval, write the [central finite difference](../../../../../../central-finite-difference.md) as an average of $f'$. The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
R_\alpha f(x)-f'(x)=\int_{-h}^h k_\alpha(s)f''(x+s)\,ds,\qquad k_\alpha(s)=\frac{\operatorname{sgn}(s)(h-|s|)}{\alpha},
$$

where $\|k_\alpha\|_1=\alpha/4$. Extend $f''$ by zero to the [real line](../../../../../../real-line.md). [Young's convolution inequality](../../../../../../young-s-convolution-inequality.md) bounds the middle-interval $L^2$ error by $\alpha c/4$. Combining its squared error with the supplied outer-interval estimate gives the [central-difference noise-bias bound](../../../../../../central-difference-noise-bias-bound.md)

$$
\|R_\alpha f-f'\|_2\leq\sqrt{\alpha^2c^2+\alpha^2c^2/16}=\frac{\sqrt{17}}4\alpha c.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) and the [operator norm](../../../../../../operator-norm.md) estimate now give

$$
\boxed{\|K^\dagger f-R_\alpha f^\delta\|_2\leq\frac{\sqrt6\,\delta}{\alpha}+\frac{\sqrt{17}}4\alpha c.}
$$

For $c>0$, [balancing noise and approximation bias](../../../../../../balancing-noise-and-approximation-bias.md) minimizes this upper bound at

$$
\boxed{\alpha(\delta)=2(6/17)^{1/4}\sqrt{\delta/c},\qquad \|K^\dagger f-R_{\alpha(\delta)}f^\delta\|_2\leq102^{1/4}\sqrt{\delta c},}
$$

for sufficiently small $\delta$ that $\alpha<1/2$. Capping the parameter at $1/4$ supplies an admissible rule for all positive noise levels. More generally, $\alpha\to0$ and $\delta/\alpha\to0$ suffice; $\alpha=\sqrt\delta$ avoids needing $c$ or dividing by $c=0$.

To prove convergence for every admissible datum, not just $H^2$ data, let $f=Ku$ with $u\in L^2(0,1)$ and extend $u$ by zero. Each stencil is a forward, centred or backward average of $u$. [Translation continuity in Lp](../../../../../../translation-continuity-in-lp.md) makes each averaged difference from $u$ tend to zero in $L^2(\mathbb R)$. Restricting those three bounds to their respective intervals proves $R_\alpha Ku\to u$. The [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md), with $\delta/\alpha\to0$, finishes the [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
