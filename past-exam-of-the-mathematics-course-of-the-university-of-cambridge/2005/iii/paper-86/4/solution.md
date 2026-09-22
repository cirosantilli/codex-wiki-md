<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [growth order of a meromorphic function](../../../../../growth-order-of-a-meromorphic-function.md) is

$$
\rho(f)=\limsup_{R\to\infty}\frac{\log^+T_f(R)}{\log R}.
$$

The order of the integrated count is defined analogously using $\log^+N(R;a)$, with an identically zero count assigned order zero. Constants have function order zero. These are growth orders, not local zero or [pole](../../../../../pole.md) orders. For nonconstant $f$, the first main theorem gives $\rho(N(\cdot;a))\le\rho(f)$ for every target.

Use the truncated [Nevanlinna second main theorem](../../../../../nevanlinna-second-main-theorem.md) in the following standard form: for distinct fixed targets $a_1,\ldots,a_q$,

$$
(q-2)T_f(R)\le\sum_{j=1}^q\overline N(R;a_j)+S_f(R),\qquad
S_f=O(\log^+T_f+\log R),
$$

outside an exceptional set of radii of finite linear measure. For finite order the error is $O(\log R)$; replacing each truncated count by its full count preserves the inequality.

Suppose $0<\rho(f)<\infty$ and three targets have counting orders below $\rho(f)$. Choose $\mu$ strictly between the maximum of their three orders and $\rho(f)$. Each full count is at most $R^\mu$ eventually. The theorem with $q=3$ then gives $T_f(R)\le C R^\mu$ for sufficiently large radii outside the exceptional set. Its tail measure is eventually less than one, so every interval $[R,R+1]$ contains a nonexceptional radius $R'$. Monotonicity of the characteristic yields $T_f(R)\le T_f(R')\le C(R+1)^\mu$ for all large $R$. This contradicts its order. If $\rho(f)=0$, all the counting orders are already zero. Hence the [counting-order exceptions for a finite-order meromorphic function](../../../../../counting-order-exceptions-for-a-finite-order-meromorphic-function.md) satisfy

$$
\boxed{\rho(N(\cdot;a))=\rho(f)\quad\text{apart from at most two targets}.}
$$

The exponential has order one but omits both zero and infinity, so those two counts are zero; this realizes two exceptions.

For a [Möbius map](../../../../../mobius-transformation.md) $U(w)=(aw+b)/(cw+d)$ with $ad-bc\ne0$, translation and multiplication by a nonzero constant change $T$ by $O(1)$, as follows directly from the proximity inequalities and unchanged [pole](../../../../../pole.md) multiplicities. The first main theorem also gives $T(1/h)=T(h)+O(1)$. If $c=0$, $U$ is affine. If $c\ne0$, write $U(w)=a/c+K/(cw+d)$ with $K\ne0$ and use these three elementary operations. Thus $T_{U\circ f}=T_f+O(1)$, proving

$$
\boxed{\rho(U\circ f)=\rho(f).}
$$

For the sum, a [pole](../../../../../pole.md) of $f_1+f_2$ has order no larger than the sum of the two [pole](../../../../../pole.md) orders, and

$$
\log^+|f_1+f_2|\le\log2+\log^+|f_1|+\log^+|f_2|.
$$

Therefore $T_{f_1+f_2}\le T_{f_1}+T_{f_2}+O(1)$ and

$$
\boxed{\rho(f_1+f_2)\le\max(\rho(f_1),\rho(f_2)).}
$$

If $\rho(f_1)>\rho(f_2)$, apply the same inequality to $f_1=(f_1+f_2)-f_2$. It forces $\rho(f_1)\le\max(\rho(f_1+f_2),\rho(f_2))$, hence the sum's order equals $\rho(f_1)$. The reversed case is identical. This reasoning also handles an infinite larger order. For equal orders cancellation can be strict: $f_1=e^z$, $f_2=-e^z$ both have order one, but their sum is zero of order zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
