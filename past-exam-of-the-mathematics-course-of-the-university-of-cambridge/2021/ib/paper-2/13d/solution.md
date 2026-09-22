<h1 id="13d/solution">Solution</h1>

↑ **Parent:** [13D](../13d.md)

Take a [variation](../../../../../variation.md) $x+\varepsilon\xi$ with $\xi(a)=\xi(b)=0$. Expanding the [action](../../../../../action.md) gives

$$
S[x+\varepsilon\xi]
=S[x]+\varepsilon\int_a^b\bigl(\dot x\dot\xi-V'(x)\xi\bigr)\,dt
+\frac{\varepsilon^2}{2}\int_a^b\bigl(\dot\xi^2-V''(x)\xi^2\bigr)\,dt
+O(\varepsilon^3).
$$

An [integration by parts](../../../../../integration-by-parts.md) and the fixed endpoint conditions give the [first variation](../../../../../first-variation.md)

$$
\delta S=-\int_a^b\bigl(\ddot x+V'(x)\bigr)\xi\,dt.
$$

The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore yields the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\ddot x+V'(x)=0},
$$

and the [second variation](../../../../../second-variation.md) is

$$
\boxed{\delta^2S=\frac12\int_a^b\bigl(\dot\xi^2-V''(x)\xi^2\bigr)\,dt}.
$$

Linearizing the equation of motion about $x$ gives

$$
0=\ddot x+V'(x)+\varepsilon\bigl(\ddot u+V''(x)u\bigr)+O(\varepsilon^2),
$$

so the [Jacobi equation](../../../../../jacobi-equation.md) is

$$
\ddot u+V''(x)u=0.
$$

When $u$ has no zero on $[a,b]$,

$$
\dot\xi^2-V''(x)\xi^2
=\left(\dot\xi-\frac{\dot u}{u}\xi\right)^2
+\frac d{dt}\left(\frac{\dot u}{u}\xi^2\right).
$$

The total derivative integrates to zero because $\xi(a)=\xi(b)=0$, hence

$$
\boxed{\delta^2S=\frac12\int_a^b
\left(\dot\xi-\frac{\dot u}{u}\xi\right)^2dt\geq0}.
$$

For the [simple harmonic oscillator](../../../../../simple-harmonic-motion.md), the Jacobi equation is $\ddot u+\omega^2u=0$. Put $t_0=(a+b)/2$ and choose

$$
u(t)=\cos\bigl(\omega(t-t_0)\bigr).
$$

If $b-a<\pi/\omega$, then $|\omega(t-t_0)|<\pi/2$ throughout $[a,b]$, so $u$ is positive there. The preceding square identity proves that the classical path is a local minimum of the action whenever the elapsed time is less than half an [oscillation period](../../../../../period-of-an-oscillation.md).

## ↑ Ancestors (10)

1. [13D](../13d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
