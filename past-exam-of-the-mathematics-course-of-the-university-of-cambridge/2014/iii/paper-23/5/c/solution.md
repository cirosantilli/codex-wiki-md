<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the product printed in the original PDF, with factors $(1-q^n)^2$ and $(1-q^{11n})^2$. The [Fricke involution](../../../../../../fricke-involution.md) normalizes $\Gamma_0(11)$ and preserves its [modular cusp](../../../../../../cusp-of-a-modular-group.md) space. Therefore $g=-11^{-1}\tau^{-2}f(-1/(11\tau))$ lies in the given one-dimensional space, so $g=cf$ for a constant $c$.

At the Fricke fixed point $\tau_*=i/\sqrt{11}$, the prefactor $-11^{-1}\tau_*^{-2}$ is one. Thus $g(\tau_*)=f(\tau_*)$. The product has $0<q_*<1$, every factor is positive, and its limit is nonzero since $\sum_nq_*^n+\sum_nq_*^{11n}<\infty$. Hence $f(\tau_*)>0$, forcing $c=1$. This [Fricke sign from a nonvanishing fixed-point value](../../../../../../fricke-sign-from-a-nonvanishing-fixed-point-value.md) proves

$$
\boxed{-\frac1{11}\tau^{-2}f\left(-\frac1{11\tau}\right)=f(\tau).}
$$

Part (b) now gives $\Lambda(f,s)=\Lambda(f,2-s)$. Its Taylor series at one contains only even powers, so its order of vanishing is even. The function is not identically zero, since its first [Fourier coefficient](../../../../../../fourier-coefficient.md) is one. In this example the product is positive on the entire positive imaginary axis, and its Mellin integral at $s=1$ is positive. Thus the stronger conclusion is

$$
\boxed{\operatorname{ord}_{s=1}\Lambda(f,s)=0,\quad\text{in particular it is even}.}
$$

The TeX aid duplicates and corrupts the product in this part; neither corrupted expression is used.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
