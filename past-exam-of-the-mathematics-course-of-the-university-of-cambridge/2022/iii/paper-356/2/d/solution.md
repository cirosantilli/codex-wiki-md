<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the low-temperature regime, the particle rapidly equilibrates near a minimum and only rarely crosses a neighboring maximum. Applying [Laplace's method](../../../../../../laplace-s-method.md) to the exact current formula gives the [Kramers escape rates](../../../../../../kramers-escape-rate.md)

$$
k_+=\frac{\sqrt{|\phi''(m_0)\phi''(M_1)|}}{2\pi}e^{-\Delta\phi_+/D},
\qquad
k_-=\frac{\sqrt{|\phi''(m_0)\phi''(M_0)|}}{2\pi}e^{-\Delta\phi_-/D}.
$$

Each right or left escape changes position by $2\pi$, hence

$$
\boxed{v_s\simeq2\pi(k_+-k_-).}
$$

The reduced [continuous-time random walk](../../../../../../continuous-time-random-walk.md) on minima has off-diagonal transition rates

$$
\boxed{W(k|l)=k_+\delta_{k,l+1}+k_-\delta_{k,l-1},}
$$

and diagonal generator entry $W(l|l)=-(k_++k_-)$. Its residence time in each well is exponentially distributed with rate $k_++k_-$, and the next jump is right with probability $k_+/(k_++k_-)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
