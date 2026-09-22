<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose an integer $k$ large enough that

$$
\theta'=\frac{\pi}{4k+2}\leq\arcsin p,
\qquad
c=\frac{\sin\theta'}p\leq1.
$$

Prepare an ancillary qubit in $\sqrt{1-c^2}|0\rangle+c|1\rangle$ and declare only $|\xi\rangle|1\rangle$ to be good. The initial good amplitude of

$$
U|b\rangle\otimes
\left(\sqrt{1-c^2}|0\rangle+c|1\rangle\right)
$$

is $pc=\sin\theta'$. Applying $k$ [amplitude amplification](../../../../../../amplitude-amplification.md) iterations gives good amplitude

$$
\sin((2k+1)\theta')=\sin(\pi/2)=1.
$$

The final state is therefore $|\xi\rangle|1\rangle$ up to a global phase. Discarding the ancilla prepares $|\xi\rangle$ exactly; this is [exact amplitude amplification](../../../../../../exact-amplitude-amplification.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
