<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For two candidates $A,C$, their difference is a continuous [adapted](../../../../../../adapted-process.md) [finite-variation process](../../../../../../finite-variation-process.md). It is also a [local martingale](../../../../../../local-martingale.md), since

$$
A-C=(Y^2-C)-(Y^2-A).
$$

Apply part (b) after subtracting its initial value. Consequently

$$
\boxed{A_t-C_t=A_0-C_0\quad\text{for all }t\text{ almost surely}.}
$$

This proves the [uniqueness of an increasing square compensator](../../../../../../uniqueness-of-an-increasing-square-compensator.md) when the initial value is prescribed, in particular under the standard [quadratic variation](../../../../../../quadratic-variation.md) normalization $A_0=C_0=0$.

The printed assertion omits that normalization and is literally false. For standard [Brownian motion](../../../../../../brownian-motion-split.md) $Y$, both $A_t=t$ and $C_t=t+1$ are continuous [adapted](../../../../../../adapted-process.md) increasing processes; both $Y_t^2-t$ and $Y_t^2-t-1$ are [martingales](../../../../../../martingale-split.md). Thus **uniqueness holds after fixing the initial value; otherwise it holds only up to an initial constant**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
