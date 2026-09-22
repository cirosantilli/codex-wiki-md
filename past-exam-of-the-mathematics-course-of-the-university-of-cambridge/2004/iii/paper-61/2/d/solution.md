<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [Schwarz conjugation of a spectral function](../../../../../../schwarz-conjugation-of-a-spectral-function.md), $F^\sharp(k)=\overline{F(\bar k)}$. Reality of $f,q_N$ and $\lambda$ gives $\Psi^\sharp=\Psi$, $\Phi^\sharp=\Phi$ and $e^\sharp=e$. Conjugating part (c) yields the second relation

$$
e(ak)\Psi(k)+e(-k)\Psi(ak)+\Psi(\bar ak)=-2iA^\sharp(k),
$$

with $A^\sharp=e(ak)\Phi(k)+e(-k)\Phi(ak)+\Phi(\bar ak)$. The explicit $i$ changes sign, while $a$ and $\bar a$ are interchanged.

Choose sampling points satisfying $k_n+\lambda/k_n=2\pi in/\ell$. Put $\varepsilon_n=(-1)^n$ and $\chi_n=\ell(\bar ak_n+\lambda/(\bar ak_n))/2$. Then $e(k_n)=e(-k_n)=\varepsilon_n$ and $e(k_n)e(\bar ak_n)e(ak_n)=1$. Multiply the first relation by $\varepsilon_n$ and subtract the conjugate relation. The coefficient of $\Psi(ak_n)$ vanishes, leaving

$$
\varepsilon_n\bigl[e(\bar ak_n)-e(-\bar ak_n)\bigr]\Psi(k_n)=2i\bigl[\varepsilon_n A(k_n)+A^\sharp(k_n)\bigr].
$$

Thus the Fourier coefficient $N_n=\Psi(k_n)=\int_{-\ell/2}^{\ell/2}e^{2\pi ins/\ell}q_N(s)ds$ is

$$
N_n=\frac{2i\bigl[\cosh\chi_n\,\Phi(k_n)+\varepsilon_n\Phi(\bar ak_n)+\Phi(ak_n)\bigr]}{\sinh\chi_n}.
$$

The endpoint terms in the derivative-free expression for $\Phi$ cancel, because the other two hyperbolic arguments sum to $-i\pi n$ and $\sinh\chi(k_n)=0$. Writing $h(k)=k-\lambda/k$, we obtain the entirely known expression

$$
\boxed{N_n=-\frac{i\bigl[\cosh\chi_n\,h(k_n)H(k_n)+\varepsilon_n h(\bar ak_n)H(\bar ak_n)+h(ak_n)H(ak_n)\bigr]}{\sinh\chi_n},\qquad q_N(s)=\frac1\ell\sum_{n\in\mathbb Z}N_ne^{-2\pi ins/\ell}.}
$$

This [Dirichlet reconstruction in an equilateral triangle](../../../../../../dirichlet-reconstruction-in-an-equilateral-triangle.md) uses [Fourier series](../../../../../../fourier-series-split.md) inversion on the finite side, with convergence in the natural trace norm and pointwise away from endpoints under sufficient smoothness.

For $\lambda>0$, take $k_n=i[\pi n/\ell+\sqrt{(\pi n/\ell)^2+\lambda}]$. It is nonzero for every integer $n$. Moreover $\operatorname{Re}\chi_n=(\sqrt3\ell/4)[v+\lambda/v]>0$ when $k_n=iv$, so the denominator cannot vanish. For $\lambda=0$ use $k_n=2\pi in/\ell$ for $n\ne0$; the remaining coefficient is $N_0=0$, since the [divergence theorem](../../../../../../divergence-theorem.md) gives $3\int q_N=\int_D\Delta q=0$. This includes the constant harmonic solution.

For negative nonresonant parameters, use either root of the sampling equation and analytic continuation of the reconstruction. Any zero denominator at a parameter where the Dirichlet operator remains invertible is removable: the uniquely determined trace, and hence its Fourier coefficients, depend analytically on that parameter. Evaluate such values by limits rather than claiming a pole or dividing by zero.

At a true [Dirichlet resonance in an equilateral triangle](../../../../../../dirichlet-resonance-in-an-equilateral-triangle.md), the request for a uniquely determined normal trace is false. A concrete counterexample uses the triangle's affine barycentric coordinates $\beta_1+\beta_2+\beta_3=1$. The function

$$
h=\prod_{j=1}^3\sin(\pi\beta_j)=\frac14\sum_{j=1}^3\sin(2\pi\beta_j)
$$

is positive inside and zero on the boundary. Since $|\nabla\beta_j|=2/(\sqrt3\ell)$, direct differentiation gives $\Delta h=-16\pi^2h/(3\ell^2)$. At $\lambda=-4\pi^2/(3\ell^2)$ both $q=0$ and $q=h$ have the same zero Dirichlet data, but different normal derivatives. On a side where $\beta_1=0$, the latter derivative is $-2\pi\sin^2(\pi\beta_2)/(\sqrt3\ell)$, not zero.

In general, if $-4\lambda$ is a Dirichlet eigenvalue, the [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) is $\int_{\partial D}f\,\partial_n\phi\,ds=0$ for every eigenfunction $\phi$ at that eigenvalue. This follows from [Green's second identity](../../../../../../green-second-identity.md). When these conditions hold, the complete answer is $q=q_p+\sum_jc_j\phi_j$ and $q_N^{(r)}=(q_p)_N^{(r)}+\sum_jc_j(\partial_n\phi_j)|_r$, with arbitrary real coefficients $c_j$. A rotation-invariant particular solution may be used, but homogeneous additions need not be invariant. Such noninvariant eigenfunctions must exist: otherwise the complete Dirichlet eigenbasis would span only the proper rotation-invariant subspace of $L^2(D)$. Thus the source's unrestricted real parameter needs this resonance qualification in both (c) and (d).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
