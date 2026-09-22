<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expanding the exponential for $|ka|\ll1$ gives $e^{-2ka}=1-2ka+2k^2a^2+O((ka)^3)$. Substitution of the [plane wave](../../../../../../plane-wave.md) $A=e^{i(kx-\omega t)}$ in the model gives

$$
-i\omega=-iak+ia^2k^2,\qquad \boxed{\omega=ak-a^2k^2},
$$

which is exactly the quadratic approximation to the [dispersion relation](../../../../../../dispersion-relation.md).

For the slowly varying width, put $X=\epsilon x$ and use the [WKB approximation](../../../../../../wkb-approximation.md)

$$
A=B(X)\exp\left(\frac{i}{\epsilon}S(X)-i\Omega t\right),\qquad k(X)=S_X.
$$

The derivatives are

$$
A_x=(ikB+\epsilon B_X)e^{iS/\epsilon-i\Omega t},\quad
A_{xx}=[-k^2B+i\epsilon(k_XB+2kB_X)+\epsilon^2B_{XX}]e^{iS/\epsilon-i\Omega t}.
$$

At leading order $\Omega=ak-a^2k^2$. On the downstream small-wavenumber branch write

$$
k=\frac q{a(X)},\qquad q=\frac{1-\sqrt{1-4\Omega}}2,
$$

so $q$ is independent of $X$. The next order gives the [slowly varying triangular-jet envelope](../../../../../../slowly-varying-triangular-jet-envelope.md) transport equation

$$
(a-2a^2k)B_X=a^2k_XB,\qquad
\frac{B_X}{B}=-\frac{q}{1-2q}\frac{a_X}{a}.
$$

Integration therefore yields

$$
\boxed{B(X)=B(0)\left[\frac{a(X)}{a(0)}\right]^{-q/(1-2q)}},\qquad
\boxed{B(X)\simeq B(0)\left[\frac{a(X)}{a(0)}\right]^{-\Omega}}\quad(\Omega\ll1).
$$

Indeed, $q/(1-2q)=\Omega+O(\Omega^2)$. The requested power is the leading low-frequency envelope, not the exact finite-frequency exponent of the quadratic model. The corresponding leading field is this [wave envelope](../../../../../../envelope-waves.md) times $\exp(i\int_0^x q/a(\epsilon s)\,ds-i\Omega t)$. Positive slowly varying width and separation from the zero of the local [group velocity](../../../../../../group-velocity.md), $1-2q=0$, are needed for this [WKB approximation](../../../../../../wkb-approximation.md). Extremely large $|\log[a(X)/a(0)]|$ can also invalidate replacing the exact exponent by $\Omega$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
