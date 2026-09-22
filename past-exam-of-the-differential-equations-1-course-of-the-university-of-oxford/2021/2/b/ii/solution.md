<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The rectangle avoids the singular line $y=0$ exactly when $0<k<1$. There $y>0$, and the largest $|x|$ on $[1-h,1+h]$ is $1+h$. Since $1+1/y$ decreases with $y$, the smallest feasible uniform bound is

$$
\boxed{M(h,k)=(1+h)\frac{2-k}{1-k},\qquad h>0,\ 0<k<1.}
$$

It is attained at $x=1+h$, $y=1-k$. For the [Lipschitz constant](../../../../../lipschitz-constant.md), the [mean value theorem](../../../../../mean-value-theorem.md) gives

$$
|f(x,y)-f(x,z)|=\frac{|x|}{yz}|y-z|\leq\frac{1+h}{(1-k)^2}|y-z|.
$$

The quotients approach this upper bound as $x=1+h$ and $y,z\downarrow1-k$, so the smallest feasible constant is

$$
\boxed{L(h,k)=\frac{1+h}{(1-k)^2}.}
$$

Substitution into part (a) gives

$$
\begin{array}{ll}
\text{M-test:}&h(1+h)\leq A(k):=\dfrac{k(1-k)}{2-k},\\[4pt]
\text{contraction:}&h(1+h)\leq A(k),\quad h(1+h)<B(k):=(1-k)^2.
\end{array}
$$

The [contraction mapping](../../../../../contraction-mapping.md) restriction is automatic for every M-test-admissible $h$ precisely when $A(k)<B(k)$. Because $0<k<1$,

$$
A(k)<B(k)\iff k<(1-k)(2-k)\iff k^2-4k+2>0.
$$

Therefore

$$
\boxed{0<k<2-\sqrt2}
$$

is exactly the range where the two proofs guarantee all the same closed symmetric intervals, including the largest M-test interval.

For completeness, set $h_M=(\sqrt{1+4A(k)}-1)/2$ and $h_C=(\sqrt{1+4B(k)}-1)/2$. The M-test allows $0<h\leq h_M$; the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) allows $0<h\leq h_M$ with $h<h_C$. At $k=2-\sqrt2$, these have the same supremum $h_M=h_C$, but contraction excludes the endpoint $h=h_M$. For $2-\sqrt2<k<1$, it gives the strictly shorter range $0<h<h_C<h_M$. For a particular $h$, both proofs work exactly when both displayed inequalities hold, even for these larger $k$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
