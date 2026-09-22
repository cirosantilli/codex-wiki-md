<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $b=(\ell+1)a$, $R(r)=r^\ell e^{-r/b}$ and $Y(\theta,\phi)=\sin^\ell\theta e^{i\ell\phi}$, for nonnegative integer $\ell$. The [angular Laplacian](../../../../laplace-beltrami-operator.md) satisfies $\Delta_{S^2}Y=-\ell(\ell+1)Y$. Direct radial differentiation gives

$$
R''+\frac2rR'-\frac{\ell(\ell+1)}{r^2}R=\left(\frac1{b^2}-\frac{2(\ell+1)}{br}\right)R.
$$

Because $(\ell+1)/b=1/a$, the $1/r$ contribution cancels the [Coulomb potential](../../../../coulomb-potential-energy.md) in the [Hamiltonian](../../../../hamiltonian.md). Therefore

$$
\boxed{H(RY)=-\frac{\hbar^2}{2mb^2}RY,\qquad E=-\frac{\hbar^2}{2m(\ell+1)^2a^2}.}
$$

The [volume element](../../../../volume-element.md) contributes $r^2\sin\theta$. The squared state factors into radial, polar and uniform azimuthal densities, so the angular [normalization](../../../../normalization.md) cancels in every [radial expectation](../../../../expectation-value.md). With $I_j=\int_0^\infty r^je^{-2r/b}\,dr$,

$$
\boxed{\mathbb E[r^k]=\frac{I_{2\ell+2+k}}{I_{2\ell+2}}.}
$$

The supplied integration-by-parts recurrence gives $I_{j+1}=(j+1)bI_j/2$. Hence

$$
\boxed{\mu=\mathbb E[r]=(\ell+\tfrac32)b,\quad\mathbb E[r^2]=(\ell+2)(\ell+\tfrac32)b^2,\quad\operatorname{Var}(r)=\frac{2\ell+3}{4}b^2.}
$$

In particular $\operatorname{Var}(r)/\mu^2=(2\ell+3)^{-1}$. Put $h=(2\ell+3)^{-1/3}$. [Chebyshev's inequality](../../../../chebyshev-s-inequality.md) gives

$$
\boxed{\mathbb P(|1-r/\mu|>h)\leq\frac1{(2\ell+3)h^2}=h.}
$$

For the polar variable set $J_j=\int_0^\pi\sin^j\theta\,d\theta$. The polar density is proportional to $\sin^{2\ell+1}\theta$, so

$$
\boxed{\mathbb E[\cos^2\theta]=1-\frac{J_{2\ell+3}}{J_{2\ell+1}}=\frac1{2\ell+3}.}
$$

An exact expression for the requested tail, as well as its useful estimate, is

$$
\boxed{\mathbb P(|\cos\theta|>h)=\frac{\int_h^1(1-z^2)^\ell\,dz}{\int_0^1(1-z^2)^\ell\,dz}\leq\frac{\mathbb E[\cos^2\theta]}{h^2}=h.}
$$

The inequality is [Markov's inequality](../../../../markov-s-inequality.md) applied to $\cos^2\theta$. If a finite expression is desired, expand $(1-z^2)^\ell$: the numerator is $\sum_{j=0}^\ell(-1)^j\binom\ell j(1-h^{2j+1})/(2j+1)$ and the denominator is the same sum with $h=0$.

By the [union bound](../../../../boole-s-inequality.md), with [probability](../../../../probability.md) at least $1-2h$ both $|r/\mu-1|\leq h$ and $|\cos\theta|\leq h$. The height above the equatorial plane is then at most $(1+h)\mu h$. The cylindrical radius differs from $\mu$ by at most $\mu h+(1+h)\mu h^2$. Thus the distance from the circle of radius $\mu$ in the equatorial plane is $O(\mu h)$ with [probability](../../../../probability.md) tending to one. This is relative concentration around a growing circle; it does not assert an absolutely shrinking thickness. The [probability concentration of a circular Coulomb eigenstate](../../../../probability-concentration-of-a-circular-coulomb-eigenstate.md) is a precise version of the large-angular-momentum orbit picture.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
