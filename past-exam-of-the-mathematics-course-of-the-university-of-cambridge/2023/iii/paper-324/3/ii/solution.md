<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If some integer $k$ obeys $(2k+1)\theta=\pi/2$, ordinary [amplitude amplification](../../../../../../amplitude-amplification.md) already gives $|g\rangle$ exactly. For a general known $\theta$, use [exact amplitude amplification](../../../../../../exact-amplitude-amplification.md). Choose $k$ so that

$$
\theta'=\frac{\pi}{4k+2}\leq\theta
$$

and put $c=\sin\theta'/\sin\theta\leq1$. Append an ancilla and coherently arrange that its designated good value has amplitude $c$ conditional on the original register being good. With the enlarged good subspace defined by

$$
f(x)=1\quad\text{and}\quad\text{ancilla}=0,
$$

the starting state's total good amplitude is $c\sin\theta=\sin\theta'$.

Apply the [amplitude amplification theorem](../../../../../../amplitude-amplification.md) $k$ times to this enlarged problem. Its final good amplitude is

$$
\sin((2k+1)\theta')=\sin\frac\pi2=1.
$$

The [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) implements the reflection $I_G$ by phase kickback, and the known state-preparation circuit implements the reflection about the starting state by prepare--reflect--unprepare. A final computational-basis measurement therefore yields an $x$ with $f(x)=1$ with certainty.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
