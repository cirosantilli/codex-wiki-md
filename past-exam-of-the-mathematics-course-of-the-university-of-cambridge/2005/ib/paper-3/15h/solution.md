<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

Write $y(t)=\sum_{k\geq0}a_kt^k$ at the ordinary point zero. Substituting into the [Legendre differential equation](../../../../../legendre-differential-equation.md) and comparing coefficients gives

$$
\boxed{a_{k+2}=\frac{k(k+1)-\lambda}{(k+1)(k+2)}a_k\quad(k\geq0).}
$$

The two arbitrary coefficients $a_0,a_1$ generate the even and odd series separately, convergent at least for $|t|<1$. A nonzero polynomial of degree $n$ has top coefficient satisfying $[\lambda-n(n+1)]a_n=0$, so $\lambda=n(n+1)$ is necessary. For this value the recurrence in parity $n$ terminates at degree $n$, while the other parity cannot terminate unless its initial coefficient is zero. Thus a polynomial solution exists and is unique up to scale, with $\boxed{P_n(-t)=(-1)^nP_n(t)}$.

For [Orthogonality of Legendre polynomials](../../../../../orthogonality-of-legendre-polynomials.md), write the equation in self-adjoint form $[(1-t^2)P_n']'+n(n+1)P_n=0$. Multiply it by $P_m$, subtract the equation for $P_m$ multiplied by $P_n$, and integrate. The boundary term is $[(1-t^2)(P_mP_n'-P_nP_m')]_{-1}^1=0$, because the functions are polynomials. For $m\ne n$ the eigenvalues differ, giving $\int_{-1}^1P_nP_m=0$. For $m=n$, the integral of the square is positive. Hence $\int P_nP_m=k_n\delta_{nm}$ with $k_n>0$.

Let $G(x,t)=(1-2xt+x^2)^{-1/2}$. The supplied operator $x\partial_x^2x$ means $x\partial_x^2(xG)$, which equals $\partial_x(x^2\partial_xG)$. Expand $G=\sum_na_n(x)P_n(t)$ in the given identity and use the Legendre equation. Each coefficient satisfies

$$
x^2a_n''+2xa_n'-n(n+1)a_n=0,
$$

whose solutions are $a_n=A_nx^n+B_nx^{-n-1}$. Regularity at $x=0$ removes $B_n$. At $t=1$, normalization $P_n(1)=1$ and $G(x,1)=1/(1-x)$ give $\sum_nA_nx^n=\sum_nx^n$, so $A_n=1$. Thus

$$
\boxed{G(x,t)=\sum_{n=0}^\infty x^nP_n(t),\qquad |x|<1.}
$$

A rigorous justification for the expansion and operations is to begin with the Taylor series of $G$ in $x$. It converges uniformly for $|x|\leq r<1$, $-1\leq t\leq1$. Its $x^n$ coefficient is a degree-$n$ polynomial in $t$, and the differential identity makes that coefficient solve the degree-$n$ Legendre equation. Its value at one is one, so it is exactly $P_n$. This avoids assuming an unjustified endpoint convergence of an arbitrary orthogonal expansion.

Square the generating series and integrate, using uniform convergence and orthogonality:

$$
\sum_{n\geq0}k_nx^{2n}=\int_{-1}^1\frac{dt}{1-2xt+x^2}=\frac1x\log\frac{1+x}{1-x}=2\sum_{n\geq0}\frac{x^{2n}}{2n+1}.
$$

Comparing coefficients proves the [generating function and norm of Legendre polynomials](../../../../../generating-function-and-norm-of-legendre-polynomials.md) result

$$
\boxed{k_n=\frac2{2n+1}}.
$$

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
