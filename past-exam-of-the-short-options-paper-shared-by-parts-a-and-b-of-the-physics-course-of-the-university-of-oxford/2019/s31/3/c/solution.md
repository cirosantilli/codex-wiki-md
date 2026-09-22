<h1 id="s31/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The characteristic [polynomial](../../../../../polynomial-split.md) is $\lambda^2+2\gamma\lambda+k^2=0$. Since $0<\gamma<|k|$,

$$
\lambda_\pm=-\gamma\pm i\sqrt{k^2-\gamma^2}.
$$

Forward [Euler method](../../../../../euler-method.md) has amplification eigenvalues $g_\pm=1+h\lambda_\pm$. Their squared modulus is

$$
|g_\pm|^2=(1-\gamma h)^2+(k^2-\gamma^2)h^2=1-2\gamma h+k^2h^2.
$$

Thus

$$
\boxed{0\le h\le\frac{2\gamma}{k^2}.}
$$

Strict inequality gives numerical damping; at the upper boundary the amplitude is constant despite physical decay, so that boundary is a poor accuracy choice. In the undamped limit $\gamma=0$, $|g|^2=1+k^2h^2>1$ for every $h>0$: forward [Euler method](../../../../../euler-method.md) is unstable for any nonzero step on an undamped [harmonic oscillator](../../../../../simple-harmonic-motion.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
