<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce $T=\epsilon t$ and write $x_0=A(T)\cos[t+\theta(T)]$. Averaging

$$
\frac d{dt}\frac{x^2+\dot x^2}{2}=-\epsilon\dot x^4
$$

over one fast period gives $AA_T=-3A^4/8$ and $\theta_T=0$. The initial data therefore give the [method of multiple scales](../../../../../../method-of-multiple-scales.md) result

$$
\boxed{x(t)\sim\frac{\cos t}{\sqrt{1+3\epsilon t/4}}}
$$

through $t=O(\epsilon^{-1})$.

For the replacement damping, $\sin(\dot x)\dot x=\dot x^2-\dot x^4/6+\cdots$ is even in $\dot x$. Every term has zero resonant projection onto the fundamental over a complete orbit, so the $O(\epsilon)$ slow amplitude and phase equations vanish. Thus

$$
\boxed{x(t)=\cos t+O(\epsilon)}
$$

through $t=O(\epsilon^{-1})$: there is no first-order secular damping, although bounded mean and higher-harmonic corrections occur.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
