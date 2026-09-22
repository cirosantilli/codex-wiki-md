<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The discrete [Bochner–Herglotz theorem](../../../../../bochner-herglotz-theorem.md) says that a sequence $r:\mathbb Z\to\mathbb C$ is a [positive-definite function](../../../../../positive-definite-function.md), meaning

$$
\sum_{j,k=0}^{N-1}c_j\overline{c_k}\,r(j-k)\geq0\quad\hbox{for every }N\text{ and every }c_0,\ldots,c_{N-1},
$$

if and only if there is a unique finite positive [Borel measure](../../../../../borel-measure.md) $\sigma$ on $\mathbb T=\mathbb R/\mathbb Z$ such that

$$
\boxed{r(n)=\int_{\mathbb T}e^{2\pi int}\,d\sigma(t)\quad(n\in\mathbb Z).}
$$

The mass is $\sigma(\mathbb T)=r(0)$. The necessity of positive definiteness follows by integrating $|\sum_j c_je^{2\pi ijt}|^2$.

For sufficiency, positive definiteness makes the relevant [Gram matrices](../../../../../gram-matrix.md) Hermitian positive semidefinite, so $r(-n)=\overline{r(n)}$ and $|r(n)|\leq r(0)$. Define

$$
p_N(t)=\frac1N\sum_{j,k=0}^{N-1}r(j-k)e^{-2\pi i(j-k)t}
=\sum_{|n|<N}\left(1-\frac{|n|}{N}\right)r(n)e^{-2\pi int}.
$$

Taking $c_j=e^{-2\pi ijt}$ in the positive-definiteness condition gives $p_N(t)\geq0$, while $\int_{\mathbb T}p_N(t)\,dt=r(0)$. Moreover,

$$
\int_{\mathbb T}e^{2\pi imt}p_N(t)\,dt
=\begin{cases}(1-|m|/N)r(m),&|m|<N,\\0,&|m|\geq N.
\end{cases}
$$

Thus the integrals against every [trigonometric polynomial](../../../../../trigonometric-polynomial.md) converge. These polynomials are uniformly dense in continuous functions on the circle: smooth periodic approximation followed by [Fourier inversion](../../../../../fourier-inversion-theorem.md) for smooth functions gives this density. The uniform mass bound $r(0)$ then makes the integrals against every continuous $\varphi$ converge as well. Their limit is a positive linear functional $L$ with $|L(\varphi)|\leq r(0)\|\varphi\|_\infty$. The standard [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) gives a finite positive [Borel measure](../../../../../borel-measure.md) $\sigma$ with $L(\varphi)=\int\varphi\,d\sigma$. The preceding coefficient computation proves its required [Fourier coefficients](../../../../../fourier-coefficient.md). Finally, two such measures agree on all [trigonometric polynomials](../../../../../trigonometric-polynomial.md), hence on all continuous functions by uniform density, and therefore are identical. This proves the [Bochner–Herglotz theorem](../../../../../bochner-herglotz-theorem.md), including existence and uniqueness; if $r(0)=0$, the estimate $|r(n)|\leq r(0)$ gives the zero measure directly.

Now let $U$ be the [Koopman operator](../../../../../koopman-operator.md) $Uf=f\circ T$ on the complex [L2 space](../../../../../l2-space-is-a-hilbert-space.md) of the probability [measure-preserving system](../../../../../measure-preserving-system.md). We use $\langle f,g\rangle=\int f\overline g\,d\mu$, linear in the first entry. Since $U$ is an [isometry](../../../../../isometry.md), the sequence $r_f(n)=\langle U^nf,f\rangle$ for $n\geq0$, extended by $r_f(-n)=\overline{r_f(n)}$, is positive-definite: its matrix is the [Gram matrix](../../../../../gram-matrix.md) of $f,Uf,\ldots$. The [Bochner–Herglotz theorem](../../../../../bochner-herglotz-theorem.md) gives its [spectral measure of a Koopman observable](../../../../../spectral-measure-of-a-koopman-observable.md) $\sigma_f$.

We first prove exactly how an [atom of a measure](../../../../../atom-measure-theory.md) detects an [eigenfunction](../../../../../eigenfunction.md). Fix $\zeta=e^{2\pi it_0}$ and set

$$
A_N^\zeta f=\frac1N\sum_{j=0}^{N-1}\zeta^{-j}U^jf.
$$

The [mean ergodic theorem](../../../../../von-neumann-mean-ergodic-theorem.md), applied to the [isometry](../../../../../isometry.md) $V=\zeta^{-1}U$, says these averages converge in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to the [orthogonal projection](../../../../../orthogonal-projection.md) $P_\zeta f$ onto $\ker(U-\zeta I)$. Its usual Hilbert-space proof works without invertibility: the orthogonal complement of $\overline{\operatorname{ran}(I-V)}$ is $\ker(I-V^*)=\ker(I-V)$, and the averages of $(I-V)h$ telescope to $(h-V^Nh)/N\to0$. The equality of the two kernels follows from $V$ being an [isometry](../../../../../isometry.md), by expanding $\|Vh-h\|^2$ when $V^*h=h$.

