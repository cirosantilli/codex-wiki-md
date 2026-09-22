# Analysis of Boolean functions

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analysis_of_Boolean_functions)

Analysis of Boolean functions studies real-valued [functions](function.md) on a [Boolean hypercube](#boolean-hypercube) using [Fourier analysis](#fourier-walsh-transform), [probability theory](probability-theory.md), and [combinatorics](combinatorics.md).

**Table of contents**

- [Friedgut-Kalai sharp threshold theorem](#friedgut-kalai-sharp-threshold-theorem)
- [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)
  - [Maximum-influence logarithmic lower bound](#maximum-influence-logarithmic-lower-bound)
  - [Squared-influence logarithmic lower bound](#squared-influence-logarithmic-lower-bound)
- [Boolean hypercube](#boolean-hypercube)
  - [Face of the Boolean hypercube](#face-of-the-boolean-hypercube)
  - [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)
    - [Complementary-size simplicial vertex boundaries can be asymmetric](#complementary-size-simplicial-vertex-boundaries-can-be-asymmetric)
    - [Simplicial vertex boundaries need not increase below half volume](#simplicial-vertex-boundaries-need-not-increase-below-half-volume)
  - [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)
    - [Half-cube vertex-boundary extrema](#half-cube-vertex-boundary-extrema)
    - [Cross-intersection bound from cube separation](#cross-intersection-bound-from-cube-separation)
    - [Nonunique down-set extremizers for Harper theorem](#nonunique-down-set-extremizers-for-harper-theorem)
    - [Simplicial section compression](#simplicial-section-compression)
      - [Terminal families for simplicial section compression](#terminal-families-for-simplicial-section-compression)
    - [Harper theorem implies the Kruskal-Katona theorem](#harper-theorem-implies-the-kruskal-katona-theorem)
  - [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)
    - [Section compression in binary order](#section-compression-in-binary-order)
      - [Families compressed in every binary section](#families-compressed-in-every-binary-section)
    - [Binary initial segment](#binary-initial-segment)
    - [Binary digit-sum inequality](#binary-digit-sum-inequality)
  - [Edge boundary in a graph](#edge-boundary-in-a-graph)
    - [Isoperimetric number of a graph](#isoperimetric-number-of-a-graph)
    - [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)
      - [Entropy proof of cube edge-isoperimetry](#entropy-proof-of-cube-edge-isoperimetry)
        - [Equality cases of entropy cube edge-isoperimetry](#equality-cases-of-entropy-cube-edge-isoperimetry)
      - [Edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments)
        - [Binary initial segments maximize contained square faces](#binary-initial-segments-maximize-contained-square-faces)
      - [Binary entropy function](#binary-entropy-function)
  - [Boolean function](#boolean-function)
    - [Quite fair Boolean function](#quite-fair-boolean-function)
    - [Algebraic normal form](#algebraic-normal-form)
    - [Separated Boolean decomposition](#separated-boolean-decomposition)
    - [Random restriction of a Boolean function](#random-restriction-of-a-boolean-function)
    - [Tribes function](#tribes-function)
      - [Balanced tribes construction with unused coordinates](#balanced-tribes-construction-with-unused-coordinates)
      - [Tribes threshold window](#tribes-threshold-window)
    - [Block sensitivity](#block-sensitivity)
    - [Monotone Boolean function](#monotone-boolean-function)
    - [Fourier-Walsh transform](#fourier-walsh-transform)
      - [Fourier weight](#fourier-weight)
        - [Expected Fourier weight after a random restriction](#expected-fourier-weight-after-a-random-restriction)
      - [Coordinate-flip generator on a hypercube](#coordinate-flip-generator-on-a-hypercube)
        - [Even-function spectral gap on a hypercube](#even-function-spectral-gap-on-a-hypercube)
      - [Walsh character](#walsh-character)
      - [p-biased product measure](#p-biased-product-measure)
        - [p-biased Fourier coefficient](#p-biased-fourier-coefficient)
      - [Discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function)
        - [Influence of a variable](#influence-of-a-variable)
          - [Hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound)
          - [Total influence](#total-influence)
            - [Margulis–Russo formula](#margulis-russo-formula)
              - [Pivotal for an increasing event](#pivotal-for-an-increasing-event)
      - [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)
        - [Beckner's inequality](#beckner-s-inequality)
          - [Low-degree Fourier mass of a sparse Boolean set](#low-degree-fourier-mass-of-a-sparse-boolean-set)
        - [Noise stability](#noise-stability)
      - [Linear Fourier weight](#linear-fourier-weight)
    - [Junta](#junta)
      - [Friedgut junta inequality](#friedgut-junta-inequality)
        - [Friedgut junta theorem](#friedgut-junta-theorem)
      - [Nisan-Szegedy junta theorem](#nisan-szegedy-junta-theorem)
    - [Quasirandom Boolean function](#quasirandom-boolean-function)
      - [Regularity lemma for Boolean functions](#regularity-lemma-for-boolean-functions)
- [Bonami lemma](#bonami-lemma)
  - [Hypercontractive inequality on the Boolean hypercube](#hypercontractive-inequality-on-the-boolean-hypercube)
  - [Anticoncentration of a low-degree function](#anticoncentration-of-a-low-degree-function)
- [Arrow's impossibility theorem](#arrow-s-impossibility-theorem)
  - [Condorcet paradox](#condorcet-paradox)
- [Invariance principle for a low-degree multilinear polynomial](#invariance-principle-for-a-low-degree-multilinear-polynomial)
  - [Lindeberg replacement method](#lindeberg-replacement-method)

## Friedgut-Kalai sharp threshold theorem

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)

There is an absolute $C>0$ such that any nontrivial [transitive increasing event](probability-inequality.md#transitive-increasing-event) on $n\geq2$ independent bits satisfies $\mu_q(A)>1-\varepsilon$ if $\mu_p(A)>\varepsilon$, $0<\varepsilon<1/2$, and the displayed bound holds with $p<q<1$. A uniform weighted [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem) gives one pivotal probability at least $c\mu_r(A)(1-\mu_r(A))\log(n)/n$. Transitivity makes the [total influence](#total-influence) at least $c\mu_r(A)(1-\mu_r(A))\log n$. The [Margulis–Russo formula](#margulis-russo-formula) identifies this with the derivative of $\mu_r(A)$. Integration of the derivative of its log odds proves the threshold bound.

## Kahn-Kalai-Linial theorem

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)

For a [Boolean function](#boolean-function) $f:\{0,1\}^n\to\{0,1\}$ under the uniform [probability measure](probability-space.md#probability-measure), some coordinate has [influence of a variable](#influence-of-a-variable) at least $c\operatorname{Var}(f)\log(n)/n$, where $c>0$ is an absolute constant and $I_i(f)$ is the probability that flipping coordinate $i$ changes $f$. For [variance](variance.md) bounded below, this is order $\log(n)/n$. The [tribes function](#tribes-function) shows that this order cannot be improved for general balanced [Boolean functions](#boolean-function).

### Maximum-influence logarithmic lower bound

↑ **Parent:** [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)

For a zero-one [Boolean function](#boolean-function) on the unbiased [Boolean hypercube](#boolean-hypercube) with flip-probability [influences](#influence-of-a-variable) $\beta_i\leq\beta$, the displayed bound holds for sufficiently small $\beta>0$. If it fails, write $b=\log(1/\beta)/3$. The [total influence](#total-influence) identity puts at least half the nonconstant [Fourier weight](#fourier-weight) on levels $1\leq|S|\leq b$. The [hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound) at $\delta=e^{-1}$ then gives $\sum_i\beta_i^{2/(1+\delta)}\geq2b\delta^b\operatorname{Var}(f)$. Its upper bound $\beta^{(1-\delta)/(1+\delta)}\sum_i\beta_i$ contradicts $(1-\delta)/(1+\delta)>1/3$.

### Squared-influence logarithmic lower bound

↑ **Parent:** [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)

For a zero-one [Boolean function](#boolean-function) of mean $t$, the displayed bound holds for sufficiently large $n$, uniformly in $t$. If it failed, put $v=t(1-t)$, $\lambda=v\log n$ and split its nonconstant [Fourier weight](#fourier-weight) at level $b=(\log n)/3$. The [total influence](#total-influence) bound puts at most $3v/4$ above that level. The [hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound) with $\delta=1-3\log\log n/\log n$ puts only $o(v)$ below it: the conversion factor $\max_{1\leq s\leq b}[s\delta^{s-1}]^{-1}$ stays bounded, while $\lambda^{2/(1+\delta)}n^{1-2/(1+\delta)}=vO((\log n)^{-1/2+o(1)})$. This contradicts total nonconstant weight $v$.

## Boolean hypercube

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)

The Boolean hypercube is the set $\{-1,1\}^n$, or equivalently $\{0,1\}^n$. Its [hypercube graph](graph.md#hypercube-graph) joins two vertices exactly when they differ in one coordinate.

### Face of the Boolean hypercube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

A face is obtained by fixing some coordinates of the [Boolean hypercube](#boolean-hypercube) and letting the remaining $d$ coordinates vary freely. It is isomorphic to $Q_d$. A two-dimensional face is a square with four vertices, and a face is contained in a [set family](extremal-set-theory.md#set-family) when all its vertices belong to that family.

### Simplicial order on the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

Order subsets first by increasing [cardinality](cardinal-number.md#cardinality) and, within each level, by [lexicographic order](extremal-set-theory.md#lexicographic-order), with the smallest differing coordinate belonging to the earlier set. This convention makes simplicial [initial segments](set.md#initial-segment) the extremizers in [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube).

#### Complementary-size simplicial vertex boundaries can be asymmetric

↑ **Parent:** [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)

In the seven-dimensional [Boolean hypercube](#boolean-hypercube), $C(63)$ contains every set of size at most three except $\{5,6,7\}$. Its external [vertex boundary](graph-theory.md#external-vertex-boundary) consists of that missing triple and all 35 four-sets. The complementary-size [initial segment](set.md#initial-segment) $C(65)$ contains every set of size at most three and $\{1,2,3,4\}$. Its external [vertex boundary](graph-theory.md#external-vertex-boundary) has the other 34 four-sets and three five-sets. Thus complementary family sizes do not impose a symmetric boundary profile.

#### Simplicial vertex boundaries need not increase below half volume

↑ **Parent:** [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)

In dimension three, the first three vertices are $\varnothing,\{1\},\{2\}$. Their closed [vertex neighbourhood](graph.md#vertex-neighbourhood) has seven vertices. Adding $\{3\}$ does not change that [vertex neighbourhood](graph.md#vertex-neighbourhood), so the external [vertex boundary](graph-theory.md#external-vertex-boundary) decreases from four to three even though both family sizes are at most half the cube.

### Vertex-isoperimetric inequality in the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

For the [Boolean hypercube](#boolean-hypercube), the [initial segment](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) minimizes the size of the closed [vertex neighbourhood](graph.md#vertex-neighbourhood) among families of a given size. Equivalently, it minimizes the [external vertex boundary](graph-theory.md#external-vertex-boundary). This is a vertex assertion, distinct from the [edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube).

#### Half-cube vertex-boundary extrema

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

For $n\geq1$, a family of $2^{n-1}$ vertices in the [Boolean hypercube](#boolean-hypercube) has these minimum and maximum external [vertex boundary](graph-theory.md#external-vertex-boundary) sizes. The [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube) gives the minimum: in odd dimension take the lower half of the levels, and in even dimension add the middle-level sets containing coordinate one to all lower levels. The family of even [Hamming weight](coding-theory.md#hamming-weight) attains the maximum, since every remaining vertex has an adjacent even-weight vertex.

#### Cross-intersection bound from cube separation

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

If two nonempty [set families](extremal-set-theory.md#set-family) on $m\geq1$ coordinates have every cross-intersection greater than an integer $w\geq0$, their density product obeys the displayed bound. Complementing the second [set family](extremal-set-theory.md#set-family) separates it from the first by [Hamming distance](coding-theory.md#hamming-distance) greater than $w$. [Harper inequality](#vertex-isoperimetric-inequality-in-the-discrete-cube) bounds the first [set family](extremal-set-theory.md#set-family)'s radius-$w$ neighbourhood from below. If $S_m(a-1)<|\mathcal F|\leq S_m(a)$, disjointness yields $|\mathcal F||\mathcal G|\leq S_m(a)S_m(m-a-w)$. The [binary entropy function](#binary-entropy-function) tail estimate bounds these two factors by Gaussian tails; their deficits from the middle rank sum to at least $w$, proving the claim.

#### Nonunique down-set extremizers for Harper theorem

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Equality in [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube) need not make a [down-set](extremal-set-theory.md#down-set) a cube-automorphic image of a simplicial [initial segment](set.md#initial-segment). In $Q_4$, take all sets of size at most one and the four two-element sets forming a four-cycle. This family has size nine and [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood) size fifteen, just like the size-nine [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) [initial segment](set.md#initial-segment). The induced [degree of a vertex](graph-theory.md#degree-graph-theory) distributions differ, so they cannot be related by a [graph automorphism](graph.md#graph-automorphism).

#### Simplicial section compression

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Split a [set family](extremal-set-theory.md#set-family) in the [hypercube graph](graph.md#hypercube-graph) according to whether coordinate $i$ is present, and delete that coordinate from the present section. Replace both sections by [initial segments](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) with the same respective sizes. Induction and nesting of initial-segment [closed graph neighbourhoods](graph-theory.md#closed-graph-neighbourhood) show that this operation cannot enlarge the original [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood). Repeated nontrivial compressions terminate because the sum of simplicial positions strictly decreases.

##### Terminal families for simplicial section compression

↑ **Parent:** [Simplicial section compression](#simplicial-section-compression)

A family fixed by every [simplicial section compression](#simplicial-section-compression) is either an [initial segment](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) or that segment with its last vertex exchanged for the next vertex, where the exchanged vertices are complementary. Indeed, an earlier absent vertex and a later present vertex must differ in every coordinate, and cannot have another vertex between them. Complementary consecutive vertices occur only across the two central ranks in odd dimension, or at the transition from middle-rank sets containing coordinate one to those avoiding it in even dimension. Direct [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood) comparison resolves these exceptions in the proof of [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube).

#### Harper theorem implies the Kruskal-Katona theorem

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Adjoin all lower levels to a [uniform set family](extremal-set-theory.md#uniform-set-family) before applying [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube). Its remaining neighbourhood contribution is the [upper shadow](extremal-set-theory.md#upper-shadow), so lexicographic [initial segments](set.md#initial-segment) minimize upper shadows. Complementation and reversal of coordinates turn this into [colexicographic order](extremal-set-theory.md#colexicographic-order) minimizing the [lower shadow](extremal-set-theory.md#lower-shadow), giving the [Kruskal-Katona theorem](extremal-set-theory.md#kruskal-katona-theorem).

### Binary order on the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

Identify a vertex $(x_1,\ldots,x_n)$ with the integer $\sum_{i=1}^n2^{i-1}x_i$. Binary order is increasing order of these integers. Its initial segment of size $a$ has $F(a)=\sum_{j=0}^{a-1}s_2(j)$ induced edges, where $s_2(j)$ is the [Hamming weight](coding-theory.md#hamming-weight) of the binary expansion of $j$.

#### Section compression in binary order

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

Fix a coordinate of the [Boolean hypercube](#boolean-hypercube), delete it in each of the two sections, and replace each section by a [binary initial segment](#binary-initial-segment) of the same size. This preserves the total size. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on dimension proves that it does not decrease contained edge counts; the crossing contribution is the size of the section intersection, maximized by nested initial segments.

##### Families compressed in every binary section

↑ **Parent:** [Section compression in binary order](#section-compression-in-binary-order)

If both sections for every coordinate are [binary initial segments](#binary-initial-segment), then the family itself is a binary initial segment, apart from the possible family $(\mathcal P([n-1])\setminus\{[n-1]\})\cup\{\{n\}\}$. Any missing vertex earlier than a present vertex must disagree with it in every coordinate; the two are therefore complementary and consecutive in [binary order on the discrete cube](#binary-order-on-the-discrete-cube), forcing this sole exceptional shape.

#### Binary initial segment

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

An [initial segment](set.md#initial-segment) of the [binary order on the discrete cube](#binary-order-on-the-discrete-cube) contains the vertices whose integer encodings are $0,\ldots,m-1$. It is a [down-set](extremal-set-theory.md#down-set), so its internal edges and two-dimensional [cube faces](#face-of-the-boolean-hypercube) can be counted at their unique upper vertices by $\sum_{j<m}\operatorname{wt}(j)$ and $\sum_{j<m}\binom{\operatorname{wt}(j)}2$.

#### Binary digit-sum inequality

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

For $F(a)=\sum_{j=0}^{a-1}s_2(j)$ and nonnegative integers $a,b$, the displayed inequality follows by induction from $F(2r)=2F(r)+r$ and $F(2r+1)=F(r)+F(r+1)+r$. Splitting a vertex set of a [hypercube graph](graph.md#hypercube-graph) into its two coordinate sections then proves the [edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments).

### Edge boundary in a graph

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

The edge boundary of a vertex set $A$ consists of graph edges with exactly one endpoint in $A$. In a $d$-regular graph,

$$
|\partial_eA|=d|A|-2e(A),
$$

where $e(A)$ counts edges with both endpoints in $A$.

#### Isoperimetric number of a graph

↑ **Parent:** [Edge boundary in a graph](#edge-boundary-in-a-graph)

For a finite [graph](graph.md) with at least two [vertices](graph.md#vertex-graph-theory), the displayed minimum measures the fewest outgoing [edges](graph-theory.md#edge-of-a-graph) per vertex in a nonempty set occupying at most half the [graph](graph.md). It uses the [edge boundary](#edge-boundary-in-a-graph), rather than the [external vertex boundary](graph-theory.md#external-vertex-boundary). For the [hypercube graph](graph.md#hypercube-graph) $Q_n$, $n\ge1$, it equals one: edge-isoperimetry gives the lower bound and a coordinate half-cube attains it.

#### Edge-isoperimetric inequality in the discrete cube

↑ **Parent:** [Edge boundary in a graph](#edge-boundary-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge-isoperimetric_inequality_in_the_discrete_cube)

For $A\subseteq\{0,1\}^n$,

$$
|\partial_eA|\geq|A|\log_2\frac{2^n}{|A|}.
$$

Equivalently, $A$ spans at most $\frac12|A|\log_2|A|$ cube edges. Induction on the dimension and concavity of [binary entropy](#binary-entropy-function) prove the inequality.

##### Entropy proof of cube edge-isoperimetry

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)

For a vertex set of size $m$ in a [hypercube graph](graph.md#hypercube-graph), split one coordinate into sections of sizes $a,b$. Induction bounds the internal edges within the sections by $(a\log_2a+b\log_2b)/2$; at most $\min(a,b)$ edges cross between them. Put $t=\min(a,b)/(a+b)$. The chord bound for the [binary entropy function](#binary-entropy-function) gives $H_2(t)\ge2t$, hence $a\log_2a+b\log_2b+2\min(a,b)\le m\log_2m$. Thus at most $m\log_2m/2$ internal edges are present, and the [edge boundary](#edge-boundary-in-a-graph) is at least $m(n-\log_2m)$. Coordinate subcubes attain equality when $m$ is a power of two.

###### Equality cases of entropy cube edge-isoperimetry

↑ **Parent:** [Entropy proof of cube edge-isoperimetry](#entropy-proof-of-cube-edge-isoperimetry)

For a nonempty subset of a [hypercube graph](graph.md#hypercube-graph), split it into sections of sizes $a,b$. The proof of the entropy edge bound uses $H_2(t)\ge2t$, $t=\min(a,b)/(a+b)$. Strict concavity makes equality possible only at $t=0$ or $t=1/2$. In the first case one section is empty; in the second the sections coincide, since all possible crossing [edges](graph-theory.md#edge-of-a-graph) must be present. Induction forces a [coordinate subcube](#face-of-the-boolean-hypercube). Conversely every [coordinate subcube](#face-of-the-boolean-hypercube) has the displayed edge count. At size $2^{n-1}$ these are exactly the two halves determined by fixing one coordinate.

##### Edge-isoperimetric theorem for binary initial segments

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)

Among subsets of the $n$-dimensional [hypercube graph](graph.md#hypercube-graph) with $a$ vertices, initial segments of the [binary order on the discrete cube](#binary-order-on-the-discrete-cube) minimize the [edge boundary](#edge-boundary-in-a-graph). Its exact minimum is $na-2\sum_{j=0}^{a-1}s_2(j)$. This strengthens the entropy lower bound on the same boundary.

###### Binary initial segments maximize contained square faces

↑ **Parent:** [Edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments)

Among families of a given size in the [Boolean hypercube](#boolean-hypercube), a [binary initial segment](#binary-initial-segment) maximizes the number of contained two-dimensional [cube faces](#face-of-the-boolean-hypercube). Under [section compression in binary order](#section-compression-in-binary-order), faces crossing the selected coordinate correspond to internal edges in the intersection of its two sections. The edge extremal theorem and [mathematical induction](foundations-of-mathematics.md#mathematical-induction) control that contribution and the faces within the sections.

##### Binary entropy function

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_entropy_function)

The binary entropy function is

$$
H_2(x)=-x\log_2x-(1-x)\log_2(1-x).
$$

It is concave on $[0,1]$ and satisfies $H_2(x)\geq2x$ for $0\leq x\leq1/2$ by comparison with the chord from $(0,0)$ to $(1/2,1)$.

### Boolean function

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_function)

A Boolean function is a function on a [Boolean hypercube](#boolean-hypercube), often with codomain $\{-1,1\}$ or $\{0,1\}$.

#### Quite fair Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

Under uniform independent input bits, a zero-one [Boolean function](#boolean-function) is quite fair when its mean lies between one quarter and three quarters. This convention excludes functions whose output is nearly constant; it does not require exact balance or equal coordinate influences.

#### Algebraic normal form

↑ **Parent:** [Boolean function](#boolean-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_normal_form)

The algebraic normal form is the unique multilinear polynomial representation of a [Boolean function](#boolean-function) over the field with two elements, using [exclusive or](theoretical-computer-science.md#exclusive-or) for addition and ordinary bit multiplication for products. The empty product is one. Existence and uniqueness follow by induction from $f(z',z_d)=f(z',0)\oplus z_d(f(z',0)\oplus f(z',1))$: the first polynomial supplies all coefficients not containing $z_d$, and the difference supplies exactly those that do. For split inputs $(x,y)$, each monomial factors into one locally computed product of Alice's bits and one of Bob's bits, yielding a [separated Boolean decomposition](#separated-boolean-decomposition).

#### Separated Boolean decomposition

↑ **Parent:** [Boolean function](#boolean-function)

Every [Boolean function](#boolean-function) of distributed inputs is an [exclusive or](theoretical-computer-science.md#exclusive-or) of products of locally computable bits. The displayed identity follows because exactly one indicator is one. It uses at most $2^m$ terms, each a function of $x$ times a function of $y$; exchanging the two input roles gives at most $2^n$ terms. This elementary truth-table factorization is useful for distributed computation with [PR boxes](foundations-of-quantum-mechanics.md#popescu-rohrlich-box) and does not depend on a probabilistic approximation.

#### Random restriction of a Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A $p$-random restriction independently leaves each coordinate live with probability $p$, otherwise fixing it to zero or one with probability $(1-p)/2$ each. Composing independent restrictions with live probabilities $p_1,\ldots,p_d$ produces the same distribution with live probability $\prod_jp_j$. Fixed values stay unbiased.

#### Tribes function

↑ **Parent:** [Boolean function](#boolean-function)

A tribes function is an OR of AND blocks: partition $mw$ coordinates into $m$ blocks of size $w$, and let $f=1$ when at least one block consists entirely of ones. For [independent random variables](random-variable.md#independent-random-variables) with each bit uniform, $\mathbb P(f=0)=(1-2^{-w})^m$. The [influence of a variable](#influence-of-a-variable) is $2^{-(w-1)}(1-2^{-w})^{m-1}$, because every other bit in its block must be one and every other block must fail. Taking $m$ approximately $(\log2)2^w$ keeps both output probabilities bounded away from zero and gives influences of order $\log(mw)/(mw)$. This shows the order in the [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem) is sharp.

##### Balanced tribes construction with unused coordinates

↑ **Parent:** [Tribes function](#tribes-function)

Choose $w\geq1$ maximal such that $wm\leq n$ for the displayed $m$, and take the OR of $m$ AND blocks of size $w$, ignoring unused coordinates. Its failure probability is $(1-2^{-w})^m$, between one quarter and three quarters. Active coordinates have [influence](#influence-of-a-variable) $2^{1-w}(1-2^{-w})^{m-1}$ and unused ones have zero influence. Maximality gives $2^{1-w}<4(\log2)(w+1)/n$; for $n\geq2$, $w\leq\log_2n$, so every influence is below $8\log n/n$. The construction is therefore a [quite fair Boolean function](#quite-fair-boolean-function) with small influences for every $n\geq2$. The logarithmic bound cannot hold at $n=1$, where every quite fair function has influence one.

##### Tribes threshold window

↑ **Parent:** [Tribes function](#tribes-function)

For $m$ tribes of size $w$ with $m\sim(\log2)2^w$ and $n=mw$, the success probability under the [p-biased product measure](#p-biased-product-measure) is $1-(1-p^w)^m$. Its $x$-quantile is $p_x=[1-(1-x)^{1/m}]^{1/w}$. For fixed $0<x<1$,

$$
p_x=\frac12+\frac1{2w}\log\frac{-\log(1-x)}{\log2}+O_x(w^{-2}).
$$

Thus the fixed-error window has order $1/\log n$. For small fixed error the leading coefficient grows with $\log(1/\varepsilon)$, so the general [Friedgut-Kalai sharp threshold theorem](#friedgut-kalai-sharp-threshold-theorem) also has the correct error dependence up to absolute constants.

#### Block sensitivity

↑ **Parent:** [Boolean function](#boolean-function)

For an input $x$, count the largest family of pairwise disjoint nonempty sets of coordinates such that flipping each set individually changes the [Boolean function](#boolean-function) value. Maximizing over inputs gives block sensitivity. Sensitive sets need not be contiguous and need not consist of single bits. The standard bounded-error [quantum query complexity](theoretical-computer-science.md#quantum-query-complexity) lower bound is $\Omega(\sqrt{\operatorname{bs}(f)})$. A certificate for $f(x)$ meets every sensitive set, so its size bounds their disjoint count.

#### Monotone Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A Boolean function $f:\{0,1\}^n\to\{0,1\}$ is a [monotone function](calculus.md#monotonic-function) when $x_i\leq y_i$ for every $i$ implies $f(x)\leq f(y)$.

#### Fourier-Walsh transform

↑ **Parent:** [Boolean function](#boolean-function)

For $f:\{-1,1\}^n\to\mathbb R$, the characters $\chi_S(x)=\prod_{i\in S}x_i$ form an [orthonormal basis](inner-product.md#orthonormal-basis), and the Fourier-Walsh expansion is

$$
f=\sum_{S\subseteq[n]}\widehat f(S)\chi_S,
\qquad
\widehat f(S)=\mathbb E[f\chi_S].
$$

On the finite Boolean hypercube, these coefficients are the [Hadamard transform](quantum-theory.md#hadamard-transform) of the vector of function values, with expectation normalization.

##### Fourier weight

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

Fourier weight is the squared [Fourier-Walsh transform](#fourier-walsh-transform) coefficient mass on specified levels or a specified family of subsets. [Parseval's identity](fourier-analysis.md#parseval-identity) identifies the total weight with $\mathbb E|f|^2$, and the nonconstant weight with [variance](variance.md). A decision tree of depth at most $s$ has no weight above level $s$.

###### Expected Fourier weight after a random restriction

↑ **Parent:** [Fourier weight](#fourier-weight)

For a [random restriction](#random-restriction-of-a-boolean-function), first fix the live set $J$ and average over the unbiased assignment $a$ outside it. The coefficient at $U\subset J$ is $\sum_{B\subset J^c}\widehat f(U\cup B)\chi_B(a)$. Orthogonality eliminates cross terms in its squared expectation. Averaging over $J$ gives the displayed identity. The original [Fourier weight](#fourier-weight) is weighted by a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) survival probability, not simply preserved.

##### Coordinate-flip generator on a hypercube

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

For independent coordinate flips at rate $1/2$, a [Walsh character](#walsh-character) $w_A$ is an eigenfunction with [eigenvalue](linear-operator-theory.md#eigenvalue) $-|A|$. The generator is self-adjoint and negative semidefinite. Its [Dirichlet form of a Markov chain](markov-chain.md#dirichlet-form-of-a-markov-chain) is $-\mathbb E[fLf]=\frac14\sum_i\mathbb E(f(\omega^{(i)})-f(\omega))^2$.

###### Even-function spectral gap on a hypercube

↑ **Parent:** [Coordinate-flip generator on a hypercube](#coordinate-flip-generator-on-a-hypercube)

Global sign-even functions have zero coefficients on odd-size [Walsh characters](#walsh-character). Every nonconstant remaining character has generator [eigenvalue](linear-operator-theory.md#eigenvalue) at most $-2$, yielding the displayed improvement from gap one to gap two. Combining this with the convexity of a [norm](normed-vector-space.md#norm) proves the [sharp Rademacher second-moment inequality](fourier-analysis.md#sharp-rademacher-second-moment-inequality).

##### Walsh character

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

For $S\subseteq[n]$, the Walsh character on the [Boolean hypercube](#boolean-hypercube) is $\chi_S(x)=\prod_{i\in S}x_i$, equivalently $(-1)^{\sum_{i\in S}x_i}$ in the zero-one convention.

##### p-biased product measure

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

Under the $p$-biased product measure $\mu_p$ on $\{-1,1\}^n$, the coordinates are [independent random variables](random-variable.md#independent-random-variables) with $\mathbb P(x_i=-1)=p$ and $\mathbb P(x_i=1)=1-p$. Writing $\mu=1-2p$, $\sigma=2\sqrt{p(1-p)}$, and $\phi_i=(x_i-\mu)/\sigma$, the products $\phi_S=\prod_{i\in S}\phi_i$ form the $p$-biased [Fourier basis](#fourier-walsh-transform).

###### p-biased Fourier coefficient

↑ **Parent:** [P-biased product measure](#p-biased-product-measure)

The $p$-biased Fourier coefficient of $f$ at $S$ is $\widehat f_p(S)=\mathbb E_{\mu_p}[f\phi_S]$.

##### Discrete derivative of a Boolean function

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

On the unbiased cube, the discrete derivative is

$$
D_i f(x)=\frac{f(x^{i\to1})-f(x^{i\to-1})}{2}
=\sum_{S\ni i}\widehat f(S)\chi_{S\setminus\{i\}}(x).
$$

For the [p-biased product measure](#p-biased-product-measure), the normalization factor is $\sigma/2$.

###### Influence of a variable

↑ **Parent:** [Discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function)

For the $\{-1,1\}$-valued convention on the unbiased [Boolean hypercube](#boolean-hypercube), the influence of coordinate $i$ is $\operatorname{Inf}_i(f)=\lVert D_i f\rVert_2^2$, where $D_i f$ is the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function). It equals the [probability](probability-theory.md#probability) that flipping coordinate $i$ changes $f$. For the $\{0,1\}$-valued convention, the same flip probability is instead $4\lVert D_i f\rVert_2^2$, since a nonzero discrete derivative has magnitude $1/2$.

###### Hypercontractive weighted influence bound

↑ **Parent:** [Influence of a variable](#influence-of-a-variable)

For a zero-one [Boolean function](#boolean-function), the flip-probability [influence](#influence-of-a-variable) is $\beta_i=4\sum_{S\ni i}\widehat f(S)^2$. Apply [Beckner's inequality](#beckner-s-inequality) with noise parameter $\sqrt\delta$ to the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function), whose nonzero magnitude is $1/2$. Its $L^{1+\delta}$ norm squared is $\beta_i^{2/(1+\delta)}/4$. Summing over coordinates gives the displayed weighted [Fourier weight](#fourier-weight) bound, a useful intermediate step in influence lower bounds.

###### Total influence

↑ **Parent:** [Influence of a variable](#influence-of-a-variable)

The total influence is

$$
\mathbf I(f)=\sum_i\operatorname{Inf}_i(f)
=\sum_{S\subseteq[n]}|S|\widehat f(S)^2.
$$

This [Fourier-Walsh transform](#fourier-walsh-transform) identity uses $\{-1,1\}$-valued $f$ and the flip-probability convention for [influence of a variable](#influence-of-a-variable). For $\{0,1\}$-valued $f$, the right-hand side is multiplied by four. Indeed [Parseval's identity](fourier-analysis.md#parseval-identity) applied to the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function) gives $\|D_i f\|_2^2=\sum_{S\ni i}\widehat f(S)^2$; sum over coordinates and apply the chosen normalization.

<h6 id="margulis-russo-formula">Margulis–Russo formula</h6>

↑ **Parent:** [Total influence](#total-influence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Margulis–Russo_formula)

For the indicator $f$ of a monotone family under a [p-biased product measure](#p-biased-product-measure), the Margulis–Russo formula identifies the derivative of $\mathbb E_{\mu_p}f$ with the suitably normalized [total influence](#total-influence) of $f$.

###### Pivotal for an increasing event

↑ **Parent:** [Margulis–Russo formula](#margulis-russo-formula)

A coordinate is pivotal for an increasing event in a configuration when changing only that coordinate changes whether the event occurs. Its pivotal probability is the coordinate's influence.

##### Noise operator on the Boolean hypercube

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

The noise operator averages $f(y)$ over a random $y$ correlated with $x$ by $\rho$. It acts diagonally on the [Fourier-Walsh transform](#fourier-walsh-transform):

$$
T_\rho f=\sum_S\rho^{|S|}\widehat f(S)\chi_S.
$$

<h6 id="beckner-s-inequality">Beckner's inequality</h6>

↑ **Parent:** [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)

For $1<p\leq q<\infty$ and $0\leq\rho\leq\sqrt{(p-1)/(q-1)}$, the [noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube) satisfies $\|T_\rho f\|_q\leq\|f\|_p$ for the uniform [probability measure](probability-space.md#probability-measure). In particular,

$$
\sum_S\rho^{2|S|}|\widehat f(S)|^2\leq\|f\|_{1+\rho^2}^2
\qquad(0\leq\rho\leq1).
$$

Here $\widehat f(S)$ are [Fourier-Walsh transform](#fourier-walsh-transform) coefficients. The endpoint $\rho=0$ follows by averaging. This [hypercontractive inequality on the Boolean hypercube](#hypercontractive-inequality-on-the-boolean-hypercube) controls [Fourier-Walsh transform](#fourier-walsh-transform) coefficients of [discrete derivatives of a Boolean function](#discrete-derivative-of-a-boolean-function) and is a principal ingredient in the [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem).

###### Low-degree Fourier mass of a sparse Boolean set

↑ **Parent:** [Beckner's inequality](#beckner-s-inequality)

For a subset of the unbiased [Boolean hypercube](#boolean-hypercube) of density $\alpha$, use normalized [Fourier-Walsh transform](#fourier-walsh-transform) coefficients. Applying [Beckner's inequality](#beckner-s-inequality) with $\rho=1/\sqrt3$ gives $\|T_\rho1_A\|_2^2\leq\|1_A\|_{4/3}^2=\alpha^{3/2}$. On levels at most two the weights $\rho^{2|S|}$ are at least $1/9$, giving the displayed bound. [Parseval's identity](fourier-analysis.md#parseval-identity) gives total Fourier mass $\alpha$, so when $9\sqrt\alpha<1/2$ the higher levels contain strictly more than the lower levels.

###### Noise stability

↑ **Parent:** [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noise_stability)

The noise stability is

$$
\operatorname{Stab}_\rho(f)=\langle f,T_\rho f\rangle
=\sum_S\rho^{|S|}\widehat f(S)^2.
$$

##### Linear Fourier weight

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

The linear Fourier weight is $W_1(f)=\sum_{|S|=1}\widehat f(S)^2$.

#### Junta

↑ **Parent:** [Boolean function](#boolean-function)

A $J$-junta is a function whose value depends only on coordinates indexed by $J$. A $k$-junta depends on at most $k$ coordinates.

##### Friedgut junta inequality

↑ **Parent:** [Junta](#junta)

If $f:\{-1,1\}^n\to\{-1,1\}$ satisfies $\lVert f^{\leq k}\rVert_2^2\geq1-\varepsilon$, then it has a real-valued $J$-junta approximation $g$ with $\lVert f-g\rVert_2^2\leq2\varepsilon$ and

$$
|J|\leq\frac{3^{2k}\mathbf I(f)^3}{\varepsilon^2}.
$$

###### Friedgut junta theorem

↑ **Parent:** [Friedgut junta inequality](#friedgut-junta-inequality)

For every $\varepsilon>0$, a Boolean function $f$ has an $\exp(O(\mathbf I(f)/\varepsilon))$-junta approximation with squared $L^2$ error at most $2\varepsilon$.

##### Nisan-Szegedy junta theorem

↑ **Parent:** [Junta](#junta)

Every Boolean function of degree at most $k$ is a $k2^{k-1}$-junta.

#### Quasirandom Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A Boolean function $f:\{0,1\}^n\to\{0,1\}$ is $(\varepsilon,p,r)$-quasirandom when conditioning any set of at most $r$ coordinates to any values changes its $\mu_p$-expectation by at most $\varepsilon$.

##### Regularity lemma for Boolean functions

↑ **Parent:** [Quasirandom Boolean function](#quasirandom-boolean-function)

For every $\varepsilon,p,r,\delta$, there is $T$ such that every Boolean function has a set $J$ with $|J|\leq T$ for which a $\mu_p$-random restriction on $J$ leaves an $(\varepsilon,p,r)$-quasirandom function with probability at least $1-\delta$.

## Bonami lemma

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)

The Bonami lemma states that a function of [Fourier degree](#fourier-walsh-transform) at most $k$ satisfies $\lVert f\rVert_4\leq3^{k/2}\lVert f\rVert_2$.

### Hypercontractive inequality on the Boolean hypercube

↑ **Parent:** [Bonami lemma](#bonami-lemma)

One form of the hypercontractive inequality is $\lVert T_{1/\sqrt3}f\rVert_4\leq\lVert f\rVert_2$, where $T_\rho$ is the [noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube).

### Anticoncentration of a low-degree function

↑ **Parent:** [Bonami lemma](#bonami-lemma)

If a nonzero function on the [Boolean hypercube](#boolean-hypercube) has degree at most $k$, then its support has measure at least $2^{-k}$. This sharp bound follows by induction on the dimension.

<h2 id="arrow-s-impossibility-theorem">Arrow's impossibility theorem</h2>

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arrow's_impossibility_theorem)

Arrow's theorem says that a rank-order voting system with at least three alternatives cannot simultaneously satisfy unrestricted preferences, unanimity, independence of irrelevant alternatives, and absence of a dictator.

### Condorcet paradox

↑ **Parent:** [Arrow's impossibility theorem](#arrow-s-impossibility-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Condorcet_paradox)

The Condorcet paradox is a cycle in collective pairwise preferences even though each individual voter's preference is transitive.

## Invariance principle for a low-degree multilinear polynomial

↑ **Parent:** [Analysis of Boolean functions](analysis-of-boolean-functions.md)

Let $X_i$ and $Y_i$ be independent, centered, variance-one random variables with vanishing third moments and fourth moments at most $9$. If $f$ is multilinear of degree at most $k$ and $\lVert\psi^{(4)}\rVert_\infty\leq M$, then

$$
|\mathbb E\psi(f(X))-\mathbb E\psi(f(Y))|
\leq\frac{M}{12}9^k\sum_i\operatorname{Inf}_i(f)^2.
$$

### Lindeberg replacement method

↑ **Parent:** [Invariance principle for a low-degree multilinear polynomial](#invariance-principle-for-a-low-degree-multilinear-polynomial)

The Lindeberg replacement method, inspired by the [Lindeberg condition](convergence-of-random-variables.md#lindeberg-condition), compares functions of two independent random vectors by replacing their coordinates one at a time. Matching moments cancel the corresponding terms in a [Taylor expansion](calculus.md#taylor-s-theorem).

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
