<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Use the equally likely release prior, and write $s$ for the [probability](../../../../../probability.md) that the guard names B when A is released. If B is released the guard cannot name B; if C is released the guard must name B. The [law of total probability](../../../../../law-of-total-probability.md) therefore gives

$$
P(B\text{ named})=\frac{s}{3}+\frac13=\frac{1+s}{3}.
$$

A remains jailed and B is named precisely when C is released. Its [probability](../../../../../probability.md) is $1/3$, so the [conditional probability](../../../../../conditional-probability.md) is

$$
\boxed{P(A\text{ remains}\mid B\text{ named})=\frac1{1+s}.}
$$

In **(a)** unbiased naming has $s=1/2$, giving **$2/3$**: the guard's claim is false and A's chances have not improved. In **(b)** preferentially naming B has $s=1$, giving **$1/2$**: that naming rule makes the claim correct. In **(c)** preferentially naming C has $s=0$, giving **$1$**: naming B then reveals that C is the released person, so A certainly remains.

This is the [three prisoners problem](../../../../../three-prisoners-problem.md). The observed name includes information about how the guard selects a name; it is not merely the event that B remains. With general release priors $\pi_A,\pi_B,\pi_C$, the same calculation gives $\pi_C/(s\pi_A+\pi_C)$, making explicit where the equal-prior convention enters.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
