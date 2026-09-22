<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**One Grover iteration returns a marked label with certainty.** Prepare $|s\rangle=N^{-1/2}\sum_x|x\rangle$; apply the supplied [phase oracle](../../../../../phase-oracle.md) to negate amplitudes on the $N/4$ marked inputs; apply the [Grover diffusion operator](../../../../../grover-diffusion-operator.md) $D=2|s\rangle\langle s|-I$; and measure in the [computational basis](../../../../../computational-basis.md). If F prepares $|s\rangle$ from $|0\rangle$, the reflection is $D=F(2|0\rangle\langle0|-I)F^\dagger$, requiring no further oracle query.

After the oracle the amplitudes are $1/\sqrt N$ on the $3N/4$ unmarked labels and $-1/\sqrt N$ on the marked labels. Their average is

$$
\mu=\frac1N\left(\frac{3N}{4\sqrt N}-\frac{N}{4\sqrt N}\right)=\frac1{2\sqrt N}.
$$

The reflection performs [inversion about the mean](../../../../../inversion-about-the-mean.md), $a_x\mapsto2\mu-a_x$. It therefore sends every unmarked amplitude to zero and every marked amplitude to $2/\sqrt N$. The resulting normalized state is

$$
\boxed{\frac2{\sqrt N}\sum_{f(x)=1}|x\rangle.}
$$

Each marked label has [Born rule](../../../../../born-rule.md) [probability](../../../../../probability.md) $4/N$, every unmarked label has [probability](../../../../../probability.md) zero, and the marked [probabilities](../../../../../probability.md) sum to $(N/4)(4/N)=1$. This is [one-step exact Grover search with a quarter of the inputs marked](../../../../../one-step-exact-grover-search-with-a-quarter-of-the-inputs-marked.md), using one reduced-oracle query. The positive integer N must be divisible by four; a [qubit](../../../../../qubit.md) implementation may take $N=2^m$, but the stated reflection proof does not assume that register convention.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
