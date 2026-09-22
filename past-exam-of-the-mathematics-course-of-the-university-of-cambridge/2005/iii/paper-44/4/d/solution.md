<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the quoted daily death rates as piecewise constant [hazard functions](../../../../../../hazard-function.md), and use the custody schedules described in the problem. This means community service itself has the ordinary community hazard, a completer has no prison exposure, and a breacher is imprisoned from day 60 to day 120. Subsequent imprisonment after another conviction is not specified, so it is not added to the exposure schedule. The abbreviated “CS180” denotes the same initial community-service policy.

For a completer, all 360 days have the baseline rate, giving [integrated hazard](../../../../../../cumulative-hazard-function.md)

$$
H_C=\frac{360}{30000}=0.012.
$$

For a breacher, the four periods are 60 community days, 60 prison days, 30 high-risk days immediately after release, and 210 further community days. Thus

$$
H_B=\frac{60+(60)(1/2)+(30)(4)+210}{30000}
=\frac{420}{30000}=0.014.
$$

The [piecewise-exponential survival model](../../../../../../piecewise-exponential-survival-model.md) gives death [probabilities](../../../../../../probability.md) $1-e^{-H_C}$ and $1-e^{-H_B}$. Average these over the stated 60%/40% mixture of paths. Equivalently, everyone first survives the common initial 60-day community interval, and survivors then take the two paths in those proportions. The [expected value](../../../../../../expected-value.md) among 10,000 initial assignments is

$$
\boxed{\mathbb E D=10000\left[0.6(1-e^{-0.012})+0.4(1-e^{-0.014})\right]
\simeq127.18.}
$$

This accounts for removal of people after death. Since the daily hazards and endpoint death [probabilities](../../../../../../probability.md) are small, the usual [person-time](../../../../../../person-time.md) approximation replaces $1-e^{-H}$ by $H$ and gives

$$
\mathbb E D\simeq6000\frac{360}{30000}+4000\frac{420}{30000}
=72+56=\boxed{128\text{ deaths}.}
$$

Both calculations use the same specified schedules. The latter treats all planned exposure as if contributed and is slightly larger. Additional custody histories would change the exposure-weighted [integrated hazard](../../../../../../cumulative-hazard-function.md); the provided reconviction proportions alone do not determine those histories.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
