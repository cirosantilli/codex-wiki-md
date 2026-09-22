<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $f=m_T$. Part (ii) identifies the first superdiagonal block exactly:

$$
\boxed{\bigl(f(B)\bigr)_{k,k+1}=f'(A),}
$$

where $f'$ is the [formal derivative](../../../../../formal-derivative.md). Thus the candidate is $g=f'$. If the [irreducible polynomial](../../../../../irreducible-polynomial.md) $f$ has $f'\ne0$, its [polynomial degree](../../../../../degree-of-a-polynomial.md) makes $f$ and $f'$ coprime. Equivalently, $f$ is a [separable polynomial](../../../../../separable-polynomial.md). This includes every irreducible [polynomial](../../../../../polynomial-split.md) over a [field](../../../../../field.md) of characteristic zero, and every irreducible [polynomial](../../../../../polynomial-split.md) over a [perfect field](../../../../../perfect-field.md).

Under this separability hypothesis, [Bézout's identity for polynomials](../../../../../bezout-s-identity-for-polynomials.md) gives $a(x)f(x)+b(x)f'(x)=1$. Evaluating at $A$ proves that $C=f'(A)$ is an [invertible matrix](../../../../../invertible-matrix.md). Moreover, $f(B)$ has zero diagonal blocks, because $f(A)=0$. It is therefore a [nilpotent matrix](../../../../../nilpotent-matrix.md) with $f(B)^N=0$. The only product of $N-1$ strictly upward block steps that reaches block $(1,N)$ uses the first superdiagonal every time, so

$$
\bigl(f(B)^{N-1}\bigr)_{1,N}=C^{N-1}\ne0.
$$

For $N=1$, the corresponding assertion is simply $f(B)^0=I\ne0$. The [block upper triangular matrix](../../../../../block-upper-triangular-matrix.md) $B$ has

$$
\chi_U(x)=\det(B-xI)=\det(A-xI)^N=(-1)^{nN}f(x)^N.
$$

The [minimal polynomial](../../../../../minimal-polynomial.md) divides this [characteristic polynomial](../../../../../characteristic-polynomial.md). Since $f$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md), it must be a power of $f$; the exact [nilpotency index](../../../../../nilpotency-index.md) just found forces

$$
\boxed{m_U=f^N,\qquad \chi_U=(-1)^{nN}f^N\quad\text{if }f\text{ is separable}.}
$$

**The arbitrary-field qualification is necessary.** In the [rational function field](../../../../../rational-function-field.md) $F=\mathbb F_2(t)$, take $f(x)=x^2-t$. This is an [irreducible polynomial](../../../../../irreducible-polynomial.md): a square of a rational function has even order of vanishing at $t=0$, while $t$ has odd order. Its [formal derivative](../../../../../formal-derivative.md) is zero. With $N=2$,

$$
A=\begin{pmatrix}0&1\\t&0\end{pmatrix},\qquad
B=\begin{pmatrix}A&I\\0&A\end{pmatrix},\qquad
B^2=tI_4.
$$

The off-diagonal block in $f(B)$ is zero, and $m_U=f$, rather than $f^2$. No alternative [polynomial](../../../../../polynomial-split.md) $g$ coprime to $f$ could represent that block: $g(A)=0$ would imply $m_T=f\mid g$. Thus the printed coprimality claim fails as stated over a general [field](../../../../../field.md).

There is also a precise general replacement. In characteristic $p>0$, let $q=p^r$ be the largest power for which $f(x)=h(x^q)$, so that $h'\ne0$; set $q=1$ in characteristic zero. Irreducibility of $f$ implies that $h$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md), so $h$ and $h'$ are coprime. The [binomial theorem](../../../../../binomial-theorem.md) in characteristic $p$ gives $B^q=D^q+K^q$. Expanding $h(D^q+K^q)$, with the coefficients equivalently supplied by the [Hasse derivatives](../../../../../hasse-derivative.md), gives

$$
f(B)=K^qH,
$$

where $H$ commutes with $K$ and is a [block upper triangular matrix](../../../../../block-upper-triangular-matrix.md) whose diagonal blocks are $h'(A^q)$. These blocks are invertible by [Bézout's identity for polynomials](../../../../../bezout-s-identity-for-polynomials.md), since $h(A^q)=f(A)=0$. Thus $H$ is invertible, and

$$
f(B)^s=K^{qs}H^s=0\quad\Longleftrightarrow\quad qs\geq N.
$$

The same [characteristic polynomial](../../../../../characteristic-polynomial.md) and divisibility argument now prove the corrected arbitrary-field answer:

$$
\boxed{m_U(x)=f(x)^{\lceil N/q\rceil},\qquad
\chi_U(x)=(-1)^{nN}f(x)^N.}
$$

This is the [minimal polynomial of a companion block chain](../../../../../minimal-polynomial-of-a-companion-block-chain.md); $q=1$ recovers the intended separable case.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
