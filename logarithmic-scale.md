# Logarithmic scale

↑ **Parent:** [Logarithm](logarithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_scale)

A [logarithmic scale](logarithmic-scale.md) places a positive quantity $x$ according to a [logarithm](logarithm.md), so equal [ratios](ratio.md) occupy equal distances. For example, $1,2,4,8$ are equally spaced under the [natural logarithm](natural-logarithm.md) because every successive difference is $\ln2$. An ordinary [linear scale](linear-scale.md) instead gives equal distances to equal differences: $1,2,3,4$.

For a base $b>1$ and a positive reference $x_0$, define the axis position

$$
u=\log_b(x/x_0),\qquad x>0.
$$

The reference has the same units as $x$, making $x/x_0$ a [dimensionless quantity](dimensionless-quantity.md). The distance between two positions is

$$
u_2-u_1=\log_b(x_2/x_1).
$$

Multiplying both values by the same positive factor preserves that distance. Replacing $x_0$ by $cx_0$ translates every position by $-\log_b c$; changing the base rescales positions through $\log_b z=\ln z/\ln b$. Neither change alters which [ratios](ratio.md) receive equal gaps.

In base ten, the values $1,10,100,1000$ occupy positions $0,1,2,3$ when $x_0=1$. The differences between neighboring values grow from nine to ninety to nine hundred, but every step spans one [order of magnitude](order-of-magnitude.md). The values $2,20,200$ occupy positions $0.30103,1.30103,2.30103$: the same spacing shifted by $\log_{10}2$. This lets one plot small and large positive quantities together while keeping equal proportional changes equally visible.

A [logarithmic scale](logarithmic-scale.md) is a rule for position, not an instruction to relabel the tick marks with their [logarithms](logarithm.md). A mark labelled $100$ still means the original value one hundred. Ordinary real [logarithms](logarithm.md) exclude zero and negative inputs. Omitting such values or clipping them to a plotting boundary does not give them genuine logarithmic positions; the plotting choice needs to be clear.[Matplotlib 3.10.7 documentation; Matplotlib 3.10.7, Log scale: Logarithms with other bases and Dealing with negative values](matplotlib-3-10-7-documentation/log-scale.md)

**Table of contents**

- [Order of magnitude](order-of-magnitude.md)
- [Logarithmic midpoint](logarithmic-midpoint.md)
- [Semi-log plot](semi-log-plot.md)
- [Log-log plot](log-log-plot.md)

## ↑ Ancestors (8)

1. [Logarithm](logarithm.md)
2. [Exponential function](exponential-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (26)

- [Airy disk](airy-disk.md)
- [Antibody equilibrium occupancy](antibody-equilibrium-occupancy.md)
- [Astronomical magnitude](astronomical-magnitude.md)
- [Benford law](benford-law.md)
- [Buffer capacity and concentration](buffer-capacity-and-concentration.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
- [Diode characteristic measurement](diode-characteristic-measurement.md)
- [Distance modulus](distance-modulus.md)
- [Harmonic series](harmonic-series.md)
- [Henderson-Hasselbalch equation](henderson-hasselbalch-equation.md)
- [Laplace distribution](laplace-distribution.md)
- [Linear scale](linear-scale.md)
- [Log-log plot](log-log-plot.md)
- [Logarithmic midpoint](logarithmic-midpoint.md)
- [Logarithmic scale](logarithmic-scale.md)
- [Natural logarithm](natural-logarithm.md)
- [Numerical integration](numerical-integration-split.md)
- [PCR efficiency](pcr-efficiency.md)
- [Power law](power-law.md)
- [Return level plot](return-level-plot.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Semi-log plot](semi-log-plot.md)
- [Shared-uniform counterexample to the second Borel-Cantelli lemma](shared-uniform-counterexample-to-the-second-borel-cantelli-lemma.md)
- [Student's t-distribution](student-s-t-distribution.md)
- [Uniform convergence](uniform-convergence.md)
- [Units of Q of square root two](units-of-q-of-square-root-two.md)
