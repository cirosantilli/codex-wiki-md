<h1 id="question-5/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Put $u(r,\theta)=R(r)\Theta(\theta)$ in [Laplace's equation](../../../../../../laplace-equation.md) and multiply by $r^2/(R\Theta)$ on intervals where the factors are nonzero. [Separation of variables](../../../../../../separation-of-variables.md) gives

$$
\frac{r^2R''+rR'}R=-\frac{\Theta''}{\Theta}=\lambda,
$$

and hence

$$
\Theta''+\lambda\Theta=0,\qquad
r^2R''+rR'-\lambda R=0.
$$

The angular [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) are $\Theta(0)=\Theta(\pi/2)=0$. Multiplication of the angular equation by $\Theta$, followed by [integration by parts](../../../../../../integration-by-parts.md), gives

$$
\lambda\int_0^{\pi/2}\Theta^2\,d\theta
=\int_0^{\pi/2}(\Theta')^2\,d\theta.
$$

For a nonzero angular [eigenfunction](../../../../../../eigenfunction.md) this forces $\lambda>0$: equality would make $\Theta$ constant and then zero. Write $\lambda=\mu^2$. The first angular condition removes the [cosine](../../../../../../cosine.md) term, and the second requires $\sin(\mu\pi/2)=0$. Thus

$$
\mu=2n,\qquad \lambda_n=4n^2,\qquad
\Theta_n(\theta)=\sin(2n\theta),\qquad n=1,2,\ldots.
$$

The radial [Cauchy-Euler equation](../../../../../../cauchy-euler-equation.md) has the two solutions $r^{2n}$ and $r^{-2n}$. By [superposition](../../../../../../superposition-principle.md), the general separated [series](../../../../../../series-mathematics.md) is therefore

$$
\boxed{u(r,\theta)=\sum_{n=1}^{\infty}
\bigl(A_nr^{2n}+B_nr^{-2n}\bigr)\sin(2n\theta)}.
$$

The coefficients are arbitrary subject to convergence with enough [partial derivatives](../../../../../../partial-derivative.md) on compact subsets to give a [harmonic function](../../../../../../harmonic-function.md) and to the prescribed zero values on the two open radial edges. Completeness of the sine [eigenfunctions](../../../../../../eigenfunction.md) gives the usual series representation for solutions smooth up to those edges on closed radial subintervals. There is no constant or logarithmic zero mode because its angular factor would be linear in $\theta$ and would vanish at both ends only if it were zero.

**The negative powers must be retained:** the stated domain omits $r=0$, and no boundedness at that vertex is prescribed. For example, $r^{-2}\sin(2\theta)$ is a [harmonic function](../../../../../../harmonic-function.md) satisfying both edge conditions. An additional boundedness condition as $r\to0$ would remove all $B_n$; an additional value on the circular arc would then determine the remaining $A_n$. With only the conditions in the paper, neither restriction is available and the solution is not unique.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 5](../../question-5.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
