<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The filtered shell integral uses both signs of time, while the stated decay hypothesis controls only positive time. Here is a way to choose an even admissible [spectral filter](../../../../../../spectral-filter.md) from the given one, rather than silently assume that its negative tail is controlled. Call the supplied [spectral filter](../../../../../../spectral-filter.md) $f$. Reality and its Fourier cutoff imply that $\widehat f$ is supported in $[-\Delta,\Delta]$. It is bounded and integrable in frequency, so Fourier inversion supplies a bounded continuous representative of $f$. That representative is real analytic, since its Fourier support is compact, and is not identically zero.

Define the [evenization of a nonnegative bandlimited filter](../../../../../../evenization-of-a-nonnegative-bandlimited-filter.md) by

$$
w(t)=C f(t/2)f(-t/2),\qquad C^{-1}=\int_{\mathbb R}f(t/2)f(-t/2)dt.
$$

The normalizing integral is finite and positive: boundedness and integrability give finiteness, while a nonzero real-analytic nonnegative function cannot vanish on an interval, so the product is positive on some interval. The new [spectral filter](../../../../../../spectral-filter.md) is even, nonnegative and normalized. Each factor has Fourier support in $[-\Delta/2,\Delta/2]$, and the convolution rule for the product therefore gives support in $[-\Delta,\Delta]$, including vanishing at the outer endpoints. Its positive tail is bounded by

$$
\int_T^\infty w(t)dt\leq2C\|f\|_\infty\int_{T/2}^\infty f(u)du.
$$

It has the same required tail form, with a rescaled positive constant $\beta$. Since $w$ is even, its two-sided tail is twice its positive tail. The preceding parts use this chosen $w$ consistently.

For the [almost-exponential locality of filtered Hamiltonian terms](../../../../../../almost-exponential-locality-of-filtered-hamiltonian-terms.md), split the integral defining $A^{(Z,d)}$ at $|t|=T_d$. Write $\lambda=2ks>0$ and choose $T_d=\mu d/(2\lambda)$. On the short-time part, part (d) and $\int w=1$ give

$$
\left\|\int_{|t|\leq T_d}w(t)\bigl(\tau_t^{H_d}(h_Z)-\tau_t^{H_{d-1}}(h_Z)\bigr)dt\right\|\leq C\|h_Z\|T_d d^\alpha e^{-\mu d+\lambda T_d}=O(\|h_Z\|d^{\alpha+1}e^{-\mu d/2}).
$$

For the long-time part, each conjugated operator has norm $\|h_Z\|$, so their difference has norm at most $2\|h_Z\|$. The two-sided [spectral filter](../../../../../../spectral-filter.md) tail gives

$$
\left\|\int_{|t|>T_d}\cdots dt\right\|=O\left(\|h_Z\|(\log(\beta T_d))^2 e^{-\beta T_d/(\log(\beta T_d))^2}\right).
$$

Let $c=\beta\mu/(2\lambda)>0$, so $\beta T_d=cd$. The logarithmic prefactor is bounded by $O(d^{\alpha+1})$, and the first, exponentially decaying contribution is asymptotically smaller than this almost-exponential contribution. Therefore

$$
\boxed{\|A^{(Z,d)}\|=O\left(\|h_Z\|d^{\alpha+1}\exp\left[-\frac{cd}{(\log(cd))^2}\right]\right).}
$$

This is an asymptotic statement for large $d$; small shells have the elementary bound $2\|h_Z\|$, avoiding the meaningless substitution $cd=1$ into the logarithmic expression. If $ks=0$, there is no dynamical spreading and the shell increments vanish. **Filtering gives almost-exponentially decaying shells despite the filtered operator's potentially global support.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
