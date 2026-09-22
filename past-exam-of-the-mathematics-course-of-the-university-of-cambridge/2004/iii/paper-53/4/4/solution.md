<h1 id="4/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For known $p$, use [nearest-integer stopping for amplitude amplification](../../../../../../nearest-integer-stopping-for-amplitude-amplification.md). Set

$$
r=\left\lfloor\frac\pi{4\theta}\right\rfloor,\qquad\theta=\arcsin\sqrt p.
$$

Writing $x=\pi/(4\theta)$, the difference between $r+1/2$ and $x$ has absolute value at most $1/2$. Thus $|(2r+1)\theta-\pi/2|\leq\theta$. The [Born rule](../../../../../../born-rule.md) and part 3 give

$$
\Pr(\mathrm{good})=\cos^2\bigl((2r+1)\theta-\pi/2\bigr)\geq\cos^2\theta=1-p.
$$

Count the initial $A$ once and the $A^\dagger$ and $A$ occurring inside each of the $r$ amplification iterates. The number of applications of either preparation unitary is therefore

$$
\boxed{N_A=2\left\lfloor\frac\pi{4\arcsin\sqrt p}\right\rfloor+1\sim\frac\pi{2\sqrt p}\quad(p\to0).}
$$

The counts separately are $r+1$ applications of $A$ and $r$ applications of $A^\dagger$, in addition to $r$ applications each of $V$ and $V_0$. This is a quadratic improvement over the $1/p$ mean number of unamplified trials. At an exact rounding tie either nearest iterate meets the probability bound. Knowledge of $p$ is used in selecting the stopping time; repeatedly applying $Q$ without a suitable stopping rule can rotate the state past the good axis and reduce success again. The fact that answers lie in NP supplies verification, but by itself gives no claim that $1/\sqrt p$ is polynomial in input length.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
