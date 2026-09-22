<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For one small transverse displacement, the [elastic energy](../../../../../elastic-energy.md) of the [elastic filament](../../../../../elastic-filament.md) is

$$
U[h]=\frac A2\int_0^L[h''(x)]^2\,dx,
$$

where $A$ is the [filament bending modulus](../../../../../filament-bending-modulus.md). Its [first variation](../../../../../first-variation.md) is

$$
\delta U=A[h''\delta h'-h'''\delta h]_0^L+A\int_0^Lh''''\delta h\,dx.
$$

The [clamped boundary conditions](../../../../../clamped-boundary-condition.md) remove the left boundary terms. A force-free and torque-free tip permits independent $\delta h(L)$ and $\delta h'(L)$, so the [natural boundary conditions for a free endpoint](../../../../../natural-boundary-conditions-for-a-free-endpoint.md) are **$h''(L)=h'''(L)=0$**: zero bending moment and transverse shear.

There is an important distinction between an energy minimum and a [normal mode](../../../../../normal-mode.md). The unloaded [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md) is $h''''=0$, whose only solution with these four boundary conditions is $h=0$. A general fluctuating shape is a sum of modes, not one of the stated sinusoidal/hyperbolic functions. To obtain the [clamped--free bending modes](../../../../../clamped-free-bending-mode.md), extremize the bending Rayleigh quotient, or equivalently $U[W]-\tfrac12Ak^4\int W^2dx$ with a fixed norm. Its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{W''''=k^4W.}
$$

This is the [constrained variational characterization of bending modes](../../../../../constrained-variational-characterization-of-bending-modes.md). Its four characteristic roots are $\pm k,\pm ik$. Clamping gives $F=-D$ and $E=-B$, hence

$$
W=D(\cos kx-\cosh kx)+B(\sin kx-\sinh kx).
$$

The free-tip conditions reduce to

$$
\begin{pmatrix}\cos q+\cosh q&\sin q+\sinh q\\ \sin q-\sinh q&-(\cos q+\cosh q)\end{pmatrix}\binom DB=0,\qquad q=kL.
$$

Its [determinant](../../../../../determinant.md) is $-2(1+\cos q\cosh q)$, so nontrivial modes require

$$
\boxed{\cos q_n\cosh q_n=-1,\qquad k_n=q_n/L.}
$$

No zero mode exists, since a cubic satisfying the homogeneous clamp/free conditions is zero. The [clamped-free bending spectrum](../../../../../clamped-free-bending-mode.md) starts with $q_1\in(\pi/2,2)$; bisection or Newton iteration gives **$q_1\simeq1.875104$, so $k_1\simeq1.875104/L$**. Choosing $D=N(\sin q_n+\sinh q_n)$ and $B=-N(\cos q_n+\cosh q_n)$ gives

$$
\boxed{W_n=N\big[(\sin q_n+\sinh q_n)(\cos k_nx-\cosh k_nx)-(\cos q_n+\cosh q_n)(\sin k_nx-\sinh k_nx)\big].}
$$

The second boundary condition follows from the root equation, and $N$ is arbitrary until a normalization is chosen.

The bending operator with these boundary conditions is positive and [self-adjoint](../../../../../self-adjoint-operator.md). Twice integrating by parts gives

$$
\int_0^L W_n''W_m''\,dx=k_m^4\int_0^L W_nW_m\,dx.
$$

Symmetry implies [orthogonality](../../../../../orthogonal-vectors.md) when $n\ne m$. Expand $h(x)=\sum_n a_nW_n(x)$ and use $I_n=L^{-1}\int_0^LW_n^2dx$. Then

$$
U=\frac{AL}2\sum_n k_n^4 I_na_n^2,\qquad \langle a_na_m\rangle=\delta_{nm}\frac{k_BT}{ALk_n^4I_n},
$$

by the [equipartition theorem](../../../../../equipartition-theorem.md). The supplied endpoint identity therefore yields the [thermal bending fluctuations of a clamped filament](../../../../../thermal-bending-fluctuations-of-a-clamped-filament.md):

$$
\langle h(L)^2\rangle=\frac{4k_BT}{AL}\sum_{n=1}^\infty k_n^{-4}=\frac{4k_BTL^3}{A}\sum_{n=1}^\infty q_n^{-4}.
$$

To evaluate the sum, apply a tip force $f$ and minimize $U-fh(L)$. The modified free-end conditions are $h''(L)=0$ and $-Ah'''(L)=f$, and $h''''=0$ in the interior. Integration gives $h(x)=fx^2(3L-x)/(6A)$, so the [tip-force compliance of a cantilever](../../../../../tip-force-compliance-of-a-cantilever.md) is $L^3/(3A)$. On the other hand, minimizing the modal energy minus $f\sum_na_nW_n(L)$ gives $a_n=fW_n(L)/(ALk_n^4I_n)$ and hence

$$
\frac{h(L)}f=\frac4{AL}\sum_nk_n^{-4}=\frac{4L^3}{A}\sum_nq_n^{-4}.
$$

Comparison evaluates the [fourth inverse-power sum of the cantilever spectrum](../../../../../fourth-inverse-power-sum-of-the-cantilever-spectrum.md) without truncating the modes:

$$
\boxed{\sum_{n=1}^\infty q_n^{-4}=\frac1{12},\qquad \langle h(L)^2\rangle=\frac{k_BTL^3}{3A}.}
$$

The boxed [variance](../../../../../variance-split.md) is for the specified single transverse direction. An independent equilibrium check follows by differentiating the Gaussian partition function with respect to $f$: $\partial\langle h(L)\rangle/\partial f=\langle h(L)^2\rangle/(k_BT)$ at zero load, reproducing the same result from the static compliance. Keeping only the first [normal mode](../../../../../normal-mode.md) gives about $0.32356\,k_BTL^3/A$, roughly $97.1\%$ of the exact [variance](../../../../../variance-split.md). With two independent equivalent transverse directions, their summed [variance](../../../../../variance-split.md) is twice the boxed result. The small-slope model requires $k_BTL/A\ll1$, or $L$ small compared with the usual three-dimensional [persistence length](../../../../../persistence-length.md) $A/(k_BT)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
