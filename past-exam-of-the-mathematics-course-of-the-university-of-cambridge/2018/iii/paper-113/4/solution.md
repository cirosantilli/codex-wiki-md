<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [resolution principle for sheaf cohomology](../../../../../resolution-principle-for-sheaf-cohomology.md) states that an [exact sequence](../../../../../exact-sequence.md)

$$
0\longrightarrow\mathcal F\longrightarrow\mathcal A^0\longrightarrow\mathcal A^1\longrightarrow\cdots
$$

with $H^q(X,\mathcal A^j)=0$ for every $q>0$ computes $H^i(X,\mathcal F)$ as the cohomology of $\Gamma(X,\mathcal A^\bullet)$. In particular one may use a [flasque resolution](../../../../../flasque-resolution.md).

An [affine morphism](../../../../../affine-morphism.md) $\phi:X\to Y$ is one for which the inverse image of every affine open subset of $Y$ is affine. We use [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md): a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) has zero higher [sheaf cohomology](../../../../../sheaf-cohomology.md) on an [affine variety](../../../../../affine-algebraic-set.md). Take a [flasque resolution](../../../../../flasque-resolution.md) $\mathcal F\to\mathcal I^\bullet$. Each [direct image sheaf](../../../../../direct-image-sheaf.md) $\phi_*\mathcal I^j$ is flasque, because restriction on $V\subseteq U\subseteq Y$ is restriction on $\phi^{-1}V\subseteq\phi^{-1}U$. On an affine open $U\subseteq Y$, the augmented complex of sections is

$$
0\longrightarrow\Gamma(\phi^{-1}U,\mathcal F)\longrightarrow\Gamma(\phi^{-1}U,\mathcal I^0)\longrightarrow\Gamma(\phi^{-1}U,\mathcal I^1)\longrightarrow\cdots.
$$

Its positive-degree cohomology vanishes by the affine theorem, and its degree-zero kernel is $\Gamma(\phi^{-1}U,\mathcal F)$. Checking exactness on this affine basis shows that $\phi_*\mathcal I^\bullet$ is a [flasque resolution](../../../../../flasque-resolution.md) of $\phi_*\mathcal F$. The global-section complexes are identical, proving [cohomology under an affine morphism](../../../../../cohomology-under-an-affine-morphism.md):

$$
\boxed{H^i(Y,\phi_*\mathcal F)\cong H^i(X,\mathcal F)\quad(i\geq0).}
$$

For [projective space](../../../../../projective-space-split.md), put $S=k[x_0,\ldots,x_n]$ with its usual grading and $U_i=\{x_i\ne0\}$. Construct the [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) by setting its sections on $U_i$ to be the degree-$m$ part $(S_{x_i})_m$, viewed as a module over $(S_{x_i})_0$. It is free of rank one with generator $x_i^m$, even when $m$ is negative. On overlaps the generators differ by the unit $(x_i/x_j)^m$, so these modules glue to a [line bundle](../../../../../line-bundle.md) $\mathcal O(m)$.

Assume first $n\geq1$. These local modules all embed in the graded fraction field, and agreement on overlaps identifies global sections with $\bigcap_i(S_{x_i})_m$. Since $S$ is a [unique factorization domain](../../../../../unique-factorization-domain.md) and at least two distinct variables occur, a reduced fraction belonging to every $S_{x_i}$ has no nonconstant denominator. Thus the intersection is $S_m$. Counting monomials by [stars and bars](../../../../../stars-and-bars-combinatorics.md) gives

$$
H^0(\mathbf P^n,\mathcal O(m))=S_m,\qquad
h^0_n(m)=\begin{cases}\binom{m+n}{n},&m\geq0,\\0,&m<0.\end{cases}
$$

Here $h^i_n(m)=\dim_kH^i(\mathbf P^n,\mathcal O(m))$. The printed formula needs the convention that a counting [binomial coefficient](../../../../../binomial-coefficient.md) is zero when its upper integer is smaller than its nonnegative lower integer; the generalized polynomial convention for negative upper integers would give incorrect dimensions. For $n=0$, every twist on the single point $\mathbf P^0$ is trivial, so $h^0_0(m)=1$ for every $m$ and its higher cohomology is zero. This case supplies the base of dimension induction; the displayed top-cohomology formula below is for $n\geq1$.

