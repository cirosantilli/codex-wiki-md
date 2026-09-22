<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A positive-eigenvalue [normal mode](../../../../../../normal-mode.md) satisfies $KW_n=Ak_n^4W_n$. Solving the constant-coefficient equation gives the [sine](../../../../../../sine.md), [cosine](../../../../../../cosine.md), [hyperbolic sine](../../../../../../hyperbolic-sine.md) and [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) family. To avoid confusing modal coefficients with the [filament bending modulus](../../../../../../filament-bending-modulus.md), write those coefficients as $c_1,c_2,c_3,c_4$.

The free conditions at zero require $c_3=c_1$ and $c_4=c_2$. With $q=kL$, the remaining conditions are

$$
\begin{pmatrix}
\cosh q-\cos q&\sinh q-\sin q\\
\sinh q+\sin q&\cosh q-\cos q
\end{pmatrix}\binom{c_1}{c_2}=0.
$$

Its determinant is $2(1-\cos q\cosh q)$. Therefore the [free-free bending spectrum](../../../../../../free-free-bending-spectrum.md) is

$$
\boxed{\cos q_n\cosh q_n=1,\qquad k_n=q_n/L\quad(n\geq1).}
$$

A convenient corresponding [eigenfunction](../../../../../../eigenfunction.md) is

$$
W_n(x)=N_n\left[\cos(k_nx)+\cosh(k_nx)
-\gamma_n(\sin(k_nx)+\sinh(k_nx))\right],\qquad
\gamma_n=\frac{\cosh q_n-\cos q_n}{\sinh q_n-\sin q_n},
$$

where $N_n$ gives unit $L^2$ norm. The [stable characteristic equation for free-free bending modes](../../../../../../stable-characteristic-equation-for-free-free-bending-modes.md) is $\cos q=\operatorname{sech}q$. Intersections or numerical bracketing give

$$
\boxed{q_1\simeq4.730040745,\quad q_2\simeq7.853204624,\quad
q_3\simeq10.995607838,\quad q_4\simeq14.137165491,\quad q_5\simeq17.278759657,\ldots.}
$$

For the entire positive sequence, let $q_n^0=(n+\tfrac12)\pi$. Expanding $\cos q_n$ near its zero and using $\operatorname{sech}q_n\sim2e^{-q_n}$ gives

$$
\boxed{q_n=(n+\tfrac12)\pi+2(-1)^{n+1}e^{-(n+1/2)\pi}
+O(e^{-2(n+1/2)\pi}).}
$$

There are also two [zero-energy filament modes](../../../../../../zero-energy-filament-mode.md), not captured by substituting $k=0$ into the finite-coefficient trigonometric expression. Solving $W^{(4)}=0$ with free endpoints gives the affine kernel. An [orthonormal basis](../../../../../../orthonormal-basis.md) of that kernel is

$$
W_{\rm tr}(x)=L^{-1/2},\qquad
W_{\rm tilt}(x)=\sqrt{12/L^3}(x-L/2).
$$

The positive [normal modes](../../../../../../normal-mode.md) are [orthogonal](../../../../../../orthogonal-vectors.md) to both. Including these two rigid-motion modes is essential for completeness; the regular [self-adjoint operator](../../../../../../self-adjoint-operator.md) on a finite interval has a complete discrete eigenbasis.

<a id="2/b/image-characteristic-roots-and-bending-shapes-of-a-filament-with-two-free-ends"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-74-free-filament-modes.png)

**[Figure 1](#2/b/image-characteristic-roots-and-bending-shapes-of-a-filament-with-two-free-ends). Characteristic roots and bending shapes of a filament with two free ends**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
