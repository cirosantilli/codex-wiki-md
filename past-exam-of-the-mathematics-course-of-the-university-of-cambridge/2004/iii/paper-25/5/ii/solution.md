<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\omega=(1+\sqrt{229})/2$. Since $229\equiv1\pmod4$ is squarefree,

$$
\mathcal O_K=\mathbb Z[\omega],\qquad
\omega^2-\omega-57=0,\qquad
N_{K/\mathbb Q}(x+y\omega)=x^2+xy-57y^2.
$$

We first compute the [ideal class group](../../../../../../ideal-class-group.md), rather than assume the proposed extension has the full Hilbert-class-field degree.

The real quadratic [Minkowski bound for ideal classes](../../../../../../minkowski-s-bound.md) is $\sqrt{229}/2<8$. Thus every [ideal](../../../../../../ideal.md) class has an integral representative of norm at most seven. The prime two is inert because $229\equiv5\pmod8$, while seven is inert because $229\equiv5\pmod7$ is a nonsquare. The inert [ideal](../../../../../../ideal.md) $(2)$ has norm four and is principal; a prime above seven has norm forty-nine. The only possible nonprincipal prime factors of these small representatives are therefore primes above three and five.

Reduction of $X^2-X-57$ gives roots $0,1$ modulo three and $2,4$ modulo five. Write

$$
P=(3,\omega),\quad\bar P=(3,\omega-1),\qquad
Q=(5,\omega-4),\quad\bar Q=(5,\omega-2).
$$

Their conjugate pairs multiply to $(3)$ and $(5)$. Direct norm calculations give

$$
N(6+\omega)=-15,\qquad N(15+2\omega)=27.
$$

The element $6+\omega$ vanishes at the residue roots $0$ modulo three and $4$ modulo five, and not at the conjugate roots. Its absolute norm forces each exponent to be one. Likewise $15+2\omega$ vanishes only at the root zero modulo three, and its norm forces exponent three. Thus

$$
\boxed{(6+\omega)=PQ,\qquad(15+2\omega)=P^3.}
$$

These also give the factorizations suggested by the hint: $(13+\sqrt{229})=(2)PQ$ and $(16+\sqrt{229})=P^3$. The classes of $P,Q$ generate the [ideal class group](../../../../../../ideal-class-group.md); the first relation makes $[Q]=[P]^{-1}$ and the second makes $[P]^3=1$. Hence the [class number](../../../../../../class-number.md) divides three.

It is not one. The algebraic integer

$$
\epsilon=7+\omega=\frac{15+\sqrt{229}}2>1
\quad\text{has}\quad N(\epsilon)=-1,
$$

so it is a unit. If $P$ were principal, its generator $a=x+y\omega$ would have norm $\pm3$. Multiply $a$ by a suitable integer power of $\epsilon$ so that

$$
\sqrt{3/\epsilon}\leq|a|<\sqrt{3\epsilon}.
$$

Its conjugate then also has absolute value at most $\sqrt{3\epsilon}$ because $|aa'|=3$. Therefore

$$
|y|\sqrt{229}=|a-a'|\leq|a|+|a'|\leq2\sqrt{3\epsilon}<\sqrt{229}.
$$

The final inequality is $12\epsilon<229$, immediate from the displayed value of $\epsilon$. Thus the integer $y$ is zero, which makes $|N(a)|=x^2=3$ impossible. Consequently

$$
\boxed{\operatorname{Cl}(K)\cong C_3,\qquad h_K=3.}
$$

This proves the [ideal class group of Q of square root 229](../../../../../../ideal-class-group-of-q-of-square-root-229.md). No claim that $\epsilon$ is a fundamental unit is needed. Its norm minus one also realizes all real sign patterns after multiplication by $-1$, so the ordinary and narrow class numbers agree.

Now let $f(X)=X^3-4X-1$ and let $H$ be its [splitting field](../../../../../../splitting-field.md). The possible rational roots $\pm1$ are not roots, so $f$ is irreducible. Its discriminant is

$$
-4(-4)^3-27(-1)^2=256-27=229.
$$

