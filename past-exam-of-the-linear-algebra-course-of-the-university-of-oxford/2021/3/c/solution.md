<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Write

$$
\omega((v,f),(w,g))=f(w)-g(v)
$$

on $V=W\times W'$, where $W'$ is the [dual space](../../../../dual-space-split.md). The [dual pairing](../../../../dual-pairing.md) is [linear](../../../../linearity.md) separately in the [vector](../../../../vector.md) and the [linear functional](../../../../linear-functional.md). For example, for [real numbers](../../../../real-number.md) $a,b$,

$$
\begin{aligned}
\omega(a(v_1,f_1)+b(v_2,f_2),(w,g))
&=(af_1+bf_2)(w)-g(av_1+bv_2)\\
&=a\omega((v_1,f_1),(w,g))+b\omega((v_2,f_2),(w,g)),\\
\omega((v,f),a(w_1,g_1)+b(w_2,g_2))
&=f(aw_1+bw_2)-(ag_1+bg_2)(v)\\
&=a\omega((v,f),(w_1,g_1))+b\omega((v,f),(w_2,g_2)).
\end{aligned}
$$

Thus $\omega$ is a [bilinear form](../../../../bilinear-form-split.md). It is also an [alternating bilinear form](../../../../alternating-bilinear-form.md), since

$$
\omega((v,f),(v,f))=0,\qquad
\omega((w,g),(v,f))=-\omega((v,f),(w,g)).
$$

To prove that this is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md), suppose $(v,f)$ pairs to zero with every $(w,g)$. Setting $g=0$ gives $f(w)=0$ for every $w\in W$, hence $f=0$. Setting $w=0$ gives $g(v)=0$ for every $g\in W'$. If $v\ne0$, [basis extension](../../../../basis-extension.md) supplies a [coordinate functional](../../../../coordinate-functional.md) with $g(v)=1$, a contradiction. Thus $v=0$. The [left radical](../../../../left-radical-of-a-bilinear-form.md) is zero, and the displayed change of sign implies the [right radical](../../../../right-radical-of-a-bilinear-form.md) is zero as well. Hence **$\omega$ is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md)**, making $V$ a [symplectic vector space](../../../../symplectic-vector-space.md).

For the required example take the [coordinate subspace](../../../../coordinate-subspace.md)

$$
U=W\times\{0\}.
$$

Using the definition of the [bilinear orthogonal complement](../../../../orthogonal-complement-for-a-bilinear-form.md) in part (b),

$$
\begin{aligned}
(w,g)\in U^\perp
&\ \Longleftrightarrow\ \omega((v,0),(w,g))=-g(v)=0\quad\text{for every }v\in W\\
&\ \Longleftrightarrow\ g=0.
\end{aligned}
$$

Therefore

$$
\boxed{U^\perp=W\times\{0\}=U.}
$$

This is a [Lagrangian subspace](../../../../lagrangian-subspace.md). Its [dimension](../../../../dimension-vector-space.md) is $\dim W$, exactly half of $\dim V=2\dim W$, so part (b)(i) is satisfied.

There is no contradiction with part (b)(ii): that part asks whether a [direct sum](../../../../direct-sum.md) is guaranteed, and the answer is already no. Moreover, when $W\ne0$, the present [alternating bilinear form](../../../../alternating-bilinear-form.md) is not a [symmetric bilinear form](../../../../symmetric-bilinear-form.md). Choose $v\ne0$ and $f\in W'$ with $f(v)=1$; then

$$
\omega((v,0),(0,f))=-1,\qquad \omega((0,f),(v,0))=1.
$$

It therefore does not satisfy the symmetry hypothesis of part (b)(ii). If $W=0$, then $V=U=0$, and both $U=U^\perp$ and $V=U\oplus U^\perp$ hold trivially.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
