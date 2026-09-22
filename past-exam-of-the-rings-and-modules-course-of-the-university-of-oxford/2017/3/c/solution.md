<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $J=\begin{pmatrix}0&-2\\1&0\end{pmatrix}$, so the displayed [rational canonical form](../../../../rational-canonical-form.md) of $T$ is $J\oplus J$. Since $J^2=-2I_2$, we have $T^2=-2I_4$.

If $a=0$, then $U=bI_4$ is a [scalar matrix](../../../../scalar-matrix.md). Its [invariant factors of a linear operator](../../../../invariant-factors-of-a-linear-operator.md) are four copies of $t-b$, so its rational canonical form is

$$
\boxed{C(t-b)^{\oplus4}=bI_4\qquad(a=0).}
$$

Here $m_U=t-b$ and $c_U=(t-b)^4$, including when $b=0$.

Now let $a\ne0$ and put

$$
q(t)=(t-b)^2+2a^2=t^2-2bt+(b^2+2a^2).
$$

On each two-dimensional invariant block, $A=aJ+bI_2$ satisfies $q(A)=0$. The vectors $e_1,Ae_1$ form a [cyclic vector](../../../../cyclic-vector.md) basis, since their coordinate matrix is $P=\begin{pmatrix}1&b\\0&a\end{pmatrix}$ with [determinant](../../../../determinant.md) $a\ne0$. Directly,

$$
P^{-1}AP=
\begin{pmatrix}0&-(b^2+2a^2)\\1&2b\end{pmatrix}=C(q).
$$

Applying this basis change to both blocks gives

$$
\boxed{\operatorname{RCF}(U)=
\begin{pmatrix}
0&-(b^2+2a^2)&0&0\\
1&2b&0&0\\
0&0&0&-(b^2+2a^2)\\
0&0&1&2b
\end{pmatrix}\qquad(a\ne0).}
$$

Thus $m_U=q$ and $c_U=q^2$. In particular there are two invariant factors $q,q$, rather than a single block for $q^2$. Also $q(t)>0$ for every real $t$, so it is an [irreducible polynomial](../../../../irreducible-polynomial.md) over $\mathbb R$. This is an instance of [rational canonical form under an affine change](../../../../rational-canonical-form-under-an-affine-change.md).

Finally $T^2=-2I_4$ implies $T^{-1}=-T/2$. Substituting $a=-1/2$, $b=0$ in the preceding result gives $q(t)=t^2+1/2$, and hence

$$
\boxed{\operatorname{RCF}(T^{-1})=
\begin{pmatrix}
0&-1/2&0&0\\
1&0&0&0\\
0&0&0&-1/2\\
0&0&1&0
\end{pmatrix}.}
$$

Its minimal polynomial is $t^2+1/2$ and its characteristic polynomial is $(t^2+1/2)^2$. The normalized reciprocal of $t^2+2$ is also $t^2+1/2$, agreeing with [rational canonical form of an inverse](../../../../rational-canonical-form-of-an-inverse.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