Thus its [Galois group](../../../../../../galois-group.md) is $S_3$, since an irreducible cubic has group $A_3$ precisely when its discriminant is a square. Its quadratic subfield is $\mathbb Q(\sqrt{229})=K$, and $H/K$ is cyclic of degree three. If $\alpha$ is one root, then $H=K(\alpha)$.

For every rational prime $\ell\ne229$, the reduction of $f$ is separable. Its roots lift in an [unramified extension](../../../../../../unramified-extension.md) containing its residue [splitting field](../../../../../../splitting-field.md), by Hensel's lemma. Hence its [splitting field](../../../../../../splitting-field.md) is unramified over $\mathbb Q$ at all these primes, and consequently over $K$ there.

At 229 there is exactly one double residue root and one simple root:

$$
f(X)\equiv(X+29)^2(X-58)\pmod{229}.
$$

The simple root lifts to $r\in\mathbb Q_{229}$, and division gives $f=(X-r)q$ with $q$ monic quadratic. The discriminant-product identity is

$$
\operatorname{disc}(f)=\operatorname{disc}(q)q(r)^2.
$$

Here $q(r)=f'(r)$ is a unit, since $r$ has the simple residue root. Therefore the quadratic discriminant has [valuation](../../../../../../valuation.md) one, and its root field is the ramified quadratic field $\mathbb Q_{229}(\sqrt{229})$. This is already the completion of $K$. The local [splitting field](../../../../../../splitting-field.md) has no further extension over it: the simple root lies in $\mathbb Q_{229}$ and the other two lie in that quadratic field. Thus $H/K$ is unramified even at 229. Equivalently its rational inertia is a transposition and has trivial intersection with $A_3$.

The positive cubic discriminant gives three distinct real roots, so $H$ is totally real and there is no infinite ramification over $K$. We have exhibited an everywhere-unramified cyclic extension of degree $h_K=3$. The Hilbert-class-field characterization in part (i) now proves

$$
\boxed{H_K=\mathbb Q(\sqrt{229},\alpha),\qquad\alpha^3-4\alpha-1=0.}
$$

Finally let $p\ne229$ be rational prime. A [prime ideal](../../../../../../prime-ideal.md) of norm $p$ is principal if and only if its [Artin symbol](../../../../../../artin-symbol.md) in $H_K/K$ is trivial. If it is principal, a generator has norm $\pm p$; multiplying by the norm-minus-one unit if necessary gives norm $+p$. Conversely an element of norm $p$ generates a [prime ideal](../../../../../../prime-ideal.md) of norm $p$. Hence representation by $x^2+xy-57y^2$ is equivalent to $p$ splitting in $K$ with trivial [Artin symbol](../../../../../../artin-symbol.md) in $H_K/K$, or to complete splitting of $p$ in $H_K/\mathbb Q$.

Let $\tau_p\in S_3$ be its rational Frobenius, defined up to conjugacy. Its restriction to the discriminant quadratic field is its sign. The splitting criterion for that quadratic field is

$$
p\text{ splits in }K\iff(p/229)=1.
$$

For odd $p$ this follows by [quadratic reciprocity](../../../../../../quadratic-reciprocity.md) from the character of discriminant 229; for $p=2$ both criteria are negative since $229\equiv5\pmod8$. The polynomial is separable modulo $p$, and the degrees of its factors are the cycle lengths of $\tau_p$. Thus a root modulo $p$ means that $\tau_p$ fixes a root. An even permutation of three letters with a fixed point is the identity: a nonidentity three-cycle has none. Therefore the two stated conditions together are exactly complete splitting in $H_K$, and

$$
\boxed{p=x^2+xy-57y^2\text{ for some }x,y\in\mathbb Z
\iff (p/229)=1\ \text{and }X^3-4X-1\text{ has a root modulo }p.}
$$

This is [prime representation by the norm form of Q of square root 229](../../../../../../prime-representation-by-the-norm-form-of-q-of-square-root-229.md), with the norm sign and the prime two explicitly covered.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