The standard $n+1$ affine opens have affine finite intersections. The [acyclic cover theorem](../../../../../leray-s-theorem.md) and affine vanishing identify [sheaf cohomology](../../../../../sheaf-cohomology.md) with a [Čech cochain complex](../../../../../cech-cochain-complex.md) ending in degree $n$. In particular $H^i(\mathbf P^n,\mathcal O(m))=0$ for $i>n$.

Let $H=\{x_n=0\}\cong\mathbf P^{n-1}$, with inclusion $i$. Multiplication by $x_n$ gives the [hyperplane exact sequence for twisting sheaves](../../../../../hyperplane-exact-sequence-for-twisting-sheaves.md)

$$
0\longrightarrow\mathcal O_{\mathbf P^n}(m-1)\xrightarrow{\,x_n\,}\mathcal O_{\mathbf P^n}(m)\longrightarrow i_*\mathcal O_H(m)\longrightarrow0.
$$

Exactness is checked in the local trivializations, where a hyperplane equation is a non-zero-divisor and the quotient is its restriction to $H$. Since a [closed immersion](../../../../../closed-immersion.md) is an [affine morphism](../../../../../affine-morphism.md), the first part identifies the cohomology of $i_*\mathcal O_H(m)$ with that on $H$.

For $n=1$, the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) and $H\cong\mathbf P^0$ give

$$
h^1_1(m-1)-h^1_1(m)=1-\bigl(h^0_1(m)-h^0_1(m-1)\bigr)
=\begin{cases}0,&m\geq0,\\1,&m<0.\end{cases}
$$

Starting from the given vanishing for sufficiently large $m$ and descending gives $h^1_1(m)=0$ for $m\geq-1$ and $h^1_1(m)=-m-1$ for $m\leq-2$.

Now let $n\geq2$, and assume the formulas in dimension $n-1$. Restriction

$$
H^0(\mathbf P^n,\mathcal O(m))\longrightarrow H^0(H,\mathcal O_H(m))
$$

is surjective for every $m$: for $m\geq0$ it is polynomial restriction, and for $m<0$ both groups are zero since $\dim H\geq1$. The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) therefore makes $H^1(\mathbf P^n,\mathcal O(m-1))\to H^1(\mathbf P^n,\mathcal O(m))$ injective. For $2\leq j<n$, dimension induction gives $H^{j-1}(H,\mathcal O_H(m))=0$, so the same sequence makes

$$
H^j(\mathbf P^n,\mathcal O(m-1))\longrightarrow H^j(\mathbf P^n,\mathcal O(m))
$$

injective. Composing these injections up to a sufficiently large twist, where the target is zero by the given hypothesis, proves $H^j(\mathbf P^n,\mathcal O(m))=0$ for every $m$ and $0<j<n$.

The remaining part of the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) is consequently

$$
0\longrightarrow H^{n-1}(H,\mathcal O_H(m))\longrightarrow H^n(\mathbf P^n,\mathcal O(m-1))\longrightarrow H^n(\mathbf P^n,\mathcal O(m))\longrightarrow0,
$$

where the last zero uses the affine-cover dimension bound on $H$. Hence $h^n_n(m-1)=h^n_n(m)+h^{n-1}_{n-1}(m)$. Using dimension induction and eventual vanishing, downward summation yields

$$
h^n_n(m)=\sum_{j=m+1}^{-n}\binom{-j-1}{n-1}=\binom{-m-1}{n}\quad(m\leq-n-1),
$$

by telescoping Pascal's identity; for $m\geq-n$ it is zero. Thus, without invoking [Serre duality](../../../../../serre-duality.md) in the induction,

$$
\boxed{
H^j(\mathbf P^n,\mathcal O(m))=0\ (j>0,\ j\ne n),\qquad
h^n_n(m)=\begin{cases}\binom{-m-1}{n},&m\leq-n-1,\\0,&m\geq-n.\end{cases}}
$$

Finally, the [canonical bundle of projective space](../../../../../canonical-bundle-of-projective-space.md) is $\omega_{\mathbf P^n}\cong\mathcal O(-n-1)$, obtained by taking determinants in the dual [Euler sequence](../../../../../euler-sequence.md). [Serre duality](../../../../../serre-duality.md) therefore predicts

$$
H^j(\mathbf P^n,\mathcal O(m))\cong H^{n-j}(\mathbf P^n,\mathcal O(-m-n-1))^*.
$$

It pairs the two computed extreme-degree dimensions and pairs zero intermediate groups with zero intermediate groups, exactly as required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 113](../../paper-113-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
