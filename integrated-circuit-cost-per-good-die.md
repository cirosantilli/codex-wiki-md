# Integrated circuit cost per good die

↑ **Parent:** [Poisson defect yield](poisson-defect-yield.md)

Let a circular [semiconductor wafer](semiconductor-wafer.md) have [diameter](diameter.md) $d$ and processed cost $C_w$. For square [semiconductor dies](semiconductor-die.md) of [area](surface-area.md) $A$, ignoring all edge losses gives the ideal gross count $N_0=\pi d^2/(4A)$. For illustration adopt the geometric edge approximation

$$
N_g\approx\frac{\pi d^2}{4A}-\frac{\pi d}{\sqrt{2A}},\qquad
\mathbb E[G]\approx N_g e^{-DA},\qquad
C_{\rm good}\approx\frac{C_w}{N_g e^{-DA}}.
$$

Here $G$ is the good-die count. The correction scales as wafer perimeter divided by die side length: only a boundary strip can lose partially fitting squares. Its coefficient is an approximation depending on layout; the expression is not an exact packing theorem and is useful only when $\sqrt A\ll d$. Counts from it need not be [integers](integer-split.md). Actual layouts, edge exclusion and separation lanes determine an integer gross count. The [expected value](expected-value-split.md) of $G$ follows by [linearity of expectation](linearity-of-expectation.md); independence between [semiconductor dies](semiconductor-die.md) is not required for that step if each has the same yield.

For the original example $d=200\,\mathrm{mm}$, $A=100\,\mathrm{mm}^2$, $D=0.005\,\mathrm{mm}^{-2}$ and $C_w=1000$ cost units, $N_0=314.159$ and $N_g\approx269.730$. The predicted good count is $163.600$ per wafer, and the processed cost is $6.11248$ units per good die. This is total processed cost divided by expected output, appropriate to a large repeated batch; it is not the [expected value](expected-value-split.md) of a single-wafer random ratio $C_w/G$, which is undefined when $G=0$. Test, packaging, design and equipment costs are excluded.

A hypothetical test readout makes the inference explicit. Suppose $600$ of $1000$ tested [semiconductor dies](semiconductor-die.md), each of [area](surface-area.md) $100\,\mathrm{mm}^2$, pass a specified functional test. These are invented counts for calculation, not reported measurements. The pass fraction is $\widehat Y=0.600$; within the [Poisson defect yield](poisson-defect-yield.md) assumptions it implies

$$
\widehat D=-\frac{\ln\widehat Y}{A}=0.00510826\,\mathrm{mm}^{-2}.
$$

If pass indicators are [independent random variables](independent-random-variables.md) with common success probability $Y$, their sum has a [binomial distribution](binomial-distribution.md). The fitted standard deviation of the pass fraction is $\sqrt{0.6(1-0.6)/1000}=0.01549$. A test readout estimates pass probability for its tested functions and conditions; it cannot alone establish spatially independent defects, detect every latent failure or distinguish fabrication losses from a faulty test. The [logarithm](logarithm.md) only translates the observed fraction into a defect intensity after those additional assumptions are adopted.

## ↑ Ancestors (7)

1. [Poisson defect yield](poisson-defect-yield.md)
2. [Integrated circuit](integrated-circuit.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
