<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $S=k[X_0,\ldots,X_n]$ with its usual grading, and put $S(m)_d=S_{m+d}$. Define the [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) by

$$
\mathcal O_{\mathbb P^n}(m)=\widetilde{S(m)}.
$$

More explicitly, on $U_i=D_+(X_i)$ its sections are the homogeneous degree-$m$ part of $S_{X_i}$. They are a free rank-one [module](../../../../../module-mathematics.md) over $(S_{X_i})_0=k[X_j/X_i:j\ne i]$, with generator $e_i=X_i^m$. These generators make sense for every integer $m$, since $X_i$ is invertible on this chart. Their transition rule is

$$
e_i=(X_i/X_j)^m e_j.
$$

The ratios are regular units on overlaps and satisfy the cocycle identity, so they glue to an [invertible sheaf](../../../../../line-bundle.md). In particular $\mathcal O(m)\otimes\mathcal O(r)\cong\mathcal O(m+r)$.

For $n\ge1$, a [global section](../../../../../global-section.md) is a compatible homogeneous degree-$m$ rational expression lying in every $S_{X_i}$. Inside the [fraction field](../../../../../field-of-fractions.md) of $S$,

$$
\bigcap_{i=0}^nS_{X_i}=S.
$$

To justify this, write a fraction in lowest terms in the [unique factorization domain](../../../../../unique-factorization-domain.md) $S$. Membership in $S_{X_i}$ forces every irreducible divisor of its denominator to be associated with $X_i$. Since there are at least two nonassociated variables, the denominator must be a unit. Therefore

$$
H^0(\mathbb P^n,\mathcal O(m))=
\begin{cases}
S_m,&m\ge0,\\
0,&m<0,
\end{cases}
\qquad(n\ge1).
$$

The degree-$m$ [monomials](../../../../../monomial.md) are indexed by nonnegative integers $a_0,\ldots,a_n$ with sum $m$. The [stars and bars](../../../../../stars-and-bars-combinatorics.md) count gives

$$
\boxed{h^0(\mathcal O_{\mathbb P^n}(m))=
\begin{cases}
\binom{m+n}{n},&m\ge0,\\
0,&m<0,
\end{cases}\qquad(n\ge1).}
$$

Here and below, an all-integer binomial shorthand must use the counting convention $\binom{a}{n}=0$ when $a<n$, including negative $a$. The polynomial extension of binomial coefficients to negative upper arguments does not give the stated dimensions. In dimension zero, $\mathbb P^0$ is one point and every $\mathcal O_{\mathbb P^0}(m)$ is trivial, so its space of [global sections](../../../../../global-section.md) is $k$ for every $m$; this case is treated separately.

For a closed inclusion $i:H\hookrightarrow\mathbb P^n$, [direct image sheaf](../../../../../direct-image-sheaf.md) formation is exact: its stalk is the original stalk at a point of $H$ and zero outside $H$. It preserves [flabby sheaves](../../../../../flasque-sheaf.md), since restrictions on the target are restrictions between the corresponding open subsets of $H$. Push forward a [flasque resolution](../../../../../flasque-resolution.md) of $\mathcal F$; exactness gives a [flasque resolution](../../../../../flasque-resolution.md) of $i_*\mathcal F$, and its complex of [global sections](../../../../../global-section.md) is the original one because

$$
\Gamma(\mathbb P^n,i_*\mathcal I^j)=\Gamma(H,\mathcal I^j).
$$

Taking cohomology of these identical complexes proves [sheaf cohomology under a closed inclusion](../../../../../sheaf-cohomology-under-a-closed-inclusion.md):

$$
\boxed{H^r(H,\mathcal F)\cong H^r(\mathbb P^n,i_*\mathcal F)\quad(r\ge0).}
$$

This argument applies even without quasi-coherence.

We derive the remaining [sheaf cohomology](../../../../../sheaf-cohomology.md) dimensions using the given eventual vanishing, the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md), and induction on dimension. Multiplication by the linear equation of a [hyperplane](../../../../../hyperplane.md) $H\cong\mathbb P^{n-1}$ gives the [hyperplane exact sequence for twisting sheaves](../../../../../hyperplane-exact-sequence-for-twisting-sheaves.md)

