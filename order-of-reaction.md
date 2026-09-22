# Order of reaction

↑ **Parent:** [Rate law](rate-law.md)

In a power-form [rate law](rate-law.md) $v=k[\mathrm A]^\alpha[\mathrm B]^\beta$, the partial [orders of reaction](order-of-reaction.md) are $\alpha$ and $\beta$, and the overall [order of reaction](order-of-reaction.md) is $n=\alpha+\beta$. For example, doubling $[\mathrm A]$ at fixed $[\mathrm B]$ multiplies $v$ by $2^\alpha$: factors of one, two, and four correspond to partial [orders of reaction](order-of-reaction.md) zero, one, and two. These exponents can also be fractional or negative. A single constant [order of reaction](order-of-reaction.md) need not describe a [rate law](rate-law.md) that is not a power form. See [IUPAC Gold Book: order of reaction](https://goldbook.iupac.org/terms/view/O04322).

For a simple irreversible conversion $\mathrm A\longrightarrow\mathrm B$ with [rate equation](rate-equation.md) $-d[\mathrm A]/dt=k[\mathrm A]^n$, initial [concentration](concentration.md) $A_0>0$, and fixed $k>0$, compare [zero-order reactions](zero-order-reaction.md), [first-order reactions](first-order-reaction.md), and [second-order reactions](second-order-reaction.md) using the [dimensionless quantities](dimensionless-quantity.md)

$$
X=\frac{[\mathrm A]}{A_0},\qquad \tau=kA_0^{n-1}t,\qquad \frac{dX}{d\tau}=-X^n.
$$

Their integrated curves, starting at $X(0)=1$, are

$$
\begin{aligned}
n=0:&\quad X=1-\tau\quad(0\leq\tau<1),\\
n=1:&\quad X=e^{-\tau},\\
n=2:&\quad X=\frac1{1+\tau}.
\end{aligned}
$$

For the [zero-order reaction](zero-order-reaction.md), the plotted extension $X=\max(1-\tau,0)$ stops conversion at depletion. It does not continue to obey $dX/d\tau=-1$ once $X=0$. A negative [concentration](concentration.md) would be unphysical. The [first-order reaction](first-order-reaction.md) and [second-order reaction](second-order-reaction.md) approach zero without reaching it at finite time in these models.

<a id="image-dimensionless-concentration-decays-for-three-orders-of-reaction-with-zero-order-reaction-depletion-and-the-corresponding-linearizing-plots"></a>
![](reaction-order-concentration-curves.png)

**[Figure 13](#image-dimensionless-concentration-decays-for-three-orders-of-reaction-with-zero-order-reaction-depletion-and-the-corresponding-linearizing-plots). Dimensionless concentration decays for three orders of reaction, with zero-order reaction depletion and the corresponding linearizing plots**.

The common $\tau$ axis compares curve shapes after each model's own time rescaling, rather than equal laboratory times for an identical numerical $k$. In the lower panels, $X$, $\ln X$, and $1/X$ respectively give straight lines with slopes $-1$, $-1$, and $+1$ for the matching [order of reaction](order-of-reaction.md). The [natural logarithm](natural-logarithm.md) uses a [dimensionless quantity](dimensionless-quantity.md). These transformed plots help test a proposed [rate law](rate-law.md); the [zero-order reaction](zero-order-reaction.md) line applies only before depletion. See [Flowers et al., Chemistry 2e, §12.4: integrated rate laws](https://openstax.org/books/chemistry-2e/pages/12-4-integrated-rate-laws).

**Table of contents**

- [First-order reaction](first-order-reaction.md)
  - [First-order rate constant](first-order-rate-constant.md)
- [Zero-order reaction](zero-order-reaction.md)
- [Second-order reaction](second-order-reaction.md)
  - [Unequal-concentration second-order integration](unequal-concentration-second-order-integration.md)
  - [Conductometric saponification assay](conductometric-saponification-assay.md)
- [Pseudo-first-order reaction](pseudo-first-order-reaction.md)

## ↑ Ancestors (6)

1. [Rate law](rate-law.md)
2. [Reaction rate](reaction-rate.md)
3. [Chemical kinetics](chemical-kinetics-split.md)
4. [Chemical reaction](chemical-reaction-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Acetone iodination rate-law experiment](acetone-iodination-rate-law-experiment.md)
- [Arrhenius equation](arrhenius-equation.md)
- [Modified Arrhenius equation](modified-arrhenius-equation.md)
- [Molecularity](molecularity.md)
- [Order of reaction](order-of-reaction.md)
- [Rate constant](rate-constant.md)
- [Second-order reaction](second-order-reaction.md)
