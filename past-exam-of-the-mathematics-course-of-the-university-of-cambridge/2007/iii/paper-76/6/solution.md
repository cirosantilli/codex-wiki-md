<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write $c=\cos2\phi$, $s=\sin2\phi$ and $\sigma=(\sigma_{11}+\sigma_{22})/2$. On the fixed [yield surface](../../../../../yield-surface.md), $\xi_{,l}=-c$ and $\tau_{,l}=-s$, where $l$ is stress-space [arc length](../../../../../arc-length.md). Substituting $\sigma_{11}=\sigma+\xi$, $\sigma_{22}=\sigma-\xi$, $\sigma_{12}=\tau$ into planar [force balance](../../../../../force-balance.md) gives

$$
\boxed{\sigma_{,1}=c\,l_{,1}+s\,l_{,2},\qquad\sigma_{,2}=s\,l_{,1}-c\,l_{,2}.}
$$

Thus $\nabla\sigma=M\nabla l$, with $M=\begin{pmatrix}c&s\\s&-c\end{pmatrix}$.

For a spatial curve $x(s_0)$ and a function $\mathcal F(\sigma,l)$, the [chain rule](../../../../../chain-rule.md) gives

$$
\frac{d\mathcal F}{ds_0}=
(\mathcal F_{,\sigma}\ \mathcal F_{,l})
\begin{pmatrix}
x_1'c+x_2's&x_1's-x_2'c\\
x_1'&x_2'
\end{pmatrix}
\begin{pmatrix}l_{,1}\\l_{,2}\end{pmatrix}.
$$

Here primes refer to the spatial parameter $s_0$, not the yield-curve parameter $l$. The displayed row-matrix product being zero is therefore sufficient for $\mathcal F$ to remain constant.

The [eigenvectors](../../../../../eigenvector.md) of $M$ are $e_\alpha=(\cos\phi,\sin\phi)$ and $e_\beta=(-\sin\phi,\cos\phi)$, with [eigenvalues](../../../../../eigenvalue.md) $+1$ and $-1$. Along these [slip lines](../../../../../slip-line.md), respectively, $d\sigma=dl$ and $d\sigma=-dl$. This proves the [stress characteristics for an anisotropic yield curve](../../../../../stress-characteristics-for-an-anisotropic-yield-curve.md):

$$
\boxed{\sigma-l=\text{constant on }\alpha,\quad\frac{dx_2}{dx_1}=\tan\phi;\qquad\sigma+l=\text{constant on }\beta,\quad\frac{dx_2}{dx_1}=-\cot\phi.}
$$

For the velocity relations, the outward normal to the reduced yield curve is proportional to $(-\sin2\phi,\cos2\phi)$. The [associated flow rule](../../../../../associated-flow-rule.md), using the symmetric stress work pairing $D:\delta\sigma$, therefore gives a [rate-of-strain tensor](../../../../../strain-rate-tensor.md) proportional to

$$
D\propto\begin{pmatrix}-\sin2\phi&\cos2\phi\\\cos2\phi&\sin2\phi\end{pmatrix}.
$$

The off-diagonal stress variation contributes $2D_{12}\delta\sigma_{12}$, which ensures this normality calculation uses the correct factor. Direct multiplication gives $e_\alpha^TDe_\alpha=e_\beta^TDe_\beta=0$: neither [slip line](../../../../../slip-line.md) direction extends instantaneously.

Resolve the velocity as $w=u e_\alpha+v e_\beta$. Since $de_\alpha=e_\beta\,d\phi$ and $de_\beta=-e_\alpha\,d\phi$, its longitudinal derivative along an $\alpha$ curve is $du-v\,d\phi$, and along a $\beta$ curve it is $dv+u\,d\phi$. Setting these extensions to zero gives the [Geiringer velocity relations](../../../../../geiringer-velocity-relations.md):

$$
\boxed{du-v\,d\phi=0\quad\text{along }\alpha,\qquad dv+u\,d\phi=0\quad\text{along }\beta.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