$$
0\longrightarrow\mathcal O_{\mathbb P^n}(m-1)
\longrightarrow\mathcal O_{\mathbb P^n}(m)
\longrightarrow i_*\mathcal O_H(m)\longrightarrow0.
$$

Exactness can be checked in each chart by quotienting its [polynomial ring](../../../../../polynomial-ring.md) by the equation of $H$; multiplication is [injective](../../../../../injective-function.md) because that equation is a [non-zero-divisor](../../../../../non-zero-divisor.md). We use the closed-inclusion cohomology identification to replace the cohomology of the final [sheaf](../../../../../sheaf-mathematics.md) by that on $H$.

The dimension-zero base is a point, whose global-section functor is exact. Thus all its higher [sheaf cohomology](../../../../../sheaf-cohomology.md) is zero. For $n=1$, the relevant [long exact sequence](../../../../../long-exact-sequence.md) is

$$
0\to H^0(\mathcal O(m-1))\to H^0(\mathcal O(m))
\to k\to H^1(\mathcal O(m-1))\to H^1(\mathcal O(m))\to0.
$$

When $m\ge0$, restriction of [homogeneous polynomials](../../../../../homogeneous-polynomial.md) to the hyperplane point is [surjective](../../../../../surjective-function.md): after choosing that point as $[1:0]$, the section $X_0^m$ restricts to a generator. Therefore the consecutive $H^1$ groups are isomorphic for $m\ge0$. The given vanishing for large $m$ propagates down to $m=-1$. For $m<0$, both displayed $H^0$ groups are zero, and the sequence becomes

$$
0\to k\to H^1(\mathcal O(m-1))\to H^1(\mathcal O(m))\to0.
$$

Starting with $H^1(\mathcal O(-1))=0$, induction downward gives $h^1(\mathcal O(m))=-m-1$ for $m\le-2$. For degrees $i>1$, the point contributes no cohomology to the exact sequence, so consecutive $H^i$ groups are isomorphic for every $m$; the given eventual vanishing makes them all zero. Hence the complete positive-degree formula holds for $\mathbb P^1$.

Now let $n\ge2$ and assume the formulas for $H\cong\mathbb P^{n-1}$. For every $m$, the restriction

$$
H^0(\mathbb P^n,\mathcal O(m))\to H^0(H,\mathcal O_H(m))
$$

is [surjective](../../../../../surjective-function.md): for $m\ge0$ extend a polynomial in the hyperplane coordinates to the same polynomial on $\mathbb P^n$, and for $m<0$ both groups vanish because $H$ has positive dimension. Consequently the exact sequence gives an [injection](../../../../../injective-function.md)

$$
H^1(\mathbb P^n,\mathcal O(m-1))
\hookrightarrow H^1(\mathbb P^n,\mathcal O(m)).
$$

For $2\le i\le n-1$, the induction hypothesis says $H^{i-1}(H,\mathcal O_H(m))=0$, and gives the same [injection](../../../../../injective-function.md) in degree $i$. For each fixed $m$, composing finitely many [injections](../../../../../injective-function.md) reaches a sufficiently large twist, whose higher cohomology is zero by the given hypothesis. Therefore

$$
H^i(\mathbb P^n,\mathcal O(m))=0
\quad(0<i<n,\ \text{every }m).
$$

For $i>n$, the two neighbouring hyperplane groups $H^{i-1}(H,\mathcal O_H(m))$ and $H^i(H,\mathcal O_H(m))$ are zero by induction. Consecutive $H^i$ groups on $\mathbb P^n$ are then isomorphic, and eventual vanishing again makes them zero. This derives vanishing above the dimension too, without needing a special projective-space cohomology theorem.

For top cohomology the exact sequence now reduces to

$$
0\to H^{n-1}(H,\mathcal O_H(m))
\to H^n(\mathbb P^n,\mathcal O(m-1))
\to H^n(\mathbb P^n,\mathcal O(m))\to0.
$$