Expanding the averaged norm through the [spectral measure of a Koopman observable](../../../../../spectral-measure-of-a-koopman-observable.md) gives

$$
\|A_N^\zeta f\|_2^2=\int_{\mathbb T}\left|\frac1N\sum_{j=0}^{N-1}e^{2\pi ij(t-t_0)}\right|^2\,d\sigma_f(t).
$$

The integrand is at most one and converges to $\mathbf1_{\{t_0\}}$. By the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md),

$$
\boxed{\|P_\zeta f\|_2^2=\sigma_f(\{t_0\}).}
$$

Thus a nonzero atom corresponds to a nonzero [Koopman operator](../../../../../koopman-operator.md) [eigenfunction](../../../../../eigenfunction.md), with eigenvalue $\zeta$, in the cyclic spectral data of $f$.

We also need the [Wiener Fourier coefficient lemma](../../../../../wiener-fourier-coefficient-lemma.md), which here has a short proof. For any finite positive circle measure $\sigma$ with coefficients $r(n)$,

$$
\frac1N\sum_{n=0}^{N-1}|r(n)|^2
=\iint\left(\frac1N\sum_{n=0}^{N-1}e^{2\pi in(t-s)}\right)\,d\sigma(t)\,d\sigma(s).
$$

The bracket is bounded in absolute value by one and tends to the indicator of the diagonal $t=s$. Another application of the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{\lim_{N\to\infty}\frac1N\sum_{n=0}^{N-1}|r(n)|^2=\sum_{t\in\mathbb T}\sigma(\{t\})^2.}
$$

In particular the limit is zero for an [atomless measure](../../../../../non-atomic-measure.md).

Suppose there are no nonconstant [Koopman operator](../../../../../koopman-operator.md) [eigenfunctions](../../../../../eigenfunction.md). For every $f$ in the [mean-zero L2 space](../../../../../mean-zero-l2-space.md), all its projections $P_\zeta f$ vanish: a nonzero projection would be a nonconstant [eigenfunction](../../../../../eigenfunction.md), since it has mean zero. Hence $\sigma_f$ is atomless, and the [Wiener Fourier coefficient lemma](../../../../../wiener-fourier-coefficient-lemma.md) gives

$$
\frac1N\sum_{n<N}|\langle U^nf,f\rangle|^2\longrightarrow0.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) also gives vanishing averaged absolute autocorrelations. For two mean-zero observables $f,g$, the sesquilinear polarization identity

$$
\langle U^nf,g\rangle=\frac14\sum_{j=0}^3i^j\langle U^n(f+i^jg),f+i^jg\rangle
$$

then gives vanishing averaged absolute cross-correlations. Taking $f=\mathbf1_A-\mu(A)$ and $g=\mathbf1_B-\mu(B)$ proves

$$
\frac1N\sum_{n<N}|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)|\longrightarrow0,
$$

which is [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md).

Conversely, this set formulation of [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md) extends to all pairs of mean-zero [L2 space](../../../../../l2-space-is-a-hilbert-space.md) observables by finite-simple-function approximation and the uniform estimate $|\langle U^nf,g\rangle|\leq\|f\|_2\|g\|_2$. If $Uh=\zeta h$ and $h\ne0$, the [isometry](../../../../../isometry.md) property gives $|\zeta|=1$. If $\zeta\ne1$, invariance of the integral gives $\int h=0$. If $\zeta=1$ and $h$ is nonconstant, replace it by $h-\int h$, a nonzero mean-zero [eigenfunction](../../../../../eigenfunction.md). But in either case

$$
|\langle U^nh,h\rangle|=\|h\|_2^2>0
$$

for every $n$, contradicting [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md). We have proved **weak mixing is equivalent to absence of nonconstant [eigenfunctions](../../../../../eigenfunction.md)**, including for noninvertible transformations.

Finally, the [doubling map](../../../../../dyadic-transformation.md) $Tx=2x\pmod1$ preserves normalized [Lebesgue measure](../../../../../lebesgue-measure.md), as substitution on its two inverse branches shows. Let $f\in L^2(\mathbb T)$ be an [eigenfunction](../../../../../eigenfunction.md), $f(2x)=\zeta f(x)$, with [Fourier coefficients](../../../../../fourier-coefficient.md) $c_k$. The [Fourier basis](../../../../../fourier-basis.md) calculation gives

$$
\widehat{Uf}(k)=\begin{cases}c_{k/2},&k\text{ even},\\0,&k\text{ odd}.
\end{cases}
$$

Since $\zeta\ne0$, all odd coefficients vanish. Every nonzero integer is $2^rm$ with $m$ odd, and repeated use of $\zeta c_{2^rm}=c_{2^{r-1}m}$ makes all nonzero coefficients vanish. Completeness of the [Fourier basis](../../../../../fourier-basis.md) then says $f$ is constant. Therefore the [doubling map](../../../../../dyadic-transformation.md) has no nonconstant [eigenfunctions](../../../../../eigenfunction.md), and

$$
\boxed{x\mapsto2x\pmod1\text{ is weakly mixing for Lebesgue measure}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
