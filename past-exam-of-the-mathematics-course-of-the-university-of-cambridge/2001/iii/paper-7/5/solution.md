<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $K=\sigma(T)$ for a bounded [normal operator](../../../../../normal-operator.md) on a nonzero complex [Hilbert space](../../../../../hilbert-space-split.md). The zero Hilbert space has the trivial calculus. Take the [inner product](../../../../../inner-product.md) linear in its first argument. The [continuous functional calculus](../../../../../continuous-functional-calculus.md) is an isometric [unital](../../../../../unital-algebra.md) star-representation $\pi:C(K)\to\mathcal B(H)$ with $\pi(z)=T$. The [Borel calculus](../../../../../borel-functional-calculus-for-a-normal-operator.md) will act on $B_b(K)$, the algebra of actual bounded [Borel measurable functions](../../../../../borel-measurable-function.md). A quotient by null functions is introduced only after specifying the spectral measure; there is no preferred scalar measure such as plane area on $K$.

Here is a construction that also covers a nonseparable [Hilbert space](../../../../../hilbert-space-split.md). For $v\in H$, the positive functional $f\mapsto\langle\pi(f)v,v\rangle$ has a finite [regular Borel measure](../../../../../regular-borel-measure.md) $\mu_v$ by the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md). On [continuous functions](../../../../../continuous-function.md),

$$
\|\pi(f)v\|^2=\int_K|f|^2\,d\mu_v.
$$

[Continuous functions](../../../../../continuous-function.md) are dense in $L^2(K,\mu_v)$. Hence $f\mapsto\pi(f)v$ extends to a unitary map from that space onto $H_v=\overline{\pi(C(K))v}$. This subspace reduces $T$ and $T^*$, which correspond to multiplication by $z$ and $\overline z$. Decompose $H$ as an [orthogonal direct sum](../../../../../orthogonal-direct-sum.md) of such cyclic [reducing subspaces](../../../../../reducing-subspace-of-a-hilbert-space-operator.md), using maximality: a nonzero vector in the remaining orthogonal complement would generate another summand. The family need not be countable. This is the [cyclic multiplication model for a normal operator](../../../../../cyclic-multiplication-model-for-a-normal-operator.md).

On each summand define $f(T)$ to be multiplication by $f$, for $f\in B_b(K)$, and take their bounded direct sum. It defines a [unital](../../../../../unital-algebra.md) star-homomorphism

$$
\Phi:B_b(K)\longrightarrow\mathcal B(H),\qquad\Phi(z)=T,\qquad\|\Phi(f)\|\le\|f\|_\infty.
$$

Thus $(fg)(T)=f(T)g(T)$, $\overline f(T)=f(T)^*$, and positivity of $f$ gives positivity of $f(T)$. The [continuous functional calculus](../../../../../continuous-functional-calculus.md) is recovered on $C(K)$.

Set $E(S)=\Phi(\mathbf1_S)$ for a Borel subset $S$ of $K$. Then $E(S)$ is an [orthogonal projection](../../../../../orthogonal-projection.md), $E(K)=I$, $E(S)E(R)=E(S\cap R)$, and disjoint countable unions add in the [strong operator topology](../../../../../strong-operator-topology.md). Indeed on every multiplication summand the indicators add pointwise, and the tail squared [norm](../../../../../norm.md) is the measure of a decreasing sequence of sets tending to the empty set. Thus $E$ is a [projection-valued measure](../../../../../projection-valued-measure.md), and

$$
\boxed{f(T)=\int_K f(z)\,dE(z),\qquad T=\int_Kz\,dE(z)}.
$$

For $v,w\in H$, polarization gives scalar measures $\mu_{v,w}(S)=\langle E(S)v,w\rangle$ satisfying $\langle f(T)v,w\rangle=\int f\,d\mu_{v,w}$. Regularity of these finite scalar measures and uniqueness in the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) make the [projection-valued measure](../../../../../projection-valued-measure.md) unique: its values on [continuous functions](../../../../../continuous-function.md) determine all scalar measures and hence every projection. This also makes the calculus independent of the chosen cyclic decomposition.

The correct convergence assertion is bounded pointwise convergence in the [strong operator topology](../../../../../strong-operator-topology.md). If $f_n\to f$ pointwise and $\sup_n\|f_n\|_\infty<\infty$, then

$$
\|(f_n(T)-f(T))v\|^2=\int_K|f_n-f|^2\,d\mu_v\longrightarrow0
$$

