<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $[m]=\{1,\ldots,m\}$. A [combinatorial line](../../../../../combinatorial-line.md) in $[m]^n$ has one nonempty active set of coordinates, all carrying the same variable letter, with every other coordinate fixed. The [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) states that **for every finite alphabet size $m$ and number of colours $k$, some $n$ makes every $k$-[finite colouring](../../../../../finite-coloring.md) of $[m]^n$ contain a [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md)**.

Here is a complete proof through the [alphabet insensitivity lemma](../../../../../alphabet-insensitivity-lemma.md). A $d$-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md) is obtained from $d$ pairwise disjoint nonempty coordinate blocks, one independently variable letter on each block, and fixed letters elsewhere. For two distinct letters $a,b$, a colouring restricted to such a [combinatorial subspace](../../../../../combinatorial-subspace.md) is $(a,b)$-insensitive if switching $a$ and $b$ in any of its parameter coordinates leaves the colour unchanged, with all other letters and coordinates arbitrary.

We first prove that any desired dimension $d$ admits such an insensitive [combinatorial subspace](../../../../../combinatorial-subspace.md), using only the [pigeonhole principle](../../../../../pigeonhole-principle.md). Define finite bounds recursively by

$$
I(m,k,0)=0,\qquad N=I(m,k^m,d-1),\qquad L=k^{m^N},\qquad I(m,k,d)=L+N.
$$

Split the ambient coordinates into a prefix of length $L$ and a suffix of length $N$. For $0\leq j\leq L$, let the prefix $p_j$ consist of $j$ copies of $b$ followed by $L-j$ copies of $a$. Give it the entire colour profile

$$
\big(c(p_j u):u\in[m]^N\big).
$$

There are at most $k^{m^N}=L$ such profiles, but $L+1$ prefixes. Hence two prefixes $p_s,p_t$, $s<t$, have the same profile. Replace their differing coordinates $s+1,\ldots,t$ by one variable letter, obtaining a prefix word $v(x)$ with $v(a)=p_s$ and $v(b)=p_t$. Then $c(v(a)u)=c(v(b)u)$ for every suffix $u$.

Colour the suffixes by the vector

$$
c'(u)=\big(c(v(x)u):x\in[m]\big),
$$

which has at most $k^m$ colours. By the dimension-$d-1$ induction hypothesis, there is a $(d-1)$-dimensional suffix [combinatorial subspace](../../../../../combinatorial-subspace.md) on which this vector colouring is $(a,b)$-insensitive. Combining it with the variable block of $v$ gives dimension $d$. Switching the first parameter between $a,b$ preserves colour by the equal prefix profiles; switching any other parameter preserves every entry of $c'$ by induction. This proves the [alphabet insensitivity lemma](../../../../../alphabet-insensitivity-lemma.md), including $d=1$, where the suffix is empty.

Now induct on $m$ to prove the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md). For $m=1$, any one-variable word gives a one-point [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md). Suppose the theorem holds for $m-1$, and let $d$ be a sufficient dimension for $k$ colours on $[m-1]^d$. The lemma supplies a $d$-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md) insensitive to $(m-1,m)$. Restrict its parameter colouring to $[m-1]^d$. By the alphabet induction hypothesis it contains a [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md). Its $m$th point has the same colour as its $(m-1)$st point: switch the active parameter coordinates from $m-1$ to $m$, one at a time. Therefore the full line over $[m]$ is [monochromatic](../../../../../monochromatic-set.md). Its actual active coordinate set is the nonempty union of the active parameter blocks. This completes both inductions.

To deduce the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md), choose the dimension $n$ for alphabet size $m$ and pull back a colouring of a sufficiently long integer interval along

$$
\Phi(w_1,\ldots,w_n)=\sum_{j=1}^n w_jm^{j-1}.
$$

All images lie in $[N]$ for $N=m\sum_{j=1}^n m^{j-1}$. A [combinatorial line](../../../../../combinatorial-line.md) with active coordinates $D$ maps to

$$
a+d,\ a+2d,\ldots,a+md,\qquad d=\sum_{j\in D}m^{j-1}>0,
$$

where $a$ is the contribution of the fixed coordinates. Thus **every finite colouring of the positive integers contains [monochromatic](../../../../../monochromatic-set.md) [arithmetic progressions](../../../../../arithmetic-progression.md) of every finite length**. The argument also provides the finite-interval version. Length one is immediate.

The [Strengthened Van der Waerden theorem](../../../../../strengthened-van-der-waerden-theorem.md) requires the common difference itself to have the progression's colour. We prove a useful stronger, scaled version, the [Brauer progression theorem](../../../../../brauer-progression-theorem.md): for every $k,t,\ell\geq1$, a finite bound $B(k,t,\ell)$ guarantees a [monochromatic](../../../../../monochromatic-set.md) set

$$
\boxed{\{td,a,a+d,\ldots,a+(\ell-1)d\},\qquad a,d>0.}
$$

The desired strengthening is $t=1$. For $\ell=1$ choose $a=t,d=1$; for one colour any interval covering the displayed configuration suffices. For the induction on $k$, assume $M=B(k-1,t,\ell)$ and $\ell\geq2$. Put $L=(\ell-1)M+1$, let $W$ be a [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) bound for $k$ colours and length $L$, and take $B(k,t,\ell)=tMW$. Inside $[W]$, obtain a one-colour progression $a+j\delta$ for $0\leq j<L$, of colour $c$.

All numbers $tj\delta$, $1\leq j\leq M$, lie in the larger interval because $\delta\leq W$. If one has colour $c$, then the subsequence $a,a+j\delta,\ldots,a+(\ell-1)j\delta$, together with $tj\delta$, is the desired configuration with $d=j\delta$. Otherwise the colouring $j\mapsto c(t\delta j)$ of $[M]$ uses at most $k-1$ colours. Apply the induction hypothesis to obtain a one-colour configuration $\{te,b,b+e,\ldots,b+(\ell-1)e\}$ there. Multiplication by $t\delta$ gives common difference $d=t\delta e$ and distinguished point $td=t^2\delta e$, all of the same original colour. This proves the scaled theorem using only the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md).

**The fixed-active-size strengthening is false.** It already fails for $m=k=2$. For any proposed positive $n,d$, if $d>n$ there is no eligible line. Otherwise colour a word by

$$
\boxed{c(w)=\left\lfloor\frac{\#\{j:w_j=2\}}d\right\rfloor\pmod2.}
$$

The two points of a line with exactly $d$ active coordinates have counts $q$ and $q+d$ of the letter $2$. Their quotient floors differ by exactly one, so their colours differ. This [fixed-active-size obstruction for combinatorial lines](../../../../../fixed-active-size-obstruction-for-combinatorial-lines.md) is valid for every proposed $n,d$. The colouring may depend on $d$, since the assertion chooses $n,d$ before demanding the conclusion for every colouring.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
