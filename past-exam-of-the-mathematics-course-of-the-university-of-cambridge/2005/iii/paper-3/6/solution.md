<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [kernel intersection theorem for Specht modules](../../../../../kernel-intersection-theorem-for-specht-modules.md) uses maps that move entries between adjacent rows. For $1\le i<\ell(\mu)$ and $0\le v<\mu_{i+1}$, let $\mu(i,v)$ replace the row lengths $(\mu_i,\mu_{i+1})$ by $(\mu_i+\mu_{i+1}-v,v)$, keeping every other length unchanged. This is allowed to be a composition rather than a decreasing [partition of an integer](../../../../../partition-of-an-integer.md), and a zero row can be omitted. For a [tabloid](../../../../../tabloid.md) with row sets $R_j$, define

$$
\psi_{i,v}:M^\mu\longrightarrow M^{\mu(i,v)}
$$

by summing over all $v$-subsets $B\subset R_{i+1}$: the new row $i+1$ is $B$, the new row $i$ is $R_i\cup(R_{i+1}\setminus B)$, and all other rows are unchanged. These are [module homomorphisms](../../../../../module-homomorphism.md), since relabelling commutes with choosing subsets. The theorem is

$$
\boxed{S^\mu=\bigcap_{i=1}^{\ell(\mu)-1}\,\bigcap_{v=0}^{\mu_{i+1}-1}\ker\psi_{i,v}.}
$$

It holds over every [field](../../../../../field.md). Column cancellation shows the inclusion of $S^\mu$ in each kernel; the full theorem identifies the common kernel with the [Specht module](../../../../../specht-module.md).

For completeness, the [semistandard homomorphism theorem](../../../../../semistandard-homomorphism-theorem.md) concerns a [partition of an integer](../../../../../partition-of-an-integer.md) $\lambda$, a composition $\alpha$, and fillings $T$ of shape $\lambda$ with $\alpha_j$ occurrences of $j$. Such a filling gives $\Theta_T:M^\lambda\to M^\alpha$: replace its labels by the numbered entries of an input tableau, and sum the output [tabloids](../../../../../tabloid.md) over distinct [permutations](../../../../../permutation.md) of the labels within each input row. Label $j$ assigns an entry to output row $j$. The use of distinct assignments avoids dividing by any factorial. Let $\widehat\Theta_T$ be its restriction to $S^\lambda$. The restrictions indexed by [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) are linearly independent. They form a basis of $\operatorname{Hom}_{FS_n}(S^\lambda,M^\alpha)$ when $p\ne2$, or when $\lambda$ is two-regular. In [characteristic two](../../../../../characteristic-two.md) for a two-singular shape they need not span; omitting this exception would make the statement incorrect.

We now prove the [invariant vector criterion for a Specht module](../../../../../invariant-vector-criterion-for-a-specht-module.md) directly from the first theorem. The group acts transitively on the [tabloid](../../../../../tabloid.md) basis of $M^\mu$, so any invariant vector has all coefficients equal. Thus $(M^\mu)^{S_n}=Fz_\mu$, where $z_\mu$ is the sum of all its [tabloids](../../../../../tabloid.md) and is nonzero over every [field](../../../../../field.md). Fix $i,v$, write $a=\mu_i$, $b=\mu_{i+1}$, and count preimages of one output [tabloid](../../../../../tabloid.md). The $v$ retained entries are prescribed; among the $a+b-v$ entries of the enlarged row, exactly $a$ must have come from its old row. Hence

$$
\psi_{i,v}(z_\mu)=\binom{a+b-v}{a}z_{\mu(i,v)}.
$$

The common-kernel criterion becomes

$$
z_\mu\in S^\mu\quad\Longleftrightarrow\quad
\binom{a+j}{j}\equiv0\pmod p\quad(1\le j\le b)
$$

for every adjacent pair, where $j=b-v$.

Suppose $p>0$, and let $t$ be least with $b<p^t$. If $a\equiv-1\pmod{p^t}$, its lowest $t$ base-$p$ digits are all $p-1$. For any $0<j<p^t$, adding $j$ to $a$ creates a carry at the lowest nonzero digit of $j$. At that position the digit of $a+j$ is smaller than the corresponding digit of $j$. [Lucas's theorem](../../../../../lucas-s-theorem.md) therefore gives $\binom{a+j}{j}\equiv0$. Conversely, if one of the first $t$ digits $a_d$ is not $p-1$, take $j=p^d$. Minimality of $t$ gives $p^d\le b$, while addition at that digit creates no carry. Lucas then yields

$$
\binom{a+p^d}{p^d}\equiv a_d+1\not\equiv0\pmod p.
$$

This proves the claimed equivalence, and therefore

$$
\boxed{(S^\mu)^{S_n}\ne0\iff
\mu_i\equiv-1\pmod{p^{t_i}}\text{ for every }i,
\quad t_i=\min\{t\ge0:\mu_{i+1}<p^t\}.}
$$

The invariant space, when present, is one-dimensional. At the last row put $\mu_{i+1}=0$; then $t_i=0$ and the condition is vacuous. This congruence formulation is for positive characteristic. In [characteristic zero](../../../../../characteristic-zero.md) the positive [binomial coefficients](../../../../../binomial-coefficient.md) cannot vanish, so an invariant vector exists precisely for the one-row shape $(n)$.

Finally suppose $\mu$ is regular. It has a unique simple [head](../../../../../head-of-a-module.md) $D^\mu$, by Question 1. The given sign-twisted duality of [Specht modules](../../../../../specht-module.md) implies

$$
\operatorname{Hom}_{S_n}(S^\mu,\operatorname{sgn})
\cong\operatorname{Hom}_{S_n}((S^{\mu'})^*,F)
\cong\operatorname{Hom}_{S_n}(F,S^{\mu'}).
$$

Thus $D^\mu$ is sign exactly when the conjugate shape $\mu'$ satisfies the invariant congruences.

Here is an explicit solution of those congruences under regularity. Write the positive column heights of $\mu$ as $a_1\ge\cdots\ge a_l>0$, so $\mu'=(a_1,\ldots,a_l)$. Regularity says $a_i-a_{i+1}<p$, including $a_l-a_{l+1}=a_l<p$, because this difference counts rows of length $i$. Starting with $0<a_l<p$, the congruence for its preceding row forces $a_{l-1}\equiv-1\pmod p$. Since $a_l\le a_{l-1}<a_l+p\le2p-1$, the only possibility is $a_{l-1}=p-1$. Repeating upwards forces every earlier height to be $p-1$. Consequently

$$
\mu'=((p-1)^q,r),\qquad n=q(p-1)+r,\quad0\le r<p-1,
$$

where a zero final part is omitted. Conversely this shape satisfies every invariant congruence, so its conjugate is the desired [regular label of the modular sign representation](../../../../../regular-label-of-the-modular-sign-representation.md):

$$
\boxed{\mu=((q+1)^r,q^{p-1-r}),\qquad n=q(p-1)+r,quad0\le r<p-1.}
$$

Zero parts are omitted. For $p=2$ this is $(n)$, as it should be because sign is trivial. In [characteristic zero](../../../../../characteristic-zero.md) the answer is $(1^n)$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
