<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) gives, for a bounded [coercive bilinear form](../../../../coercive-bilinear-form.md) on a real [Hilbert space](../../../../hilbert-space-split.md) and every [bounded linear functional](../../../../continuous-linear-functional.md), a unique vector representing that functional through the form, with the inverse bound supplied by coercivity. The [Fredholm alternative](../../../../fredholm-alternative.md) for a [compact operator](../../../../compact-operator-split.md) $K$ says that $I+\mu K$ is invertible if its kernel is zero; in general its range is closed and consists exactly of vectors orthogonal to $\ker(I+\mu K)^*$ in the Hilbert-space case.

[Uniform ellipticity](../../../../uniformly-elliptic-operator.md) gives $\sum a_{ij}\xi_i\xi_j\geq\theta|\xi|^2$ for some $\theta>0$. Bounded coefficients make $B_\lambda$ bounded on $H^1$, and for $\lambda<-\gamma$,

$$
B_\lambda[u,u]\geq\theta\|Du\|_2^2+(-\gamma-\lambda)\|u\|_2^2\geq\min\{\theta,-\gamma-\lambda\}\|u\|_{H^1}^2.
$$

The forcing $v\mapsto\int fv$ is bounded on $H^1$. The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) therefore gives **a unique [weak solution](../../../../weak-solution.md) for every $\lambda<-\gamma$**.

When $c=0$, choose the shift $\lambda_0=-1$ and let $Kf$ be the unique solution of $B[Kf,v]+\int(Kf)v=\int fv$. Thus $K=(L+I)^{-1}$ in the weak sense. The equation $Lu=f$ is equivalent to $u=K(f+u)$, or

$$
\boxed{(I-K)u=Kf.}
$$

Conversely a solution in $L^2$ of this operator equation lies in $H^1$ because it equals $K(f+u)$, and satisfies the variational equation. The assumed boundedness $K:L^2\to H^1$, followed by the compact Rellich embedding $H^1\hookrightarrow L^2$, proves [compactness](../../../../compact-space.md) of $K$ as an $L^2$ operator.

By the supplied kernel assumption, $\ker(I-K)$ consists of constants. Also $K1=1$. Since $K$ is a [self-adjoint operator](../../../../self-adjoint-operator.md), the [Fredholm alternative](../../../../fredholm-alternative.md) condition is $Kf\perp1$, and

$$
\langle Kf,1\rangle=\langle f,K1\rangle=\int_\Omega f.
$$

Therefore **a [weak solution](../../../../weak-solution.md) exists exactly when the mean of $f$ is zero**, and solutions differ by a constant. On a disconnected domain the actual kernel would consist of constants on each component and the condition would apply separately on each; the question's given kernel assumption specifies the single-constant case.

For a general coefficient matrix, the stated variational definition encodes zero conormal flux $(aDu)\cdot n=0$. It agrees with ordinary zero normal derivative only under additional conditions on $a$. The argument above uses the [weak formulation](../../../../weak-formulation.md) explicitly defined in the paper, so does not require that stronger boundary identification.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
