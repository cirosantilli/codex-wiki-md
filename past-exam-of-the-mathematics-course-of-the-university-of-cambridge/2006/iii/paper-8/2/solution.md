<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [linear operator](../../../../../linear-operator.md) $Z$ on a [Banach space](../../../../../banach-space-split.md) is called a [dissipative operator](../../../../../dissipative-operator.md) when

$$
\|(\lambda I-Z)f\|\geq\lambda\|f\|\qquad(\lambda>0,\ f\in D(Z)).
$$

On a [Hilbert space](../../../../../hilbert-space-split.md), using the [inner product](../../../../../inner-product.md) linear in its first argument,

$$
\|(\lambda I-Z)f\|^2
=\lambda^2\|f\|^2-2\lambda\operatorname{Re}\langle Zf,f\rangle+\|Zf\|^2.
$$

If $\operatorname{Re}\langle Zf,f\rangle\leq0$, this proves the defining inequality. Conversely that inequality implies $2\lambda\operatorname{Re}\langle Zf,f\rangle\leq\|Zf\|^2$ for every $\lambda>0$; letting $\lambda\to\infty$ gives

$$
\boxed{Z\text{ is dissipative}\quad\Longleftrightarrow\quad
\operatorname{Re}\langle Zf,f\rangle\leq0\text{ for all }f\in D(Z).}
$$

For the next spectral assertion, dissipativity must be retained as a hypothesis. Let $Z$ be closed, densely defined and dissipative. For $\alpha>0$, the dissipative bound makes $\alpha I-Z$ injective. Its range is closed: if $(\alpha I-Z)f_n\to h$, the bound makes $f_n$ Cauchy, and then $Zf_n=\alpha f_n-(\alpha I-Z)f_n$ converges. Closedness produces a preimage of $h$. If the range is all of $H$, the same bound gives a bounded inverse, so $\alpha$ is in the [resolvent set](../../../../../resolvent-set-of-an-operator.md). If the closed range is proper, there is a nonzero vector in its [orthogonal complement](../../../../../orthogonal-complement.md), and the definition of the [adjoint of a densely defined operator](../../../../../adjoint-of-a-densely-defined-operator.md) gives

$$
\operatorname{Ran}(\alpha I-Z)^\perp=\ker(\alpha I-Z^*).
$$

This proves that the [positive spectrum of a dissipative operator is adjoint point spectrum](../../../../../positive-spectrum-of-a-dissipative-operator-is-adjoint-point-spectrum.md):

$$
\boxed{\alpha\in\sigma(Z)\quad\Longleftrightarrow\quad
\alpha\text{ is an eigenvalue of }Z^*\qquad(\alpha>0).}
$$

Without dissipativity the PDF's assertion is false. For example, multiplication by $x$ on $L^2(0,2)$ is bounded, closed and densely defined. The value $1$ is spectral: normalized functions supported closer and closer to $x=1$ make $\|(Z-I)f\|$ tend to zero. But $Z^*=Z$ has no [eigenvector](../../../../../eigenvector.md) for [eigenvalue](../../../../../eigenvalue.md) $1$, since a square-integrable function supported on the singleton $\{1\}$ is zero.

For the given maximal-domain operator $Q$, finite-support sequences belong to $D(Q)$, so the domain is dense. Coordinatewise limits also show it is closed: if $f^{(j)}\to f$ and $Qf^{(j)}\to h$ in $\ell^2$, each defining coordinate equation passes to the limit, giving $Qf=h\in\ell^2$ and hence $f\in D(Q)$.

Put $g_n=2^nf_n$ and $h=Qf$. For $n\geq1$,

$$
g_n-g_{n-1}=-2^{-n}h_n.
$$

Since $\sum_{n\geq1}2^{-n}|h_n|<\infty$ by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $g_n$ has a finite limit $\ell_f$. Its increments are square summable as well. Direct summation gives

$$
\begin{aligned}
\operatorname{Re}\sum_{n=0}^{N}(Qf)_n\overline{f_n}
&=-\sum_{n=0}^{N}|g_n|^2+\sum_{n=1}^{N}\operatorname{Re}(g_{n-1}\overline{g_n})\\
&=-\frac12|g_0|^2-\frac12|g_N|^2
-\frac12\sum_{n=1}^{N}|g_n-g_{n-1}|^2.
\end{aligned}
$$

The original inner-product series converges because $Qf,f\in\ell^2$. Taking $N\to\infty$ therefore gives

$$
\boxed{\operatorname{Re}\langle Qf,f\rangle
=-\frac12\left(|g_0|^2+|\ell_f|^2+\sum_{n=1}^{\infty}|g_n-g_{n-1}|^2\right)\leq0.}
$$

Thus $Q$ is dissipative, including its full maximal domain; the limiting boundary term has not been discarded.

To decide generation, solve $(\alpha I-Q)f=h$ for arbitrary $h\in\ell^2$ and fixed $\alpha>0$. The first coordinate gives $g_0=f_0=h_0/(\alpha+1)$, and the rest give

$$
g_n=\frac{g_{n-1}+2^{-n}h_n}{1+\alpha4^{-n}}\qquad(n\geq1).
$$

Because all denominators are at least one,

$$
|g_n|\leq|g_0|+\sum_{k=1}^{n}2^{-k}|h_k|
\leq|g_0|+\frac1{\sqrt3}\left(\sum_{k\geq1}|h_k|^2\right)^{1/2}.
$$

Hence $g_n$ is bounded, so $f_n=2^{-n}g_n$ belongs to $\ell^2$. The coordinate equations give $Qf=\alpha f-h\in\ell^2$, proving $f\in D(Q)$ and surjectivity of $\alpha I-Q$. Together with density, closedness and dissipativity, the [Lumer-Phillips theorem](../../../../../lumer-phillips-theorem.md) proves the [contraction generator from an exponentially weighted difference operator](../../../../../contraction-generator-from-an-exponentially-weighted-difference-operator.md) conclusion:

$$
\boxed{Q\text{ generates a strongly continuous contraction semigroup on }\ell^2.}
$$

The domain is crucial. The formal transposed matrix suggests a positive-eigenvalue solution

$$
u_n=2^{-n}u_0\prod_{k=0}^{n-1}(1+\alpha4^{-k}),
$$

which is square summable because the products converge. It is not a true adjoint [eigenvector](../../../../../eigenvector.md): the admissible test vector $f_n=2^{-n}$ has $Qf=(-1,0,0,\ldots)$, so $\langle Qf,u\rangle=-\overline{u_0}$, while $\alpha\langle f,u\rangle=\alpha\overline{u_0}\sum_n4^{-n}\prod_{k<n}(1+\alpha4^{-k})$. These cannot agree for $\alpha>0$ unless $u_0=0$. This exemplifies how [boundary terms exclude formal adjoint eigenvectors](../../../../../boundary-terms-exclude-formal-adjoint-eigenvectors.md), and explains why a calculation using only finite-support test vectors would give the wrong generation answer.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
