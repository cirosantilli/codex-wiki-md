<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We prove the required duality pairing explicitly. This also identifies the word “canonical” in the final conclusion: the isomorphism will be the intrinsic [residue trace on a smooth projective curve](../../../../../residue-trace-on-a-smooth-projective-curve.md), not a choice of basis for a one-dimensional vector space.

Begin on the [projective line](../../../../../projective-line.md). With $s=t^{-1}$, the equation $ds=-t^{-2}dt$ identifies its [sheaf of Kähler differentials over a field](../../../../../sheaf-of-kahler-differentials-over-a-field.md) with $\mathcal O(-2)$. The Laurent description in Question 3 pairs $H^1(\mathcal O(a))$ with $H^0(\mathcal O(-a-2))$ by multiplication and extraction of the coefficient of $t^{-1}dt$. For $a\le-2$ the respective bases are

$$
t^re\quad(a<r<0),\qquad t^je^\vee dt\quad(0\le j\le-a-2),
$$

and their pairing matrix has entries

$$
\operatorname{res}_{t=0}(t^{r+j}dt)=
\begin{cases}1,&r+j=-1,\\0,&r+j\ne-1.\end{cases}
$$

This is an invertible antidiagonal matrix. For $a\ge-1$ both spaces vanish. The coefficient extraction is well defined on the [Čech cohomology](../../../../../cech-cohomology.md) quotient: a differential regular on the first chart has no $t^{-1}dt$ term, and one regular on the second chart is a sum of terms $t^{-2-j}dt$ with $j\ge0$, also with no such term.

To extend this calculation to every [vector bundle](../../../../../vector-bundle.md) $E$ on the [projective line](../../../../../projective-line.md), we give the splitting argument. Every [line bundle](../../../../../line-bundle.md) on $\mathbb P^1$ is $\mathcal O(a)$: choose a nonzero rational section to obtain a divisor, and use the divisors of $t-c$ to move each finite point to infinity. The denominator-clearing argument in Question 4 makes both $E(n)$ and $E^\vee(n)$ globally generated for large $n$. The first assertion ensures $H^0(E(-a))\ne0$ for some integer $a$; the second gives an embedding $E\hookrightarrow\mathcal O(n)^{\oplus r}$, so this is impossible for $a>n$. Choose the largest such integer $a$.

A nonzero section gives $\mathcal O(a)\to E$. Saturating its image gives a [line subbundle](../../../../../line-subbundle.md); if it were strictly larger, it would be $\mathcal O(a+d)$ for a positive integer $d$, recording the section's zeros, contrary to maximality. Thus the quotient $F$ is a [vector bundle](../../../../../vector-bundle.md). Induct on rank and write $F=\bigoplus_j\mathcal O(b_j)$. Twist the sequence by $-a-1$. Since $H^0(E(-a-1))=0$ and $H^1(\mathcal O(-1))=0$, exactness forces $H^0(F(-a-1))=0$, whence every $b_j\le a$. Local lifts of a quotient summand differ on overlaps by a [Čech cocycle](../../../../../cech-cocycle-condition.md) in $\mathcal O(a-b_j)$. But $H^1(\mathcal O(a-b_j))=0$ by Question 3. Adjusting the lifts by a coboundary makes them glue, splitting the sequence. This proves the [Birkhoff–Grothendieck theorem](../../../../../birkhoff-grothendieck-theorem.md) here. The direct-sum Laurent calculation consequently proves the perfect pairing

$$
H^1(\mathbb P^1,E)\times H^0(\mathbb P^1,E^\vee\otimes\Omega^1_{\mathbb P^1})\longrightarrow k.
$$

Although a splitting proves nondegeneracy, the pairing itself uses only evaluation followed by the coefficient trace on $H^1(\Omega^1_{\mathbb P^1})$, so does not depend on that splitting. This is [residue duality on the projective line](../../../../../residue-duality-on-the-projective-line.md).

Now choose a rational function $t$ on $C$ with $dt\ne0$. Such a choice is available over the perfect field $k$: a [local parameter](../../../../../local-parameter-on-a-smooth-algebraic-curve.md) at a smooth point has nonzero differential in the rank-one [sheaf of Kähler differentials over a field](../../../../../sheaf-of-kahler-differentials-over-a-field.md). Since $dt$ spans the differentials of $k(C)/k$, the extension $k(C)/k(t)$ has zero relative differentials and is separable. Question 1 gives a finite generically separable morphism $\pi:C\to\mathbb P^1$. It is flat: locally its finite module over a [discrete valuation ring](../../../../../discrete-valuation-ring.md) is torsion-free, hence free. For the [invertible sheaf](../../../../../line-bundle.md) $\mathcal M$, its pushforward $E=\pi_*\mathcal M$ is therefore a [vector bundle](../../../../../vector-bundle.md).

We next prove the differential-valued dual identification needed to transfer the pairing. At a point of the base, complete the local rings. Each branch is of the form

$$
A=k[[s]]\subset B=k[[u]],\qquad s=f(u),\qquad f'(u)\ne0.
$$

If $e$ is the order of $f$, formal division writes $B=A[u]$ with basis $1,u,\ldots,u^{e-1}$ and a monic degree-$e$ equation $P(u)=0$. In particular this argument does not assume tame ramification or the special equation $s=u^e$. For a polynomial $g$ the elementary interpolation identity is