Write $b_n(m)=h^n(\mathcal O_{\mathbb P^n}(m))$. The induction hypothesis and eventual vanishing give the recurrence

$$
b_n(m-1)=b_n(m)+b_{n-1}(m),\qquad
b_{n-1}(m)=
\begin{cases}
\binom{-m-1}{n-1},&m\le-n,\\
0,&m\ge-n+1.
\end{cases}
$$

Consecutive top groups agree for $m\ge-n+1$, so descending from a large twist gives $b_n(m)=0$ for $m\ge-n$. Below this range, iterating the recurrence gives a finite sum:

$$
b_n(m)=\sum_{j=m+1}^{-n}\binom{-j-1}{n-1}
=\sum_{\ell=n-1}^{-m-2}\binom{\ell}{n-1}
=\binom{-m-1}{n}
\qquad(m\le-n-1).
$$

The last equality follows by summing [Pascal's identity](../../../../../pascal-s-rule.md). These short exact sequences also prove that every group whose dimension is being counted is finite-dimensional. Thus, for $n\ge1$,

$$
\boxed{
h^i(\mathcal O_{\mathbb P^n}(m))=0\quad(0<i\ne n),\qquad
h^n(\mathcal O_{\mathbb P^n}(m))=
\begin{cases}
\binom{-m-1}{n},&m\le-n-1,\\
0,&m\ge-n.
\end{cases}}
$$

With the stated counting convention, the latter is the requested single binomial formula. The base $\mathbb P^0$ has $h^0=1$ for all twists and no higher cohomology; it is not governed by the negative-twist $H^0$ rule for positive-dimensional projective space.

Finally calculate the [canonical line bundle of a smooth variety](../../../../../canonical-line-bundle-of-a-smooth-variety.md) from its transition functions. On $U_0$ write $t_j=X_j/X_0$ for $1\le j\le n$. On $U_i$, $i>0$, take the coordinates $u_j=X_j/X_i$ in increasing order of $j\ne i$. Thus

$$
u_0=t_i^{-1},\qquad u_j=t_j/t_i\quad(j\ne0,i).
$$

In their wedge product, $du_0=-t_i^{-2}\,dt_i$ and  
$du_j=t_i^{-1}dt_j-t_jt_i^{-2}dt_i$. Every term involving a second $dt_i$ vanishes, so reordering the remaining differentials gives

$$
\bigwedge_{j\ne i}du_j
=(-1)^i t_i^{-(n+1)}\,dt_1\wedge\cdots\wedge dt_n.
$$

This computation is valid in every characteristic. Multiply the ordered local generator on $U_i$ by $(-1)^i$. The resulting generators $\eta_i$ satisfy $\eta_i=(X_i/X_0)^{-n-1}\eta_0$ on $U_i\cap U_0$, and hence the corresponding transition rule on every overlap. They are exactly the transitions of $\mathcal O(-n-1)$. Therefore the [canonical bundle of projective space](../../../../../canonical-bundle-of-projective-space.md) is

$$
\boxed{\omega_{\mathbb P^n}\cong\mathcal O_{\mathbb P^n}(-n-1).}
$$

For a [line bundle](../../../../../line-bundle.md), [Serre duality](../../../../../serre-duality.md) states

$$
H^i(\mathbb P^n,\mathcal O(m))^*
\cong H^{n-i}(\mathbb P^n,\mathcal O(-m-n-1)).
$$

The intermediate groups on both sides vanish. In the two outer degrees, the top group at twist $m$ has the same dimension as the global-section group at twist $-m-n-1$:

$$
h^n(\mathcal O(m))=h^0(\mathcal O(-m-n-1)).
$$

The polynomial degree on the right is nonnegative precisely when $m\le-n-1$, and its dimension is $\binom{-m-1}{n}$. Interchanging $m$ and $-m-n-1$ checks the other outer degree. On $\mathbb P^0$ both sides are one-dimensional. Thus all the formulas are consistent with [Serre duality](../../../../../serre-duality.md), which was used only for this final consistency check, not to prove the cohomology formulas.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
