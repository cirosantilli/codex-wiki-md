<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

During the positive half-period, write $Y=(A,B)^T$ and $\dot Y=K_+Y$, with $K_+=\begin{pmatrix}0&D^2\\ i&0\end{pmatrix}$. Then $K_+^2=iD^2I=\sigma^2I$. Its two [eigenvalues](../../../../../eigenvalue.md) are $\pm\sigma$, and corresponding [eigenvectors](../../../../../eigenvector.md) are $(\sigma,i)^T$ and $(-\sigma,i)^T$. Since $D>0$, they are independent. Thus **the general half-period solution** is

$$
\boxed{Y(t)=P_+\begin{pmatrix}\sigma\\i\end{pmatrix}e^{\sigma t}+Q_+\begin{pmatrix}-\sigma\\i\end{pmatrix}e^{-\sigma t}.}
$$

Using the even and odd terms in the [matrix exponential](../../../../../matrix-exponential.md), $e^{TK_+}=I\cosh(\sigma T)+(K_+/\sigma)\sinh(\sigma T)$. Because $D^2/\sigma=-i\sigma$, the [fundamental matrix of a linear differential equation](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) gives

$$
\boxed{M^+=\begin{pmatrix}\cosh\sigma T&-i\sigma\sinh\sigma T\\(i/\sigma)\sinh\sigma T&\cosh\sigma T\end{pmatrix},\qquad Y(T)=M^+Y(0).}
$$

The lower-left denominator is $\sigma$, as printed in the PDF. In the negative half-period $K_-=\begin{pmatrix}0&-D^2\\i&0\end{pmatrix}$ and $K_-^2=(\sigma^*)^2I$. The analogous [matrix exponential](../../../../../matrix-exponential.md) has the stated $M^-$, replacing $\sigma$ by its [complex conjugate](../../../../../complex-conjugate.md) $\sigma^*=-i\sigma$. Both matrices satisfy

$$
\boxed{\det M^+=\det M^-=\cosh^2(\sigma T)-\sinh^2(\sigma T)=1,}
$$

with $\sigma^*$ in the second determinant. Equivalently, their generators have zero [trace](../../../../../matrix-trace.md), so the determinant of each [matrix exponential](../../../../../matrix-exponential.md) is one.

At each complete period the state is multiplied by the [monodromy matrix of a periodic linear system](../../../../../monodromy-matrix-of-a-periodic-linear-system.md) $N=M^-M^+$, so $Y(2nT)=N^nY(0)$. The determinant is therefore $\det N=1$. Let $c_\pm=\cosh(\sigma^{(*)}T)$ and $s_\pm=\sinh(\sigma^{(*)}T)$. Multiplying the two matrices and taking the [trace](../../../../../matrix-trace.md) gives

$$
\operatorname{tr}N=2c_-c_++\left(\frac{\sigma^*}{\sigma}+\frac\sigma{\sigma^*}\right)s_-s_+=2|\cosh(\sigma T)|^2.
$$

The ratio sum vanishes because the two ratios are $-i$ and $i$. With $x=\sqrt2DT$, the [hyperbolic-function identity](../../../../../hyperbolic-function-identity.md) for $|\cosh(a+ia)|^2$ consequently yields

$$
\boxed{\det N=1,\qquad F\equiv\operatorname{tr}N=\cosh x+\cos x.}
$$

For $x>0$, $F>2$: differentiating gives $F'=\sinh x-\sin x>0$, since this derivative has derivative $\cosh x-\cos x>0$ and vanishes initially. The [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2-F\lambda+1$. Hence the two [Floquet multipliers](../../../../../floquet-multiplier.md) are positive, distinct and reciprocal, with **dominant multiplier and growth rate**

$$
\boxed{\Lambda=\frac{F+\sqrt{F^2-4}}2>1,\qquad
\gamma=\frac{\log\Lambda}{2T}=\frac1{2T}\operatorname{arcosh}\left(\frac{\cosh(\sqrt2DT)+\cos(\sqrt2DT)}2\right).}
$$

The finite-time propagation within each half-period is bounded independently of the number of cycles, so it does not change this asymptotic [Floquet growth rate](../../../../../floquet-growth-rate.md). The expression is the maximal rate, attained for generic nonzero initial data. The exceptional initial state in the reciprocal multiplier's [eigenspace](../../../../../eigenspace.md) decays with rate $-\gamma$; the zero state stays zero. Thus a vanishing mean [alpha effect](../../../../../alpha-effect.md) does not preclude [dynamo action](../../../../../dynamo-action.md) in this periodically switched [Parker dynamo wave](../../../../../parker-dynamo-wave.md) model.

As $x\to\infty$, $F=\tfrac12e^x[1+O(e^{-x})]$, $\Lambda=F[1+O(F^{-2})]$, and $\log\Lambda=x-\log2+o(1)$. Therefore

$$
\boxed{\gamma=\frac{\sqrt2DT-\log2}{2T}+o(1).}
$$

In particular, **at $T=1$ the rate is asymptotic to $(\sqrt2D-\log2)/2$**, as required. The growth calculation uses the product $M^-M^+$, rather than averaging the two generators: the two generators do not commute.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 318](../../paper-318-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
