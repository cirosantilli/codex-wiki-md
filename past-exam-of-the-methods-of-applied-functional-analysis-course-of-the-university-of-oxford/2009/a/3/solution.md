<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) states that a [bounded bilinear form](../../../../bounded-bilinear-form.md) $a$ on a real [Hilbert space](../../../../hilbert-space-split.md) $V$, satisfying $a(v,v)\ge\alpha\|v\|_V^2$ for some $\alpha>0$, has for each $F\in V^*$ a unique $u\in V$ with $a(u,v)=F(v)$ for all $v$. Moreover $\|u\|_V\le\|F\|/\alpha$.

For a [compact operator](../../../../compact-operator-split.md) $K$ on a [Hilbert space](../../../../hilbert-space-split.md), the [Fredholm alternative](../../../../fredholm-alternative.md) says that $I-\lambda K$ has closed range, [finite-dimensional](../../../../finite-dimensional-vector-space.md) [kernel](../../../../kernel-of-a-linear-map-split.md) and cokernel of equal dimension, and

$$
\operatorname{Ran}(I-\lambda K)=\ker(I-\lambda K^*)^\perp\qquad(\lambda\in\mathbb R).
$$

Thus a zero [kernel](../../../../kernel-of-a-linear-map-split.md) gives unique solvability for every right-hand side; a nonzero [kernel](../../../../kernel-of-a-linear-map-split.md) gives solvability exactly under the adjoint [orthogonality](../../../../orthogonal-vectors.md) conditions, and then all solutions differ by a [kernel](../../../../kernel-of-a-linear-map-split.md) [vector](../../../../vector.md).

Take $V=H_0^1(\Omega)$. [Gårding's inequality](../../../../garding-s-inequality.md) supplies constants $a>0$, $b\ge0$ with $B[v,v]\ge a\|v\|_{H^1}^2-b\|v\|_2^2$. Therefore for $\lambda\le-b$ the shifted form $B_\lambda[u,v]=B[u,v]-\lambda(u,v)_{L^2}$ is coercive. It is [bounded](../../../../boundedness.md) for every fixed $\lambda$, and $v\mapsto(f,v)$ is [bounded](../../../../boundedness.md) on $V$. Lax-Milgram gives **unique weak solvability for $\lambda\le-\gamma$, with $\gamma=b$**. The inequality itself follows, for example, by absorbing the drift cross-term $\|b\|_\infty\|\nabla v\|_2\|v\|_2$ using Young's inequality and allowing a lower $L^2$ correction for $c$.

For the [compact inverse and adjoint of a coercive elliptic operator](../../../../compact-inverse-and-adjoint-of-a-coercive-elliptic-operator.md), under the additional zero-shift coercivity assumption, define $Gg\in V$ by $B[Gg,v]=(g,v)$ for all $v\in V$, and let $K$ be this solution viewed in $L^2$. The solution operator is linear and [bounded](../../../../boundedness.md) into $V$, and the [Rellich-Kondrachov](../../../../rellich-kondrachov-theorem.md) [compact embedding](../../../../compact-embedding.md) $V\hookrightarrow L^2$ makes $K$ compact. Rewriting the weak equation as $B[u,v]=(f+\lambda u,v)$ gives

$$
\boxed{(I-\lambda K)u=Kf.}
$$

Conversely an $L^2$ solution of this operator equation lies in $V$, because it equals $K(f+\lambda u)$, and satisfies the weak [differential equation](../../../../partial-differential-equation-split.md).

For constant drift coefficients and zero [Dirichlet](../../../../dirichlet-boundary-condition.md) [traces](../../../../trace-operator.md), [integration by parts](../../../../integration-by-parts.md) gives $\int b_iD_i v\,u=-\int b_i vD_i u$. Symmetry of the principal coefficients therefore makes $B^*[u,v]=B[v,u]$ the unshifted weak form of the displayed formal adjoint. **The shifted adjoint equation requires**

$$
\boxed{B^*[u,v]-\lambda(u,v)=(f,v)\qquad(v\in V).}
$$

The [spectral shift in an adjoint weak formulation](../../../../spectral-shift-in-an-adjoint-weak-formulation.md) is essential: the printed sentence omitting it is false for nonzero $\lambda$. For instance take a smooth ball, $L=-\Delta+1$, any nonzero $u\in C_c^\infty(\Omega)$ and $f=-\Delta u+u$. The printed unshifted identity holds, but $(L^*-\lambda)u=f-\lambda u\ne f$ whenever $\lambda\ne0$. This counterexample also meets zero-shift coercivity and constant-drift assumptions. The corrected identity above is used for the remainder of the argument.

Let $G_*g\in V$ solve $B^*[G_*g,v]=(g,v)$, which exists by Lax-Milgram because the diagonal coercivity is unchanged. For $p,q\in L^2$,

$$
(Kp,q)=B[Gp,G_*q]=(p,G_*q).
$$

Thus $G_*$, viewed as an $L^2$ operator, is exactly $K^*$. Applying this inverse to the corrected shifted adjoint equation gives

$$
\boxed{(I-\lambda K^*)u=K^*f,}
$$

and the converse follows from its range lying in $V$, just as before.

Finally let the original homogeneous equation have a nonzero solution. Its parameter is nonzero, since the unshifted problem is coercive. Fredholm gives solvability precisely when $(Kf,w)=0$ for every $w\in\ker(I-\lambda K^*)$. Such a $w$ satisfies $K^*w=w/\lambda$, so $(Kf,w)=(f,w)/\lambda$. Hence the necessary and sufficient condition is

$$
\boxed{\int_\Omega fw\,dx=0\quad\text{for every }w\in H_0^1(\Omega)\text{ satisfying }(L^*-\lambda)w=0\text{ weakly}.}
$$

When this holds, the solutions are an [affine translate](../../../../affine-subspace.md) of the original [finite-dimensional](../../../../finite-dimensional-vector-space.md) [homogeneous solution space](../../../../kernel-of-a-linear-map-split.md). The compatibility space is the adjoint [kernel](../../../../kernel-of-a-linear-map-split.md); a drift term does not generally permit replacing it by the original [kernel](../../../../kernel-of-a-linear-map-split.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../split.md)
5. [Methods of applied functional analysis course of the University of Oxford](../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