$$
\operatorname{Tr}_{\operatorname{Frac}B/\operatorname{Frac}A}
\left(\frac{g(u)}{P'(u)}\right)
=[T^{e-1}]\big(g(T)\bmod P(T)\big).
$$

To see it, pass to a field containing the distinct roots $u_i$ of $P$. Lagrange interpolation writes the remainder as $\sum_i g(u_i)P(T)/((T-u_i)P'(u_i))$. Comparison of its leading coefficient gives the identity, and descent returns it to the original field. The top-coefficient pairing on $A[T]/(P)$ is perfect: in the power basis its matrix has zero entries for $i+j<e-1$ and ones for $i+j=e-1$, so its determinant is a unit. It follows that the trace-dual fractional module is exactly $P'(u)^{-1}B$.

Formal division of $f(T)-s$ gives $f(T)-s=W(T,s)P(T,s)$ with $W$ a unit. Differentiate in $T$ and evaluate at $u$. This shows that $f'(u)$ and $P'(u)$ differ by a unit. Since $ds=f'(u)du$, we obtain

$$
\operatorname{Hom}_A(B,A)\otimes_A A\,ds
=f'(u)^{-1}B\,ds=B\,du.
$$

This is the [trace-dual module of a finite curve map](../../../../../trace-dual-module-of-a-finite-curve-map.md) identity. Its map sends a differential $\eta$ to the functional $b\mapsto\operatorname{Tr}(b\eta)$, where the trace of $h\,ds$ is $\operatorname{Tr}(h)\,ds$. For several branches take the direct sum of these maps. Completion is faithfully flat, so their being isomorphisms proves the corresponding isomorphism of the original local modules. A local trivialization of $\mathcal M$ now gives, compatibly on overlaps,

$$
\pi_*(\mathcal M^\vee\otimes\Omega^1_C)
\cong\mathcal H om_{\mathcal O_{\mathbb P^1}}(E,\Omega^1_{\mathbb P^1})
=E^\vee\otimes\Omega^1_{\mathbb P^1}.
$$

The inverse images of the two standard affine charts and their intersection are affine. As in Question 4, the [Čech cochain complexes](../../../../../cech-cochain-complex.md) identify $H^1(C,\mathcal M)$ with $H^1(\mathbb P^1,E)$. Global sections in the last display identify the other factor with $H^0(C,\mathcal M^\vee\otimes\Omega^1_C)$. Thus the perfect pairing already calculated on the [projective line](../../../../../projective-line.md) gives

$$
\boxed{H^1(C,\mathcal M)\cong
H^0(C,\mathcal M^\vee\otimes\Omega^1_C)^\vee.}
$$

In particular **the stated vanishing of global sections forces $H^1(C,\mathcal M)=0$.** The proof has established the relevant case of [Serre duality](../../../../../serre-duality.md), rather than invoked it as the requested argument.

To identify its intrinsic trace, use the [rational principal-parts resolution on an algebraic curve](../../../../../rational-principal-parts-resolution-on-an-algebraic-curve.md). The constant sheaf of rational sections and the sheaf of their finite-support principal parts are both [flasque sheaves](../../../../../flasque-sheaf.md). Consequently a class of $H^1(C,\mathcal M)$ is represented by finitely many rational principal parts $(m_P)$, modulo the family coming from one global rational section. For a global section $\eta$ of $\mathcal M^\vee\otimes\Omega^1_C$, evaluation gives the pairing

$$
\langle[m_P],\eta\rangle=\sum_P\operatorname{res}_P(m_P\eta).
$$

The [algebraic residue of a rational differential](../../../../../algebraic-residue-of-a-rational-differential.md) is its $u^{-1}du$ coefficient, independent of the [local parameter](../../../../../local-parameter-on-a-smooth-algebraic-curve.md). Adding a regular representative changes no residue. The local trace calculation above also gives

$$
\operatorname{res}_s\operatorname{Tr}(\omega)
=\sum_{P\mid s}\operatorname{res}_P(\omega).
$$

One can check this directly in the monogenic description: expand a differential in the basis $1,u,\ldots,u^{e-1}$, use the displayed interpolation formula for its trace, and extract the coefficient of $s^{-1}ds$. Formal division of $f(u)-s$ makes that coefficient exactly the coefficient of $u^{-1}du$; for a product of branch fields the trace is the sum. Thus the identity remains valid in positive characteristic, including wild ramification. On $\mathbb P^1$, partial fractions show that a rational differential's residues at finite points sum to the negative of its residue at infinity. Tracing to $\mathbb P^1$ therefore proves that the sum of residues of every global [rational differential](../../../../../rational-differential-on-an-algebraic-curve.md) on $C$ is zero. Adding a global rational section to $(m_P)$ consequently changes the pairing by zero. This defines the same pairing as the finite-pushforward calculation, intrinsically, without a chosen map to $\mathbb P^1$.

Finally take $\mathcal M=\Omega^1_C$. Its differential-valued dual is $\mathcal O_C$, and Question 4 proved $H^0(C,\mathcal O_C)=k$. Perfectness identifies $H^1(C,\Omega^1_C)$ with the dual of this space. Evaluation at the distinguished constant section $1$ gives

$$
\boxed{\operatorname{tr}_C:H^1(C,\Omega^1_C)\xrightarrow{\ \sim\ }k,\qquad
[\omega_P]\longmapsto\sum_P\operatorname{res}_P(\omega_P).}
$$

This [residue trace on a smooth projective curve](../../../../../residue-trace-on-a-smooth-projective-curve.md) uses neither a basis choice nor an auxiliary finite map. **It is the canonical isomorphism.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
