<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix the orientation of the [Berezin integral](../../../../../berezin-integral.md) by defining its measure as the linear functional that extracts the coefficient of $\prod_{i=1}^N(\theta_i\bar\theta_i)$; all monomials of lower degree integrate to zero. In particular $\int\mathcal D(\bar\theta,\theta)\prod_i(\theta_i\bar\theta_i)=1$. This specifies the sign convention in the notation $d^N\bar\theta\,d^N\theta$.

The [Grassmann change-of-variables formula](../../../../../grassmann-change-of-variables-formula.md) gives

$$
d^N\theta'=\det(U)^{-1}d^N\theta,\qquad d^N\bar\theta'=\det(U^*)^{-1}d^N\bar\theta.
$$

For a [unitary matrix](../../../../../unitary-matrix.md), $\det U\det U^*=1$, so the combined measure is invariant. Diagonalize the [Hermitian matrix](../../../../../hermitian-operator.md) $B$ by a unitary change of variables. If its eigenvalues are $b_i$, the integrand factors as $\prod_i(1-b_i\bar\theta_i\theta_i)=\prod_i(1+b_i\theta_i\bar\theta_i)$. Extracting its top coefficient proves the [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md)

$$
\boxed{\int d^N\bar\theta\,d^N\theta\,e^{-\bar\theta_iB_{ij}\theta_j}=\prod_i b_i=\det B.}
$$

The determinant identity also holds without Hermiticity by direct expansion; Hermiticity makes the diagonalization proof immediate.

Let $C(x)=\sum_kx_kC^{(k)}$. Integrating out the [Grassmann variables](../../../../../grassmann-variable.md) first gives the exact polynomial expression

$$
I(g)=\int_{\mathbb R^N}d^Nx\,e^{-x^TAx/2}\det[B-gC(x)].
$$

The requested factorization requires **$B$ to be invertible**, an assumption omitted from the question. Under it, use the formal perturbative [matrix logarithm](../../../../../matrix-logarithm.md) near $g=0$:

$$
\det[B-gC(x)]=\det B\,\exp\left\{\operatorname{Tr}\log[I-gB^{-1}C(x)]\right\}.
$$

Consequently

$$
\boxed{V_{\rm eff}(x)=-\operatorname{Tr}\log[I-gB^{-1}C(x)]=\sum_{m\geq1}\frac{g^m}{m}\operatorname{Tr}[B^{-1}C(x)]^m.}
$$

Expanding $C(x)$ gives exactly the displayed coefficients $V^{(m)}_{k_1\ldots k_m}=(m-1)!\operatorname{Tr}[B^{-1}C^{(k_1)}\cdots B^{-1}C^{(k_m)}]$, and hence $I(g)=\det B\int d^Nx\,e^{-x^TAx/2-V_{\rm eff}(x)}$. The logarithmic representation is a formal series, not a globally convergent logarithm for every $x$: the determinant can have zeros. The original determinant integral remains well-defined for singular $B$, but $I(0)=0$ and the requested normalized expansion then cannot be formed.

There is a second convention to specify. The $x_i$ are real, so a complex Hermitian $A$ gives $x^TAx=x^TA_Rx$, where $A_R=\operatorname{Re}A=(A+A^T)/2$ is real symmetric positive definite. Its Gaussian [covariance matrix](../../../../../covariance-matrix.md) is $A_R^{-1}$. It equals $A^{-1}$ only if $A$ is real symmetric. Thus

$$
I(0)=\det B\,(2\pi)^{N/2}(\det A_R)^{-1/2},\qquad\frac{I(g)}{I(0)}=\mathbb E_{x\sim N(0,A_R^{-1})}[e^{-V_{\rm eff}(x)}].
$$

The effective [Feynman rules](../../../../../feynman-rule.md) are: a bosonic contraction joins indices $k,\ell$ with $(A_R^{-1})_{k\ell}$; an $m$-leg vertex carries $-g^m\operatorname{Sym}V^{(m)}_{k_1\ldots k_m}$; sum all closed [vacuum diagrams](../../../../../vacuum-feynman-diagram.md) with their [symmetry factors](../../../../../feynman-diagram-symmetry-factor.md), including disconnected diagrams. The symmetrization is necessary because the $x_k$ commute: the trace tensor is cyclically invariant but need not be fully symmetric. The minus sign comes from expanding $e^{-V_{\rm eff}}$. Taking the logarithm of the normalized integral instead keeps only connected [vacuum diagrams](../../../../../vacuum-feynman-diagram.md).

Equivalently, retain the fermions: an oriented contraction is $(B^{-1})_{ij}=\langle\theta_i\bar\theta_j\rangle$, the mixed vertex has weight $+gC^{(k)}_{ij}$, and every closed [fermion loop](../../../../../fermion-loop.md) gives a minus sign. The same bosonic covariance joins its $x$ legs. Expanding these contractions recovers the trace vertices above. This is [bosonic trace vertices from a finite fermionic determinant](../../../../../bosonic-trace-vertices-from-a-finite-fermionic-determinant.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
