<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Record the discount level at the start of each policy year as the state. A [no claims discount system](../../../../../no-claims-discount-system.md) is a [discrete-time Markov chain](../../../../../discrete-time-markov-chain.md) when, conditional on this state, the next year's claim behavior and update rule do not depend on earlier history. Independent annual accident and loss mechanisms with a fixed state-based reporting rule give this property; one should not equate the probability of an accident with the probability of a submitted claim.

The density identifies $Z=(\log L-\mu)/\sigma$ as a [standard normal random variable](../../../../../standard-normal-random-variable.md): substitute $x=e^{\mu+\sigma z}$ and $dx=\sigma x\,dz$. Therefore, for $a>0$,

$$
\boxed{\mathbb P(L>a)=1-\Phi\left(\frac{\log a-\mu}{\sigma}\right).}
$$

Here $L$ is the numerical repair cost. The character preceding $L$ in the PDF is a currency symbol, not a separate multiplier.

Order states as $0\%,20\%,30\%$. With the stipulated common annual probability $p$ of no submitted claims, the [transition matrix](../../../../../stochastic-matrix.md) is

$$
\boxed{P=\begin{pmatrix}
1-p&p&0\\
1-p&0&p\\
1-p&0&p
\end{pmatrix}.}
$$

A claim resets any state to zero, while a no-claim year raises the discount one level or keeps the top level fixed. If claim probabilities depend on the state, the corresponding row instead uses $p_i=\mathbb P(\text{no submitted claim}\mid\text{state }i)$; the same transition mechanism applies. The supplied single $p$ is a simplifying model assumption.

For a policyholder currently at zero discount, the current premium $C$ has the same value under either decision and cancels in the comparison. If the repair is self-funded and no later accidents occur, the next two premiums are $0.8C$ and $0.7C$, giving a total cost $L+2.5C$ including the current premium. If a claim is made, the next two premiums are $C$ and $0.8C$, giving total cost $2.8C$, with the repair paid by the insurer. Thus the [two-year no-claims threshold with reset to zero](../../../../../two-year-no-claims-threshold-with-reset-to-zero.md) is

$$
\boxed{L>0.3C.}
$$

At equality the holder is indifferent; it has probability zero under the continuous density. This assumes full reimbursement and no excess or deductible, as in the stated model.

Put $a=0.3C$. The conditional expected claim is $\mathbb E[L\mid L>a]$. Completing the square in the normal integral gives the [truncated lognormal moment](../../../../../truncated-lognormal-moment.md)

$$
\mathbb E[L\mathbf1_{\{L>a\}}]
=\int_{z_a}^{\infty}e^{\mu+\sigma z}\frac{e^{-z^2/2}}{\sqrt{2\pi}}\,dz
=e^{\mu+\sigma^2/2}\left[1-\Phi(z_a-\sigma)\right],\qquad z_a=\frac{\log a-\mu}{\sigma}.
$$

Dividing by the reporting probability gives **the expected size of a submitted claim for the full-premium holder**:

$$
\boxed{\mathbb E[L\mid\text{claim}]=e^{\mu+\sigma^2/2}
\frac{1-\Phi\left((\log(0.3C)-\mu-\sigma^2)/\sigma\right)}
{1-\Phi\left((\log(0.3C)-\mu)/\sigma\right)}.}
$$

All monetary amounts must use the same unit despite the PDF's mixed currency notation. The other two current levels both have next-two-year no-claim premiums $0.7C+0.7C$, versus $C+0.8C$ after a claim, so their thresholds are $0.4C$. Consequently incorporating this behavioral decision into claim probabilities generally produces state-specific $p_i$, rather than deriving a common $p$ from the severity density alone; no accident-frequency law is provided.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