by the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md). This need not be convergence in [operator norm](../../../../../operator-norm.md). For multiplication by $t$ on $L^2[0,1]$, the functions $\mathbf1_{[0,1/n]}$ converge pointwise to $\mathbf1_{\{0\}}$, their operators converge strongly to zero, but their operator norms are all one.

A [Borel measurable function](../../../../../borel-measurable-function.md) can vanish spectrally without vanishing pointwise. Precisely, $f(T)=0$ if and only if $E(\{|f|>\varepsilon\})=0$ for every $\varepsilon>0$, and

$$
\|f(T)\|=\inf\{C\ge0:E(\{|f|>C\})=0\}.
$$

The upper norm bound follows by integrating $|f|^2$ against vector measures; a unit vector in any nonzero projection $E(\{|f|>C\})$ gives $\|f(T)\|\ge C$. The induced map on the quotient by these spectral-null [Borel measurable functions](../../../../../borel-measurable-function.md) is isometric. Every nonempty relatively [open](../../../../../open-set.md) subset of $K$ has nonzero spectral projection, since otherwise a nonzero [continuous function](../../../../../continuous-function.md) supported there would contradict faithfulness of the [continuous functional calculus](../../../../../continuous-functional-calculus.md). This full support gives the usual continuous [spectral mapping theorem](../../../../../spectral-mapping-theorem.md), but for a [Borel measurable function](../../../../../borel-measurable-function.md) the exact statement is instead

$$
\boxed{\sigma(f(T))=\{\lambda:E(\{|f-\lambda|<\varepsilon\})\ne0\text{ for every }\varepsilon>0\}}.
$$

If an indicated neighborhood has zero projection, define a bounded reciprocal of $f-\lambda$ off it and zero on it; the calculus supplies an inverse. Conversely unit vectors in the nonzero projections for arbitrarily small neighborhoods give $\|(f(T)-\lambda)v\|$ arbitrarily small, contradicting invertibility. This is [spectral essential range in Borel functional calculus](../../../../../spectral-essential-range-in-borel-functional-calculus.md). For example $\mathbf1_{\{0\}}(T)=0$ in the multiplication model on $[0,1]$, although the pointwise range of that function is $\{0,1\}$.

Spectral projections provide [reducing subspaces](../../../../../reducing-subspace-of-a-hilbert-space-operator.md), and $E(\{\lambda\})H=\ker(T-\lambda I)$: the squared [norm](../../../../../norm.md) of $(T-\lambda)v$ is $\int|z-\lambda|^2\,d\mu_v$. In finite dimension the calculus is simply $f(T)=\sum_jf(\lambda_j)P_j$, the sum over [eigenspaces](../../../../../eigenspace.md). In general it also permits discontinuous cuts and Borel choices of square roots, such as $s(z)=|z|^{1/2}e^{i\operatorname{Arg}(z)/2}$ with $s(0)=0$, giving a [normal operator](../../../../../normal-operator.md) $s(T)$ with $s(T)^2=T$ even when a continuous scalar branch is unavailable.

Any [bounded operator](../../../../../continuous-linear-operator.md) commuting with both $T$ and $T^*$ commutes with their [continuous functional calculus](../../../../../continuous-functional-calculus.md) and with all $E(S)$. To justify the latter, regularity approximates $\mathbf1_S$ by uniformly bounded [continuous functions](../../../../../continuous-function.md) in the $L^2$ norms of any finite list of vector measures; the resulting net converges strongly to $E(S)$. Thus the [Borel calculus](../../../../../borel-functional-calculus-for-a-normal-operator.md) lies in the [Von Neumann algebra](../../../../../von-neumann-algebra.md) generated by $T$. On a [separable Hilbert space](../../../../../separable-hilbert-space.md), a countable dense list of vectors gives a controlling measure $\mu=\sum_j2^{-j}\mu_{v_j}/(1+\|v_j\|^2)$; spectral-null sets are exactly its [null sets](../../../../../null-set.md), and the range is the represented $L^\infty(K,\mu)$, equal to that [Von Neumann algebra](../../../../../von-neumann-algebra.md). Without separability this last equality is not automatic: for the diagonal operator with one eigenvector for each $t\in[0,1]$, the generated [Von Neumann algebra](../../../../../von-neumann-algebra.md) has arbitrary bounded diagonal functions, while the original [Borel calculus](../../../../../borel-functional-calculus-for-a-normal-operator.md) has Borel diagonal functions. The spectral-measure construction and the strong convergence theorem themselves require no separability. This distinguishes the [Borel functional calculus for a normal operator](../../../../../borel-functional-calculus-for-a-normal-operator.md) from its continuous predecessor without confusing pointwise functions, spectral equivalence classes and topological closure.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
