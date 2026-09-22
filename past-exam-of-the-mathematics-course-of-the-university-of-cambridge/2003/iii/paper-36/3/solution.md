<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [root of unity over a finite field](../../../../../root-of-unity-over-a-finite-field.md) is an element $a\in\overline{\mathbb F}_q$ satisfying $a^n=1$, with $n\geq1$; the [algebraic closure](../../../../../algebraic-closure.md) is essential because all roots need not lie in the base [field](../../../../../field.md). Write $p=\operatorname{char}\mathbb F_q$ and $n=p^a m$, where $p\nmid m$. In characteristic $p$,

$$
T^n-1=(T^m-1)^{p^a}.
$$

The latter [polynomial](../../../../../polynomial-split.md) has $m$ distinct roots, since the derivative $mT^{m-1}$ is nonzero at every root. Those roots are closed under multiplication and inversion and contain $1$, so $E(n,q)$ is a finite multiplicative subgroup of a [field](../../../../../field.md). The proof in the preceding solution makes it a [cyclic group](../../../../../cyclic-group.md). In particular

$$
\boxed{|E(n,q)|=m,\qquad |E(n,q)|=n\text{ if }\gcd(n,q)=1.}
$$

This also explains why the coprimality qualification is needed.

The [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb F_{q^s}^{\times}$ is cyclic of order $q^s-1$. It contains the entire group of $m$th roots precisely when $m\mid q^s-1$. For necessity, a generator of $E(n,q)$ has order $m$ and [Lagrange's theorem](../../../../../lagrange-s-theorem.md) applies. For sufficiency, a [cyclic group](../../../../../cyclic-group.md) whose order is divisible by $m$ contains $m$ roots of $T^m-1$; since there are exactly $m$ roots in the [algebraic closure](../../../../../algebraic-closure.md), these are all of them. Hence the least positive extension degree is

$$
\boxed{s=\operatorname{ord}_m(q)\quad(m>1),\qquad s=1\quad(m=1).}
$$

Here $\operatorname{ord}_m(q)$ is the [multiplicative order](../../../../../multiplicative-order.md) of the residue class of $q$ modulo $m$. If $n$ is coprime to $q$, replace $m$ by $n$. Existence of this order follows because $q$ is a unit modulo $m$.

A primitive $n$th [root of unity over a finite field](../../../../../root-of-unity-over-a-finite-field.md) has [multiplicative order](../../../../../multiplicative-order.md) exactly $n$. If $p\mid n$, no such element exists, since all roots have order dividing $m<n$. If $\gcd(n,q)=1$, choose a generator $\zeta$ of $E(n,q)$. The element $\zeta^j$ has order $n/\gcd(n,j)$, so it is primitive precisely when $\gcd(n,j)=1$. Therefore **there are $\varphi(n)$ primitive roots**, with $\varphi$ the [Euler totient function](../../../../../euler-totient-function.md).

If $\omega$ is primitive of order $n$, then $\omega\in\mathbb F_{q^\ell}$ exactly when $\omega^{q^\ell}=\omega$, equivalently $n\mid q^\ell-1$. The implication from that equality to membership follows because the roots of $T^{q^\ell}-T$ form $\mathbb F_{q^\ell}$, as proved in the preceding solution. Consequently

$$
\boxed{\min\{\ell\geq1:\omega\in\mathbb F_{q^\ell}\}=\operatorname{ord}_n(q)}
$$

for $n>1$, and the degree is one for $n=1$. This is also the length of the [finite-field Frobenius automorphism](../../../../../finite-field-frobenius-automorphism.md) orbit of $\omega$.

Using the same $(1,u)$ [basis](../../../../../basis.md) of $\mathbb F_9$ as before, the fourth roots of unity are

$$
\boxed{E(4,9)=\{1,-1,u,-u\}=\{(1,0),(2,0),(0,1),(0,2)\}.}
$$

There are four, they are already in $\mathbb F_9$, and the primitive fourth roots are the two vectors $(0,1)$ and $(0,2)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
