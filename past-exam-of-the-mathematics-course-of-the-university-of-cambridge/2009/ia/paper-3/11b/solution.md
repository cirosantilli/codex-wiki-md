<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

The integrand is symmetric in $i,j$, so $T$ is a [symmetric tensor](../../../../../symmetric-tensor.md). The sphere and its area element are invariant under rotations, and the integrand transforms covariantly when $\mathbf x,\mathbf y$ are rotated together. For fixed $\mathbf y$, rotations about its direction therefore leave $T$ unchanged. In axes with $\mathbf y$ along the third axis, the mixed transverse-axial entries vanish and the two transverse eigenvalues are equal. Thus it is an [axisymmetric symmetric rank-two tensor](../../../../../axisymmetric-symmetric-rank-two-tensor.md),

$$
T_{ij}=\alpha\delta_{ij}+\beta y_i y_j,
$$

where $\alpha,\beta$ depend on $a,n$ but not on the direction of $\mathbf y$. The restriction $n>-1$ makes the integral convergent near $\mathbf x=\mathbf y$: the integrand is of size distance$^{2n}$ and the local area element has one further radial power.

Take the polar axis along $\mathbf y$. Because $|\mathbf x|=|\mathbf y|=a$,

$$
\boxed{\mathbf y\cdot(\mathbf y-\mathbf x)=a^2(1-\cos\theta),\qquad
|\mathbf y-\mathbf x|^2=2a^2(1-\cos\theta).}
$$

The area element is $a^2\sin\theta\,d\theta\,d\phi$. Hence with $s=1-\cos\theta$,

$$
\begin{aligned}
y_iT_{ij}y_j
&=2\pi a^6(2a^2)^{n-1}\int_0^\pi(1-\cos\theta)^{n+1}\sin\theta\,d\theta\\
&=2\pi a^6(2a^2)^{n-1}\frac{2^{n+2}}{n+2}
=\boxed{\frac{\pi a^2(2a)^{2n+2}}{n+2}}.
\end{aligned}
$$

For the second scalar integral, take the [trace](../../../../../matrix-trace.md). It contracts the two chord-vector factors into their squared length:

$$
\begin{aligned}
T_{ii}
&=\int_S|\mathbf y-\mathbf x|^{2n}\,dS\\
&=2\pi a^2(2a^2)^n\int_0^2s^n\,ds
=\frac{\pi(2a)^{2n+2}}{n+1}.
\end{aligned}
$$

Put $K=\pi(2a)^{2n+2}$. The tensor form gives $3\alpha+\beta a^2=K/(n+1)$, while its axial contraction gives $\alpha+\beta a^2=K/(n+2)$. Solving yields the [weighted chord tensor of a sphere](../../../../../weighted-chord-tensor-of-a-sphere.md) coefficients

$$
\boxed{\alpha=\frac{K}{2(n+1)(n+2)},\qquad
\beta=\frac{K(2n+1)}{2a^2(n+1)(n+2)}.}
$$

Because $a>0$, this is an [isotropic tensor](../../../../../isotropic-tensor.md) exactly when $\beta=0$. Therefore **$n=-1/2$** is the unique permitted isotropic exponent.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
