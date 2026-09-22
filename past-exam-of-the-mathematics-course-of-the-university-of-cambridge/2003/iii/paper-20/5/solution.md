<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [propositional geometric theory](../../../../../propositional-geometric-theory.md) has primitive propositions and sequents between formulas built with finite conjunction and arbitrary set-indexed disjunction. Start with the free [frame](../../../../../complete-heyting-algebra.md) on the primitives, identify conjunction with [meet](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) and disjunction with [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md), and impose each sequent as an inequality. The resulting quotient [frame](../../../../../complete-heyting-algebra.md) is $\mathcal O(X_T)$. In the [sheaf topos](../../../../../grothendieck-topos.md) $\operatorname{Sh}(X_T)$, interpret each primitive as the [subterminal sheaf](../../../../../subterminal-sheaf.md) corresponding to its generating open. Operations on these [subterminal sheaves](../../../../../subterminal-sheaf.md) are precisely the [frame](../../../../../complete-heyting-algebra.md) operations, so every imposed sequent is valid. This constructs the canonical model.

For a [commutative ring](../../../../../commutative-ring.md) $R$, denote the generator attached to $r$ by $U_r$. The presentation implies

$$
U_1=1,\qquad U_0=0,\qquad U_r\wedge U_s=U_{rs},\qquad U_{r+s}\leq U_r\vee U_s.
$$

The product equality uses the multiplication implication in one direction and both factor implications in the other; the latter follow by commuting $r,s$. A [ring homomorphism](../../../../../ring-homomorphism.md) $\varphi:R\to S$ sends these relations to the corresponding ones in $S$. It therefore gives a [frame homomorphism](../../../../../frame-homomorphism.md) $U_r\mapsto U_{\varphi(r)}$ and hence **a map $X_S\to X_R$ of [locales](../../../../../locale.md)**.

If $ar+bs=1$, then

$$
1=U_{ar+bs}\leq U_{ar}\vee U_{bs}\leq U_r\vee U_s,
$$

so the two opens cover. Conversely let $S=R/(r,s)$ and pull back a putative cover along $X_S\to X_R$. Both generators become $U_0$, so $1=0$ in $\mathcal O(X_S)$. The allowed degeneracy criterion gives $0=1$ in $S$, equivalently $1\in(r,s)$. Thus

$$
\boxed{U_r\vee U_s=1\iff(r,s)=R\iff\exists a,b\in R:\ ar+bs=1.}
$$

This necessity argument never selects a [prime ideal](../../../../../prime-ideal.md).

Finite intersections of the generating opens are again generators, so they form a basis. Assign $R[r^{-1}]$ to $U_r$. The [localization of a ring](../../../../../localization-of-a-ring.md) carries its ordinary addition and multiplication of fractions; equality of $a/r^n$ and $b/r^m$ means that some power of $r$ annihilates the cross-multiplied difference. On $U_r\cap U_s=U_{rs}$, restriction is further [localization](../../../../../localization-of-a-ring.md).

We also justify restriction for any inclusion of basic opens. Adding the condition $U_t=1$ to the presentation of $X_R$ gives the open $U_t$ and the presentation of $X_{R[t^{-1}]}$: the generator for $a/t^n$ corresponds to $U_a\wedge U_t$. This is well-defined since equality of fractions, after multiplication by a power of the now-invertible $t$, makes the two membership propositions equivalent. More explicitly, $U_t=1$ implies $U_{t^kz}=U_z$. If $t^kz=0$, this gives $U_z=0$. If $x-y$ is killed by a power of $t$, then $U_{x-y}=U_{y-x}=0$ (since $U_{-1}=1$), and the additive inequalities for $x=y+(x-y)$ and $y=x+(y-x)$ give $U_x=U_y$. A zero element in the localized ring has false membership, multiplication gives intersections, and the additive relation follows by clearing denominators. The reverse assignment on $a\in R$ proves that these maps are inverse. Thus **$X_{R[t^{-1}]}\cong U_t$**. If $U_t\subseteq U_r$, then in this localized theory $U_r=1$. Apply the quotient argument above, with the second generator $0$, to conclude $1\in(r)$ in $R[t^{-1}]$. Therefore $r$ is invertible there, and the [universal property](../../../../../universal-property.md) of [localization](../../../../../localization-of-a-ring.md) gives the restriction $R[r^{-1}]\to R[t^{-1}]$. These restrictions compose uniquely.

It remains to glue, and the allowed basis criterion reduces this to a whole-locale cover $U_r\vee U_s=1$. Let $\alpha\in R[r^{-1}]$ and $\beta\in R[s^{-1}]$ have equal restrictions to $R[(rs)^{-1}]$. Choose a common initial exponent $n$, writing $\alpha=a/r^n$, $\beta=b/s^n$. Equality on the overlap supplies $k\geq0$ with

$$
(rs)^k(s^na-r^nb)=0.
$$

Set $N=n+k$, $A=r^ka$ and $B=s^kb$. Then

$$
\alpha=A/r^N,\qquad\beta=B/s^N,\qquad s^NA=r^NB
$$

with the last equality in $R$ itself. This clearing step is necessary when the [commutative ring](../../../../../commutative-ring.md) has [zero divisors](../../../../../zero-divisor.md).

Since $(r,s)=R$, also $(r^N,s^N)=R$. Choose $\lambda r+\mu s=1$. For $N\geq1$, expand $(\lambda r+\mu s)^{2N-1}=1$; each term contains either $r^N$ or $s^N$, producing $C,D\in R$ with $Cr^N+Ds^N=1$. For $N=0$ choose $C=1,D=0$. Define

$$
\boxed{t=CA+DB.}
$$

In $R[r^{-1}]$,

$$
t-A/r^N=D\,(r^NB-s^NA)/r^N=0,
$$

and similarly in $R[s^{-1}]$,

$$
t-B/s^N=C\,(s^NA-r^NB)/s^N=0.
$$

Thus $t$ glues the matching pair. If $t'$ is another gluing, some $r^p$ and $s^q$ annihilate $t-t'$. The same binomial argument gives $(r^p,s^q)=R$, so $t-t'=0$. This proves uniqueness without cancellation or a domain assumption.

The [exactness of the unit-ideal localization Čech complex](../../../../../exactness-of-the-unit-ideal-localization-cech-complex.md) proves the [sheaf](../../../../../sheaf-mathematics.md) axiom for the required basic covers, and hence the assignment with its restrictions defines **a [sheaf of rings](../../../../../sheaf-of-rings.md) $\widetilde R$ with $\widetilde R(U_r)=R[r^{-1}]$**. On the empty basic open, [localization](../../../../../localization-of-a-ring.md) is the [zero ring](../../../../../zero-ring.md), whose underlying set has one section, as required. The construction and proof remain valid for the [zero ring](../../../../../zero-ring.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
