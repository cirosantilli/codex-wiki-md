<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $\lambda>0$, choose a sample $k_n$ satisfying $\chi(k_n)=i\pi n$ for each integer $n$. A convenient branch is

$$
\boxed{k_n=i\left[\frac{\pi n}l+\sqrt{\left(\frac{\pi n}l\right)^2+\lambda}\right],\qquad n\in\mathbb Z.}
$$

Thus $k_n+\lambda/k_n=2\pi in/l$. The undivided identity in part (d) gives

$$
\Phi(k_n)=-\frac{iC(k_n)}{2\sinh\chi(\bar ak_n)},\qquad
C(k_n)=\cosh\chi(\bar ak_n)\Psi(k_n)+(-1)^n\Psi(\bar ak_n)+\Psi(ak_n).
$$

Rotation invariance makes all three vertex values equal, so $q(l/2)=q(-l/2)$. The exponential has the same endpoint value $(-1)^n$ at both ends. [Integration by parts](../../../../../../integration-by-parts.md) in the definition of $\Phi$ therefore gives

$$
\Phi(k_n)=-\frac12\left(k_n-\frac\lambda{k_n}\right)Q_n,\qquad
Q_n=\int_{-l/2}^{l/2}e^{2\pi ins/l}q(s)ds.
$$

These are the [Fourier coefficients](../../../../../../fourier-coefficient.md) with the positive-exponential convention. Hence the **computed boundary trace** is

$$
\boxed{\begin{aligned}
Q_n&=\frac{i[\cosh\chi(\bar ak_n)\Psi(k_n)+(-1)^n\Psi(\bar ak_n)+\Psi(ak_n)]}
{(k_n-\lambda/k_n)\sinh\chi(\bar ak_n)},\\
q(s)&=\frac1l\sum_{n\in\mathbb Z}Q_ne^{-2\pi ins/l}.
\end{aligned}}
$$

Every quantity in this [rotationally invariant Neumann reconstruction in an equilateral triangle](../../../../../../rotationally-invariant-neumann-reconstruction-in-an-equilateral-triangle.md) is determined by the prescribed $f$. To check that no denominator was silently divided by zero, put $k_n=i\kappa_n$, $\kappa_n>0$. Then

$$
k_n-\lambda/k_n=i(\kappa_n+\lambda/\kappa_n),\qquad
\operatorname{Re}\chi(\bar ak_n)=\frac{\sqrt3l}4(\kappa_n+\lambda/\kappa_n)>0.
$$

Neither factor vanishes for $\lambda>0$. For sufficiently smooth compatible traces, the periodic extension of $q$ is continuous and piecewise smooth; the [Fourier series](../../../../../../fourier-series-split.md) recovers $q$, with the usual endpoint convention. Reality implies $Q_{-n}=\overline{Q_n}$ even though the sampling formula uses complex arguments.

For $\lambda=0$, first impose the zero-flux compatibility from part (c). For $n\ne0$ take the nonzero root $k_n=2\pi in/l$ and use the same coefficient formula with $\lambda=0$. The coefficient $Q_0$ is an arbitrary real constant times $l$, expressing the additive constant for this problem with a [Neumann boundary condition](../../../../../../neumann-boundary-condition.md). The zero sample cannot determine it. For example, $f=0$ admits every constant solution, so no uniquely specified $q(s)$ is possible without a normalization.

For completeness, negative parameters can be handled without assuming away resonances. Let $\phi_j$ be a real orthonormal [eigenbasis](../../../../../../eigenbasis.md) of the [Neumann Laplacian](../../../../../../neumann-laplacian.md), with $-\Delta\phi_j=\mu_j\phi_j$, and define

$$
F_j=\int_{\partial D}f\,\phi_j\,ds,
$$

using the corresponding oriented $f$ on each side. The weak equation and [Green's first identity](../../../../../../green-s-first-identity.md) give the explicit coefficient relation

$$
(\mu_j+4\lambda)\langle q,\phi_j\rangle=F_j.
$$

At a nonresonant parameter this determines the unique solution. Its common trace is the continuation of the displayed spectral [Fourier coefficients](../../../../../../fourier-coefficient.md) from $\lambda>0$; choose either nonzero root of $k_n^2-(2\pi in/l)k_n+\lambda=0$. If an individual quotient is $0/0$ at a nonresonant parameter, use its removable limit in $\lambda$, rather than declare a new eigenvalue. For example, a double sampling root can make $k_n-\lambda/k_n=0$ without making the boundary problem singular. The weak coefficient relation proves that the solution is analytic in the parameter wherever no $\mu_j+4\lambda$ vanishes, so these nonresonant limits exist.

At a genuine resonance $\lambda=-\mu_*/4$, the [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) is precisely $F_j=0$ for every $\mu_j=\mu_*$. Necessity follows directly from the coefficient relation. For compatible smooth data, sufficiency follows by dividing all nonresonant coefficients and leaving the resonant ones free. The boundary functional is continuous on $H^1(D)$, so $\sum_j|F_j|^2/(1+\mu_j)<\infty$; away from the finite resonant eigenspace this implies $\sum_j(1+\mu_j)|F_j/(\mu_j-\mu_*)|^2<\infty$. Thus the resulting series converges in $H^1(D)$ and satisfies the weak equation, not just its individual coefficient identities. The full solution and its boundary values are thus

$$
q(x,y)=\sum_{\mu_j\ne\mu_*}\frac{F_j}{\mu_j-\mu_*}\phi_j(x,y)
+\sum_{\mu_j=\mu_*}b_j\phi_j(x,y),\qquad b_j\in\mathbb R,
$$

with convergence in the weak solution space and the associated trace sense. Rotation averaging selects the common-side component; a nonsymmetric homogeneous addition can have different traces on the three sides. Incompatible resonant data give no solution. **For arbitrary real $\lambda$, compatibility and the free homogeneous components are essential; the source does not specify conditions that would select a unique trace at resonance.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
