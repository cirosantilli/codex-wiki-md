# Information theory

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_theory)

**Table of contents**

- [Bit](#bit)
- [Memoryless classical information source](#memoryless-classical-information-source)
- [Alphabet](#alphabet)
- [Conditional entropy](#conditional-entropy)
  - [Equality in the entropy conditioning inequality](#equality-in-the-entropy-conditioning-inequality)
  - [Chain rule for conditional entropy](#chain-rule-for-conditional-entropy)
  - [Conditional entropy under a deterministic change of variables](#conditional-entropy-under-a-deterministic-change-of-variables)
  - [Conditioning reduces entropy](#conditioning-reduces-entropy)
  - [Fano's inequality](#fano-s-inequality)
    - [Fano's inequality via an error indicator](#fano-s-inequality-via-an-error-indicator)
    - [List-decoding Fano inequality](#list-decoding-fano-inequality)
  - [Entropy of a sum of independent finite-group variables](#entropy-of-a-sum-of-independent-finite-group-variables)
- [Mutual information](#mutual-information)
  - [Entropy submodularity](#entropy-submodularity)
    - [Compression of an entropy sum](#compression-of-an-entropy-sum)
      - [Balister–Bollobás entropy inequality](#balister-bollobas-entropy-inequality)
        - [Madiman–Tetali entropy inequality](#madiman-tetali-entropy-inequality)
    - [Shearer's inequality](#shearer-s-inequality)
      - [Entropy bound for graphs with isolated-vertex-free intersections](#entropy-bound-for-graphs-with-isolated-vertex-free-intersections)
  - [Conditional mutual information](#conditional-mutual-information)
  - [Chain rule for mutual information](#chain-rule-for-mutual-information)
  - [Data processing inequality](#data-processing-inequality)
    - [Conditional data-processing inequality](#conditional-data-processing-inequality)
  - [Incremental information in a twofold binary repetition code](#incremental-information-in-a-twofold-binary-repetition-code)
- [Entropic Ruzsa distance](#entropic-ruzsa-distance)
  - [Conditional entropic Ruzsa distance](#conditional-entropic-ruzsa-distance)
    - [Simultaneous conditional entropic Ruzsa distance](#simultaneous-conditional-entropic-ruzsa-distance)
    - [Conditioned entropic Ruzsa distance of a summand](#conditioned-entropic-ruzsa-distance-of-a-summand)
  - [Entropic Ruzsa triangle inequality](#entropic-ruzsa-triangle-inequality)
  - [Entropic Ruzsa sum-difference inequality](#entropic-ruzsa-sum-difference-inequality)
  - [Entropic Balog-Szemerédi-Gowers theorem](#entropic-balog-szemeredi-gowers-theorem)
  - [C-relevant pair of random variables](#c-relevant-pair-of-random-variables)
    - [Relevance of independent self-sums](#relevance-of-independent-self-sums)
- [Entropy submodularity for three independent sums](#entropy-submodularity-for-three-independent-sums)
- [Entropy submodularity for sums](#entropy-submodularity-for-sums)
- [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)
  - [Error exponents in hypothesis testing](#error-exponents-in-hypothesis-testing)
  - [Type I and type II errors](#type-i-and-type-ii-errors)
  - [Chernoff information](#chernoff-information)
  - [Stein's lemma (information theory)](#stein-s-lemma-information-theory)
  - [Neyman-Pearson decision region](#neyman-pearson-decision-region)
- [Total correlation](#total-correlation)
- [Type (information theory)](#type-information-theory)
  - [Type class](#type-class)
  - [Method of types](#method-of-types)
    - [Sanov theorem](#sanov-theorem)
    - [Information projection](#information-projection)
      - [Entropy minimization under a prescribed sample mean](#entropy-minimization-under-a-prescribed-sample-mean)
- [Rate-distortion function](#rate-distortion-function)
  - [Hamming distortion](#hamming-distortion)
- [Channel capacity](#channel-capacity)
  - [Weakly symmetric channel capacity](#weakly-symmetric-channel-capacity)
    - [Cyclic ternary channel capacity](#cyclic-ternary-channel-capacity)
    - [Binary symmetric channel capacity](#binary-symmetric-channel-capacity)
    - [Ternary symmetric channel capacity](#ternary-symmetric-channel-capacity)
- [Information entropy](#information-entropy)
  - [Joint entropy](#joint-entropy)
  - [Entropy monotonicity under independent addition](#entropy-monotonicity-under-independent-addition)
  - [Entropy function for a q-ary alphabet](#entropy-function-for-a-q-ary-alphabet)
  - [Information content](#information-content)
  - [Graph entropy](#graph-entropy)
  - [Entropy bound with one prescribed probability](#entropy-bound-with-one-prescribed-probability)
  - [Epsilon-sufficient set](#epsilon-sufficient-set)
    - [Minimum size of a sufficient set for an IID source](#minimum-size-of-a-sufficient-set-for-an-iid-source)
  - [Differential entropy](#differential-entropy)
    - [Differential entropy under an increasing transformation](#differential-entropy-under-an-increasing-transformation)
    - [Entropy power](#entropy-power)
      - [Entropy power inequality](#entropy-power-inequality)
        - [Multiplicative entropy power inequality](#multiplicative-entropy-power-inequality)
  - [Min-entropy](#min-entropy)
    - [Information entropy dominates min-entropy](#information-entropy-dominates-min-entropy)
  - [Varentropy](#varentropy)
  - [Binary entropy](#binary-entropy)
  - [Chain rule for information entropy](#chain-rule-for-information-entropy)
  - [Subadditivity of information entropy](#subadditivity-of-information-entropy)
  - [Concavity of information entropy](#concavity-of-information-entropy)
  - [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)
    - [Maximum entropy on a finite alphabet](#maximum-entropy-on-a-finite-alphabet)
  - [Maximum entropy distribution on the nonnegative integers](#maximum-entropy-distribution-on-the-nonnegative-integers)
- [One-to-one source code](#one-to-one-source-code)
  - [Optimal one-to-one binary code](#optimal-one-to-one-binary-code)
- [Huffman coding](#huffman-coding)
  - [Huffman code](#huffman-code)
    - [Uniform-source Huffman length distribution](#uniform-source-huffman-length-distribution)
  - [Huffman sibling property](#huffman-sibling-property)
  - [Optimal prefix code](#optimal-prefix-code)
    - [Balancing exchange for a uniform optimal prefix code](#balancing-exchange-for-a-uniform-optimal-prefix-code)
    - [Expected codeword length](#expected-codeword-length)
    - [Probability monotonicity of optimal prefix-code lengths](#probability-monotonicity-of-optimal-prefix-code-lengths)
    - [Deepest sibling property of an optimal prefix code](#deepest-sibling-property-of-an-optimal-prefix-code)
    - [Nonunique optimal prefix code](#nonunique-optimal-prefix-code)
  - [Huffman codeword length bounds](#huffman-codeword-length-bounds)
- [Bernoulli source](#bernoulli-source)
- [Information rate](#information-rate)
  - [Reliable source encoding at a rate](#reliable-source-encoding-at-a-rate)
    - [Strong converse for fixed-rate source coding](#strong-converse-for-fixed-rate-source-coding)
  - [Information rate under fixed-length blocking](#information-rate-under-fixed-length-blocking)
- [Asymptotic equipartition property](#asymptotic-equipartition-property)
  - [Typical set](#typical-set)
    - [Typical sequence theorem](#typical-sequence-theorem)
    - [Weakly typical sequence](#weakly-typical-sequence)
    - [Typical-set cardinality bounds](#typical-set-cardinality-bounds)
      - [Minimal high-probability source-set exponent](#minimal-high-probability-source-set-exponent)
  - [Strongly typical sequence](#strongly-typical-sequence)
- [Lossless source coding](#lossless-source-coding)
  - [Code-distribution correspondence](#code-distribution-correspondence)
  - [Fixed-rate source-coding error exponent](#fixed-rate-source-coding-error-exponent)
- [Unicity distance](#unicity-distance)
  - [Key equivocation](#key-equivocation)
  - [Source redundancy in cryptanalysis](#source-redundancy-in-cryptanalysis)
  - [Infinite unicity distance from a source symmetry](#infinite-unicity-distance-from-a-source-symmetry)

## Bit

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bit)

A [bit](#bit) is a binary classical symbol with two distinguishable values, zero and one. A uniform random [bit](#bit) has one [bit](#bit) of [information entropy](#information-entropy), while a biased binary symbol has less. Sending one [bit](#bit) means transmitting one symbol from this binary alphabet; the [mutual information](#mutual-information) it carries about a particular input need not be one.

## Memoryless classical information source

↑ **Parent:** [Information theory](information-theory.md)

A memoryless classical source emits [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) from a fixed finite alphabet. Its block [probability mass function](probability-theory.md#probability-mass-function) factors as shown, and its information per symbol is the [Shannon entropy](#information-entropy) $H(U)=-\sum_up(u)\log_2p(u)$. Zero-probability symbols never occur and contribute zero to the entropy. The [typical sequence theorem](#typical-sequence-theorem) describes the size and probability of the high-probability block set used for reliable compression.

## Alphabet

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alphabet_(formal_languages))

An alphabet is a finite nonempty set of symbols from which strings or source outputs are formed.

## Conditional entropy

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_entropy)

For discrete random variables, conditional entropy is

$$
H(Y\mid X)=\sum_x\mathbb P(X=x)H(Y\mid X=x).
$$

### Equality in the entropy conditioning inequality

↑ **Parent:** [Conditional entropy](#conditional-entropy)

For [discrete random variables](random-variable.md#discrete-random-variable) with finite [information entropy](#information-entropy) $H(X)$, [Gibbs inequality](probability-and-statistics.md#gibbs-inequality) gives

$$
H(X)-H(X\mid Y)=\sum_y p_Y(y)D(p_{X\mid y}\Vert p_X)\geq0.
$$

Equality holds exactly when $X$ and $Y$ are [independent random variables](random-variable.md#independent-random-variables). Finiteness matters: if $A$ has infinite [information entropy](#information-entropy) and is independent of a fair bit $B$, then $X=(A,B)$ and $Y=B$ are dependent but $H(X)=H(X\mid Y)=+\infty$.

// Target: probability-and-statistics.bigb

### Chain rule for conditional entropy

↑ **Parent:** [Conditional entropy](#conditional-entropy)

For classical finite random variables, $H(X,Z\mid Y)=H(X\mid Y)+H(Z\mid X,Y)=H(Z\mid Y)+H(X\mid Z,Y)$. Each identity follows by inserting the corresponding joint entropy into $H(X,Z,Y)-H(Y)$. The two orders are particularly useful when one variable is a deterministic function of the others, as in [Fano's inequality via an error indicator](#fano-s-inequality-via-an-error-indicator).

### Conditional entropy under a deterministic change of variables

↑ **Parent:** [Conditional entropy](#conditional-entropy)

If $f(x,z)$ is a [bijection](function.md#bijection) of $x$ for every fixed $z$, then

$$
H(f(X,Z)\mid Z)=H(X\mid Z).
$$

In particular, translating a random variable in a finite group by a value determined by the conditioning variable does not change its conditional entropy.

### Conditioning reduces entropy

↑ **Parent:** [Conditional entropy](#conditional-entropy)

For discrete random variables, $H(U\mid V)\leq H(U)$, with equality exactly when $U$ and $V$ are [independent](random-variable.md#independent-random-variables).

<h3 id="fano-s-inequality">Fano's inequality</h3>

↑ **Parent:** [Conditional entropy](#conditional-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fano's_inequality)

Let $X$ take values in an alphabet of size $m$, let $\widehat X$ be an estimate determined by $Y$, and put $p_e=\mathbb P(\widehat X\ne X)$. Then

$$
H(X\mid Y)\leq h_2(p_e)+p_e\log_2(m-1),
$$

where $h_2$ is the [binary entropy function](combinatorics.md#binary-entropy-function). The error indicator costs at most $h_2(p_e)$ bits, and after an error there are at most $m-1$ possible values of $X$.

<h4 id="fano-s-inequality-via-an-error-indicator">Fano's inequality via an error indicator</h4>

↑ **Parent:** [Fano's inequality](#fano-s-inequality)

For a guess $f(Y)$ of a finite-alphabet variable $X$, let $Z=1_{X\ne f(Y)}$ and $p_e=P(Z=1)$. The [chain rule for conditional entropy](#chain-rule-for-conditional-entropy) gives $H(X\mid Y)=H(Z\mid Y)+H(X\mid Z,Y)$. The first term is at most the [binary entropy](#binary-entropy) $h(p_e)$. The second is zero when the guess is right and at most $\log_2(|J_X|-1)$ when it is wrong, proving $H(X\mid Y)\leq h(p_e)+p_e\log_2(|J_X|-1)$. This needs no optimality assumption on the guess.

#### List-decoding Fano inequality

↑ **Parent:** [Fano's inequality](#fano-s-inequality)

If a uniform index $J$ has $N$ possibilities and every proposed success neighbourhood contains at most $B<N$ possibilities, then any estimator has failure [probability](probability-theory.md#probability) at least the displayed expression. Condition on its success indicator: [conditional entropy](#conditional-entropy) is at most $\log2+(1-p_e)\log B+p_e\log N$. Subtract this from $\log N$ to bound the [mutual information](#mutual-information) and rearrange. A metric [Hamming ball](coding-theory.md#hamming-ball) gives approximate recovery rather than exact index decoding.

### Entropy of a sum of independent finite-group variables

↑ **Parent:** [Conditional entropy](#conditional-entropy)

If [independent random variables](random-variable.md#independent-random-variables) $X,Y$ take values in a [finite additive group](group.md#finite-additive-group), then

$$
H(X+Y)\geq\max\{H(X),H(Y)\}.
$$

Indeed, $H(X+Y)\geq H(X+Y\mid Y)=H(X)$, and symmetrically for $Y$. Independence is essential: taking $Y=-X$ makes the sum constant.

## Mutual information

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutual_information)

The mutual information between discrete random variables is

$$
I(X;Y)=H(Y)-H(Y\mid X)
=H(X)+H(Y)-H(X,Y).
$$

### Entropy submodularity

↑ **Parent:** [Mutual information](#mutual-information)

For discrete [random variables](random-variable.md) $X,Y,Z$,

$$
H(X,Y)+H(Y,Z)\geq H(Y)+H(X,Y,Z).
$$

The difference between the left- and right-hand sides is the nonnegative [conditional mutual information](#conditional-mutual-information) $I(X;Z\mid Y)$.

#### Compression of an entropy sum

↑ **Parent:** [Entropy submodularity](#entropy-submodularity)

A [union-intersection compression](extremal-set-theory.md#union-intersection-compression) can only decrease the sum of [information entropies](#information-entropy) $\sum_{A\in\mathcal A}H(X_A)$ for a finite-valued [random vector](random-variable.md#random-vector) $X$. Each elementary step follows from [entropy submodularity](#entropy-submodularity); iteration proves the assertion with [multiset](set.md#multiset) multiplicities. Uniform coordinate multiplicity gives [Shearer inequality](#shearer-s-inequality) by compressing to repeated full sets and empty sets.

<h5 id="balister-bollobas-entropy-inequality">Balister–Bollobás entropy inequality</h5>

↑ **Parent:** [Compression of an entropy sum](#compression-of-an-entropy-sum)

Let $\mathcal A$ be a finite multiset of subsets and let $r_i$ count its occurrences of coordinate $i$. Its nested compression consists of $L_j=\{i:r_i\geq j\}$. Then $\sum_jH(X_{L_j})\leq\sum_{A\in\mathcal A}H(X_A)$, by repeated [entropy submodularity](#entropy-submodularity). This is the compression formulation in [Balister and Bollobás, "Projections, Entropy and Sumsets"](https://arxiv.org/abs/0711.1151).

<h6 id="madiman-tetali-entropy-inequality">Madiman–Tetali entropy inequality</h6>

↑ **Parent:** [Balister–Bollobás entropy inequality](#balister-bollobas-entropy-inequality)

For a nonempty ordered coordinate set $A$, write $A^-=[\min A-1]$ and $A^+=[\max A-1]\setminus A$. An exact $k$-cover satisfies $\sum_AH(X_A\mid X_{A^+})\leq kH(X)\leq\sum_AH(X_A\mid X_{A^-})$. A short proof uses the [chain rule for information entropy](#chain-rule-for-information-entropy) contributions $h_i=H(X_i\mid X_{[i-1]})$: each conditional subset entropy bounds $\sum_{i\in A}h_i$ on the appropriate side, by [conditioning reduces entropy](#conditioning-reduces-entropy). Weighting gives the lower inequality for a fractional packing and the upper inequality for a fractional cover. See [Madiman and Tetali, "Information Inequalities for Joint Distributions"](https://arxiv.org/abs/0901.0044).

<h4 id="shearer-s-inequality">Shearer's inequality</h4>

↑ **Parent:** [Entropy submodularity](#entropy-submodularity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shearer's_inequality)

Let $X=(X_1,\ldots,X_n)$ be a discrete [random vector](random-variable.md#random-vector), and let $\mathcal S$ be a collection of subsets of $[n]$ in which every index occurs at least $r$ times. Then

$$
rH(X)\leq\sum_{S\in\mathcal S}H(X_S).
$$

Apply the [chain rule for information entropy](#chain-rule-for-information-entropy) to each projection $X_S$ and use [conditioning reduces entropy](#conditioning-reduces-entropy) to compare every term with the corresponding conditional entropy in the full chain rule.

##### Entropy bound for graphs with isolated-vertex-free intersections

↑ **Parent:** [Shearer's inequality](#shearer-s-inequality)

If every pair of [graphs](graph.md) in a family on $[n]$ has a [graph intersection](graph-theory.md#graph-intersection) without an [isolated vertex](graph-theory.md#isolated-vertex), the family has at most $2^{n(n-2)/2}$ members. At each [vertex](graph.md#vertex-graph-theory), its possible [graph neighbourhoods](graph-theory.md#graph-neighbourhood) form an [intersecting family](extremal-set-theory.md#intersecting-family), of size at most $2^{n-2}$. Every [edge](graph-theory.md#edge-of-a-graph) occurs in two such neighbourhood projections. [Shearer inequality](#shearer-s-inequality) bounds twice the full [information entropy](#information-entropy) by the sum of their [information entropies](#information-entropy).

### Conditional mutual information

↑ **Parent:** [Mutual information](#mutual-information)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_mutual_information)

Conditional mutual information is the average information shared by $X$ and $Y$ after $Z$ is known:

$$
I(X;Y\mid Z)=H(X\mid Z)-H(X\mid Y,Z)\geq0.
$$

### Chain rule for mutual information

↑ **Parent:** [Mutual information](#mutual-information)

The information supplied by two observations decomposes as

$$
I(X;Y_1,Y_2)=I(X;Y_1)+I(X;Y_2\mid Y_1).
$$

### Data processing inequality

↑ **Parent:** [Mutual information](#mutual-information)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_processing_inequality)

If $X\to Y\to Z$ is a [Markov chain](markov-process.md#markov-chain), then

$$
I(X;Z)\leq I(X;Y),
\qquad
I(X;Z)\leq I(Y;Z).
$$

Thus deterministic or randomized processing cannot increase the information shared with an unprocessed variable.

#### Conditional data-processing inequality

↑ **Parent:** [Data processing inequality](#data-processing-inequality)

If $X\to Y\to Z$ is a Markov chain conditionally on $W$, then

$$
I(X;Z\mid W)\leq I(X;Y\mid W).
$$

It follows by applying ordinary data processing inside every conditional distribution and averaging over $W$.

### Incremental information in a twofold binary repetition code

↑ **Parent:** [Mutual information](#mutual-information)

Send a uniform bit twice through independent binary symmetric channels of crossover probability $p$. The first received bit supplies $1-h_2(p)$ bits. Since the received bits disagree with probability $2p(1-p)$, the additional information in the second bit is

$$
h_2(2p(1-p))-h_2(p).
$$

## Entropic Ruzsa distance

↑ **Parent:** [Information theory](information-theory.md)

For finitely supported random variables $X,Y$ in a [finite additive group](group.md#finite-additive-group), let $X',Y'$ be independent variables with their respective marginal distributions. The entropic Ruzsa distance is

$$
d_R(X,Y)=H(X'-Y')-\frac12H(X')-\frac12H(Y').
$$

It is symmetric and nonnegative, but can have $d_R(X,X)>0$.

### Conditional entropic Ruzsa distance

↑ **Parent:** [Entropic Ruzsa distance](#entropic-ruzsa-distance)

For finitely supported random variables, the conditional entropic Ruzsa distance is

$$
d_R(X\mid U;Y\mid V)
=\sum_{u,v}\mathbb P(U=u)\mathbb P(V=v)
d_R(X\mid U=u,Y\mid V=v).
$$

Thus the two conditioning values are sampled independently. If only one variable is conditioned, write $d_R(X\mid U;Y)$.

#### Simultaneous conditional entropic Ruzsa distance

↑ **Parent:** [Conditional entropic Ruzsa distance](#conditional-entropic-ruzsa-distance)

The simultaneous conditional distance samples one value of the conditioning variable for both arguments:

$$
d_R(X;Y\mathbin\Vert U)
=\sum_u\mathbb P(U=u)d_R(X\mid U=u,Y\mid U=u).
$$

It differs in general from $d_R(X\mid U;Y\mid U)$, which uses two independently sampled conditioning values.

#### Conditioned entropic Ruzsa distance of a summand

↑ **Parent:** [Conditional entropic Ruzsa distance](#conditional-entropic-ruzsa-distance)

If $U,V,X$ are independent random variables in $\mathbb F_2^n$, then

$$
d_R(U\mid U+V;X)
\leq\frac12\bigl(d_R(U;X)+d_R(V;X)+d_R(U;V)\bigr).
$$

Indeed, [conditioning reduces entropy](#conditioning-reduces-entropy) and independence give

$$
d_R(U\mid U+V;X)
\leq H(U+X)-\frac12H(U)-\frac12H(V)
+\frac12H(U+V)-\frac12H(X).
$$

In $\mathbb F_2^n$, $V=U+(U+V)$, so [conditional entropy under a deterministic change of variables](#conditional-entropy-under-a-deterministic-change-of-variables) shows that the left-hand side is unchanged when $U$ and $V$ are exchanged. Averaging the displayed bound with its exchanged version gives the result.

### Entropic Ruzsa triangle inequality

↑ **Parent:** [Entropic Ruzsa distance](#entropic-ruzsa-distance)

The entropic Ruzsa distance satisfies

$$
d_R(X,Z)\leq d_R(X,Y)+d_R(Y,Z).
$$

For independent representatives this is equivalent to

$$
H(X-Z)+H(Y)\leq H(X-Y)+H(Y-Z).
$$

### Entropic Ruzsa sum-difference inequality

↑ **Parent:** [Entropic Ruzsa distance](#entropic-ruzsa-distance)

For finitely supported random variables,

$$
d_R(X,-Y)\leq3d_R(X,Y).
$$

Equivalently, independent $X,Y$ satisfy

$$
H(X+Y)+H(X)+H(Y)\leq3H(X-Y).
$$

<h3 id="entropic-balog-szemeredi-gowers-theorem">Entropic Balog-Szemerédi-Gowers theorem</h3>

↑ **Parent:** [Entropic Ruzsa distance](#entropic-ruzsa-distance)

For finitely supported random variables $A,B$ in an [abelian group](group.md#abelian-group),

$$
d_R(A;B\mathbin\Vert A+B)
\leq 3I(A;B)+2H(A+B)-H(A)-H(B).
$$

To prove it, take two conditionally independent copies $(A_1,B_1)$ and $(A_2,B_2)$ of $(A,B)$ given $A+B$. Since $A_1+B_1=A_2+B_2$, [entropy submodularity](#entropy-submodularity) gives

$$
H(A_1-B_2)
\leq H(A_1-B_2,A_1)+H(A_1-B_2,B_1)-H(A_1-B_2,A_1,B_1).
$$

The first two terms are at most $H(A)+H(B)$. The last joint entropy is

$$
2H(A,B)-H(A+B).
$$

Consequently $H(A_1-B_2)\leq H(A+B)+2I(A;B)$. Subtracting

$$
H(A\mid A+B)=H(B\mid A+B)
=H(A)+H(B)-I(A;B)-H(A+B)
$$

from this bound proves the theorem.

### C-relevant pair of random variables

↑ **Parent:** [Entropic Ruzsa distance](#entropic-ruzsa-distance)

A pair $(U,V)$ is $C$-relevant to $(X,Y)$ when

$$
d_R(U;X)+d_R(V;Y)\leq C d_R(X;Y).
$$

#### Relevance of independent self-sums

↑ **Parent:** [C-relevant pair of random variables](#c-relevant-pair-of-random-variables)

If $(U,V)$ is $C$-relevant to $(X,Y)$ and $U_1,U_2,V_1,V_2$ are mutually independent copies, then $(U_1+U_2,V_1+V_2)$ is $2C$-relevant to $(X,Y)$. The [entropy submodularity for three independent sums](#entropy-submodularity-for-three-independent-sums) implies

$$
d_R(U_1+U_2;X)
\leq\frac12\bigl(2d_R(U;X)+d_R(U;U)\bigr),
$$

and similarly for $V$. The [Entropic Ruzsa triangle inequality](#entropic-ruzsa-triangle-inequality) bounds

$$
d_R(U;U)\leq2d_R(U;X),
\qquad
d_R(V;V)\leq2d_R(V;Y),
$$

which proves the claim after addition.

## Entropy submodularity for three independent sums

↑ **Parent:** [Information theory](information-theory.md)

For independent finitely supported random variables $X,Y,Z$ in a [finite additive group](group.md#finite-additive-group),

$$
H(X+Y+Z)+H(Y)\leq H(X+Y)+H(Y+Z).
$$

This is the [data processing inequality for mutual information](#data-processing-inequality) applied to the [Markov chain](markov-process.md#markov-chain) $X\to X+Y\to X+Y+Z$.

## Entropy submodularity for sums

↑ **Parent:** [Information theory](information-theory.md)

For independent $U,V,V'$ with $V$ and $V'$ identically distributed,

$$
H(V+V')+H(U)\leq H(U+V)+H(U+V').
$$

This additive form of entropy submodularity follows from data processing and invariance of conditional entropy under translations.

## Binary hypothesis testing in information theory

↑ **Parent:** [Information theory](information-theory.md)

For two [probability mass functions](probability-theory.md#probability-mass-function) $P,Q$, a decision region $B_n$ accepts $P^{\otimes n}$. Its two error probabilities are $P^{\otimes n}(B_n^c)$ and $Q^{\otimes n}(B_n)$.

### Error exponents in hypothesis testing

↑ **Parent:** [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error_exponents_in_hypothesis_testing)

An error exponent is the limiting exponential decay rate of an error probability $p_n$ as sample size $n$ grows. Different constraints on the [Type I error](#type-i-and-type-ii-errors) and [Type II error](#type-i-and-type-ii-errors) give different optimal rates. The [Chernoff information](#chernoff-information) describes the optimal average-error rate for simple Bayesian hypotheses; [Stein's lemma](#stein-s-lemma-information-theory) gives the optimal type-II rate when type-I error is held below a fixed nontrivial bound.

### Type I and type II errors

↑ **Parent:** [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_I_and_type_II_errors)

For a null hypothesis $H_0$, a Type I error rejects $H_0$ when it is true, while a Type II error accepts $H_0$ when the alternative is true. If a test accepts $H_0$ on an event $A$, their conditional probabilities are $\alpha=P_0(A^c)$ and $\beta=P_1(A)$.

### Chernoff information

↑ **Parent:** [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chernoff_information)

The Chernoff information between $P$ and $Q$ is

$$
C(P,Q)=-\min_{0\leq s\leq1}\log\sum_xP(x)^sQ(x)^{1-s}.
$$

It is the optimal exponential error rate for Bayesian testing of two independent identically distributed simple hypotheses.

<h3 id="stein-s-lemma-information-theory">Stein's lemma (information theory)</h3>

↑ **Parent:** [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)

For distinct [probability distributions](probability-theory.md#probability-distribution) $P,Q$, the optimal [error exponents in hypothesis testing](#error-exponents-in-hypothesis-testing) give type-II error $Q^{\otimes n}(B_n)$ decay rate $D(P\Vert Q)$ among tests whose type-I error $P^{\otimes n}(B_n^c)$ stays below any fixed number in $(0,1)$.

### Neyman-Pearson decision region

↑ **Parent:** [Binary hypothesis testing in information theory](#binary-hypothesis-testing-in-information-theory)

The [Neyman-Pearson lemma](statistical-modelling.md#neyman-pearson-lemma) says that an optimal region accepting $P$ has the likelihood-ratio form

$$
B_n=\left\{x_1^n:\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}\geq t\right\},
$$

with possible randomization on the boundary.

## Total correlation

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_correlation)

The total correlation of a random vector is

$$
\operatorname{TC}(X_1,\ldots,X_n)
=\sum_iH(X_i)-H(X_1,\ldots,X_n)
=D\!\left(P_{X_1,\ldots,X_n}\middle\Vert\bigotimes_iP_{X_i}\right).
$$

It is nonnegative and vanishes exactly when the coordinates are independent.

## Type (information theory)

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_(information_theory))

The type, or [empirical distribution](#type-information-theory), of a finite string records the relative frequency of each symbol.

### Type class

↑ **Parent:** [Type (information theory)](#type-information-theory)

The type class $T(P)$ is the set of all strings of a fixed length whose [type](#type-information-theory) is $P$. Every string in one type class has the same probability under any independent identically distributed source law.

### Method of types

↑ **Parent:** [Type (information theory)](#type-information-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_types)

For a finite [alphabet](#alphabet) $A$, there are at most $(n+1)^{|A|}$ length-$n$ types, and under an [i.i.d.](random-variable.md#independent-and-identically-distributed-random-variables) law $P$ the probability of the type class $T_R$ is at most $2^{-nD(R\Vert P)}$ when logarithms use base two.

#### Sanov theorem

↑ **Parent:** [Method of types](#method-of-types)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sanov_theorem)

Sanov's theorem is the [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) for empirical distributions of independent identically distributed observations. On a finite alphabet with sampling law $Q$, its rate function is $D_e(R\Vert Q)$.

#### Information projection

↑ **Parent:** [Method of types](#method-of-types)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_projection)

An information projection of $Q$ onto a set $\mathcal C$ of [probability distributions](probability-theory.md#probability-distribution) minimizes $D(P\Vert Q)$ over $P\in\mathcal C$. For a closed [convex set](mathematical-optimization.md#convex-set) and suitable $Q$, it obeys the Pythagorean inequality

$$
D(P\Vert Q)\geq D(P\Vert P^*)+D(P^*\Vert Q).
$$

##### Entropy minimization under a prescribed sample mean

↑ **Parent:** [Information projection](#information-projection)

For positive probabilities $p_i$ on a finite alphabet with numerical values $a_i$, impose $\sum_iq_ia_i=m$. The [relative entropy](probability-and-statistics.md#kullback-leibler-divergence) is minimized by the displayed [exponential tilting](probability-theory.md#exponential-tilting), with $\theta$ chosen to give mean $m$. For any other feasible distribution $r$, direct substitution gives $D(r\Vert p)=D(r\Vert q)+\theta m-\log\sum_jp_je^{\theta a_j}$. [Relative entropy nonnegativity](probability-and-statistics.md#relative-entropy-nonnegativity) proves optimality and uniqueness. The [method of types](#method-of-types) makes this the typical empirical distribution conditioned on the rare sample-mean constraint, on the leading exponential scale.

## Rate-distortion function

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rate-distortion_function)

For source $X$ and distortion function $d(x,y)$, the rate-distortion function is

$$
R(D)=\inf_{P_{Y\mid X}:\,\mathbb E d(X,Y)\leq D}I(X;Y).
$$

### Hamming distortion

↑ **Parent:** [Rate-distortion function](#rate-distortion-function)

Hamming distortion is $d(x,y)=\mathbf1_{\{x\ne y\}}$, so its expected distortion is the symbol-error probability.

## Channel capacity

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Channel_capacity)

The capacity of a discrete memoryless channel is

$$
C=\max_{P_X}I(X;Y).
$$

### Weakly symmetric channel capacity

↑ **Parent:** [Channel capacity](#channel-capacity)

If every row of an $m$-output channel matrix is a permutation of every other row and all column sums agree, the uniform input achieves a uniform output and

$$
C=\log_2m-H(\text{one row}).
$$

#### Cyclic ternary channel capacity

↑ **Parent:** [Weakly symmetric channel capacity](#weakly-symmetric-channel-capacity)

A [discrete memoryless channel](coding-theory.md#discrete-memoryless-channel) on the additive [group](group.md) $\mathbb Z/3\mathbb Z$ maps $x$ to $x$ with [probability](probability-theory.md#probability) $1-q$ and to $x+1$ with [probability](probability-theory.md#probability) $q$. Every input gives the same [conditional entropy](#conditional-entropy) $h_2(q)$, whereas the output [Shannon entropy](#information-entropy) is at most $\log_2 3$. A uniform input produces a uniform output since every column of the transition [matrix](vector-space.md#matrix) sums to one. Hence the [channel capacity](#channel-capacity) is $\log_2 3-h_2(q)$ [bits](#bit) per use. This cyclic-error channel differs from a channel distributing its error probability equally over both other output symbols.

#### Binary symmetric channel capacity

↑ **Parent:** [Weakly symmetric channel capacity](#weakly-symmetric-channel-capacity)

A binary symmetric channel with crossover probability $p$ has capacity

$$
C=1-h_2(p)
$$

bits per channel use.

#### Ternary symmetric channel capacity

↑ **Parent:** [Weakly symmetric channel capacity](#weakly-symmetric-channel-capacity)

For diagonal transition probability $1-2\alpha$ and each off-diagonal probability $\alpha$,

$$
C=\log_2 3
 +(1-2\alpha)\log_2(1-2\alpha)
 +2\alpha\log_2\alpha,
$$

with $0\log 0=0$.

## Information entropy

↑ **Parent:** [Information theory](information-theory.md)

For a discrete random variable with probabilities $p_i$, its Shannon information entropy is

$$
H=-\sum_i p_i\log p_i.
$$

### Joint entropy

↑ **Parent:** [Information entropy](#information-entropy)

The [information entropy](#information-entropy) of the joint [probability distribution](probability-theory.md#probability-distribution) of a [random vector](random-variable.md#random-vector). For discrete variables it is $-\sum_{x_1,\ldots,x_n}p(x_1,\ldots,x_n)\log p(x_1,\ldots,x_n)$, with zero-mass terms omitted. Factoring joint probabilities into conditional probabilities gives the [chain rule for information entropy](#chain-rule-for-information-entropy), so joint entropy measures all coordinates together while accounting for their statistical dependence.

### Entropy monotonicity under independent addition

↑ **Parent:** [Information entropy](#information-entropy)

If $U,V$ are [independent random variables](random-variable.md#independent-random-variables) taking values in a countable additive group, conditioning on $V$ makes $U+V$ a translate of $U$. Consequently $H(U+V\mid V)=H(U)$, and [conditional entropy](#conditional-entropy) gives $H(U+V)\geq H(U)$. If the two [information entropies](#information-entropy) are finite, equality holds exactly when $U+V$ and $V$ are independent.

// Target: probability-and-statistics.bigb

### Entropy function for a q-ary alphabet

↑ **Parent:** [Information entropy](#information-entropy)

This is the entropy in base $q$ of the distribution with one symbol of probability $1-x$ and each of the other $q-1$ symbols of probability $x/(q-1)$. It increases on $[0,1-1/q]$ from zero to one, and governs the exponential volume of a [Hamming ball](coding-theory.md#hamming-ball). For $q=2$ it is the [binary entropy](#binary-entropy) function.

// Target: algebra.bigb

### Information content

↑ **Parent:** [Information entropy](#information-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_content)

The self-information of a positive-probability outcome is the negative logarithm of its probability. Independent outcomes have additive self-information. Its expectation is [Shannon entropy](#information-entropy).

// Target: probability-and-statistics.bigb

### Graph entropy

↑ **Parent:** [Information entropy](#information-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_entropy)

For a vertex law $P$ on a graph, choose $X\sim P$ and an [independent set](graph-theory.md#independent-set-graph-theory) valued random variable $Y$ containing $X$ almost surely. Minimize their [mutual information](#mutual-information) over all such joint laws. This defines graph entropy. It differs from the entropy of a proper coloring, because the random independent set need not be a deterministic color class.

### Entropy bound with one prescribed probability

↑ **Parent:** [Information entropy](#information-entropy)

If one probability in a $k$-point distribution equals $t$, normalize the remaining $k-1$ probabilities to $q$. Then $H=h(t)+(1-t)H(q)\leq h(t)+(1-t)\log_2(k-1)$. Equality for $t<1$ means that the remaining probabilities are equal. This combines the [binary entropy](#binary-entropy) of the distinguished event with the largest residual [Shannon entropy](#information-entropy).

### Epsilon-sufficient set

↑ **Parent:** [Information entropy](#information-entropy)

For a finite-valued [random variable](random-variable.md), an epsilon-sufficient set $S$ retains probability at least $1-\epsilon$. This notion is about covering probability mass and is unrelated to a [sufficient statistic](probability-and-statistics.md#sufficient-statistic). For an [IID random variable](random-variable.md#independent-and-identically-distributed-random-variables) source, any such set of words with fixed $\epsilon<1$ requires exponentially many words at a rate approaching the [Shannon entropy](#information-entropy).

#### Minimum size of a sufficient set for an IID source

↑ **Parent:** [Epsilon-sufficient set](#epsilon-sufficient-set)

For finite-alphabet [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), fixed $0\leq\epsilon<1$ and $\delta>0$, every [epsilon-sufficient set](#epsilon-sufficient-set) $S_n$ of length-$n$ words satisfies $|S_n|\geq(1-\epsilon)2^{n(H-\delta)}/2$ for sufficiently large $n$. Intersect $S_n$ with a [typical set](#typical-set) whose excluded mass is at most $(1-\epsilon)/2$. The intersection retains that much probability and each word has probability at most $2^{-n(H-\delta)}$.

### Differential entropy

↑ **Parent:** [Information entropy](#information-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_entropy)

The [differential entropy](#differential-entropy) of a [probability density function](continuous-probability-distribution.md#probability-density-function) is $-\mathbb E_q[\log q(X)]$ when this [expected value](probability-theory.md#expected-value) is defined. Unlike discrete [information entropy](#information-entropy), it can be negative and depends on the coordinates and reference [measure](measure-theory.md#measure). It is the entropy term in the [evidence lower bound](statistical-inference.md#evidence-lower-bound) for continuous [variational inference](statistical-inference.md#variational-inference).

#### Differential entropy under an increasing transformation

↑ **Parent:** [Differential entropy](#differential-entropy)

Let $g:\mathbb R\to\mathbb R$ have finite, strictly positive [derivative](calculus.md#derivative) everywhere. Its inverse is defined on its image, and [change of variables](calculus.md#change-of-variables-formula) gives $p_{g(X)}(g(x))=p_X(x)/g'(x)$. If $h(X)$ and $\mathbb E\log_2 g'(X)$ are finite, taking the expectation of the logarithm proves the displayed [differential entropy](#differential-entropy) identity.

// Target: probability-and-statistics.bigb

#### Entropy power

↑ **Parent:** [Differential entropy](#differential-entropy)

The [entropy power](#entropy-power) of an $n$-dimensional [random vector](random-variable.md#random-vector) with finite [differential entropy](#differential-entropy) in bits is the [variance](variance.md) per coordinate of an isotropic [Gaussian distribution](probability-theory.md#normal-distribution) with the same [differential entropy](#differential-entropy). The normalization makes $N(X)=\sigma^2$ when $X$ has [covariance matrix](variance.md#covariance-matrix) $\sigma^2I_n$.

// Target: probability-and-statistics.bigb

##### Entropy power inequality

↑ **Parent:** [Entropy power](#entropy-power)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_power_inequality)

For independent $n$-dimensional [random vectors](random-variable.md#random-vector) with densities and finite [differential entropies](#differential-entropy), the [entropy power inequality](#entropy-power-inequality) states

$$
2^{2h(X+Y)/n}\geq2^{2h(X)/n}+2^{2h(Y)/n}.
$$

The sum's [differential entropy](#differential-entropy) is required to be defined; a value $+\infty$ makes the inequality immediate. Equality for finite nondegenerate densities occurs for [Gaussian distributions](probability-theory.md#normal-distribution) with proportional [covariance matrices](variance.md#covariance-matrix).

// Target: probability-and-statistics.bigb

###### Multiplicative entropy power inequality

↑ **Parent:** [Entropy power inequality](#entropy-power-inequality)

For independent positive [random variables](random-variable.md) $Y_1,Y_2$ with densities, finite [differential entropies](#differential-entropy) and finite $\mu_i=\mathbb E\log_2Y_i$, applying the [entropy power inequality](#entropy-power-inequality) to $Z_i=\ln Y_i$ gives

$$
2^{2h(Y_1Y_2)}\geq2^{2\mu_2}2^{2h(Y_1)}+2^{2\mu_1}2^{2h(Y_2)}.
$$

Indeed $h(Z_i)=h(Y_i)-\mu_i$, while $h(Y_1Y_2)=h(Z_1+Z_2)+\mu_1+\mu_2$, provided the sum's [differential entropy](#differential-entropy) is defined. Positivity alone does not ensure these expressions exist: $Y=e^T$ with $T$ having [Cauchy distribution](probability-theory.md#cauchy-distribution) has undefined $\mathbb E\log_2Y$.

// Target: algebra.bigb

### Min-entropy

↑ **Parent:** [Information entropy](#information-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Min-entropy)

For a discrete random variable with largest point probability $p_{\max}$, its min-entropy is

$$
H_\infty(X)=-\log p_{\max}.
$$

#### Information entropy dominates min-entropy

↑ **Parent:** [Min-entropy](#min-entropy)

For a discrete random variable, $H(X)\geq H_\infty(X)$. Indeed, every point probability satisfies $p_x\leq p_{\max}$, so averaging $-\log p_x\geq-\log p_{\max}$ proves the inequality.

### Varentropy

↑ **Parent:** [Information entropy](#information-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Varentropy)

The varentropy of a discrete random variable with mass function $P$ is the variance of its information content:

$$
V_H(X)=\operatorname{Var}[-\log P(X)].
$$

### Binary entropy

↑ **Parent:** [Information entropy](#information-entropy)

The binary entropy function is

$$
h_2(p)=-p\log_2p-(1-p)\log_2(1-p).
$$

### Chain rule for information entropy

↑ **Parent:** [Information entropy](#information-entropy)

For discrete random variables,

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

Iterating gives $H(X_1,\ldots,X_n)=\sum_iH(X_i\mid X_1,\ldots,X_{i-1})$.

### Subadditivity of information entropy

↑ **Parent:** [Information entropy](#information-entropy)

The [chain rule for information entropy](#chain-rule-for-information-entropy) and [conditioning reduces entropy](#conditioning-reduces-entropy) give

$$
H(X,Y)\leq H(X)+H(Y),
$$

with equality exactly when $X$ and $Y$ are [independent](random-variable.md#independent-random-variables).

### Concavity of information entropy

↑ **Parent:** [Information entropy](#information-entropy)

For probability mass functions $P_1,\ldots,P_m$ and convex weights $\alpha_i$, information entropy satisfies

$$
H\!\left(\sum_i\alpha_iP_i\right)\geq\sum_i\alpha_iH(P_i).
$$

This follows from the [concavity](real-analysis.md#concave-function) of $-t\log t$.

### Maximum entropy distribution on a finite set

↑ **Parent:** [Information entropy](#information-entropy)

Among [probability distributions](probability-theory.md#probability-distribution) on a finite set of $m$ elements, the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) uniquely maximizes [information entropy](#information-entropy), attaining $\log m$.

#### Maximum entropy on a finite alphabet

↑ **Parent:** [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)

An [information entropy](#information-entropy) on at most $m$ outcomes is at most $\log_2m$, with equality for the uniform distribution on all $m$ outcomes. For the uniform reference $u$, the [Kullback-Leibler divergence](probability-and-statistics.md#kullback-leibler-divergence) is $D(p\|u)=\log_2m-H(p)\geq0$, proving the bound.

### Maximum entropy distribution on the nonnegative integers

↑ **Parent:** [Information entropy](#information-entropy)

Among distributions on $\{0,1,2,\ldots\}$ with fixed [expected value](probability-theory.md#expected-value) $\mu$, the [geometric distribution](discrete-probability-distribution.md#geometric-distribution) with success probability $1/(1+\mu)$ uniquely maximizes [information entropy](#information-entropy). Its entropy is

$$
(1+\mu)h_2\!\left(\frac1{1+\mu}\right).
$$

## One-to-one source code

↑ **Parent:** [Information theory](information-theory.md)

A one-to-one source code is an [injective function](algebra.md#injective-function) from source symbols to finite codewords. Unlike a [prefix code](coding-theory.md#prefix-code), it need not permit instantaneous decoding of concatenated codewords.

### Optimal one-to-one binary code

↑ **Parent:** [One-to-one source code](#one-to-one-source-code)

Order source symbols by decreasing probability and assign the $i$th symbol a binary word of length $\lfloor\log_2i\rfloor$. This minimizes expected length among one-to-one binary codes because the available shortest words are assigned to the most probable symbols.

## Huffman coding

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Huffman_coding)

Huffman's algorithm repeatedly combines the $D$ least weights for a $D$-ary prefix code and yields an optimal expected length.

### Huffman code

↑ **Parent:** [Huffman coding](#huffman-coding)

A Huffman code is a [prefix code](coding-theory.md#prefix-code) produced by repeatedly merging the two least probable symbols or subtrees. Reversing the merges builds a [binary tree](computer-science.md#binary-tree) whose leaf depths are the codeword lengths. It minimizes expected length among binary prefix codes.

// Target: algebra.bigb

#### Uniform-source Huffman length distribution

↑ **Parent:** [Huffman code](#huffman-code)

For $m\ge2$ equiprobable symbols, the maximum [codeword length](coding-theory.md#codeword-length) of a binary [Huffman code](#huffman-code) is $s=\lceil\log_2m\rceil$. Exactly $2^s-m$ codewords have length $s-1$ and $2m-2^s$ have length $s$. The [balancing exchange for a uniform optimal prefix code](#balancing-exchange-for-a-uniform-optimal-prefix-code) restricts the depths to these two levels; counting leaves and using equality in the [Kraft inequality](coding-theory.md#kraft-mcmillan-inequality) determine the numbers.

// Target: probability-and-statistics.bigb

### Huffman sibling property

↑ **Parent:** [Huffman coding](#huffman-coding)

Some optimal prefix tree places the two least probable symbols as sibling leaves of maximum depth, which is the inductive basis of Huffman's algorithm.

### Optimal prefix code

↑ **Parent:** [Huffman coding](#huffman-coding)

An optimal prefix code minimizes probability-weighted codeword length among all prefix codes for the source.

#### Balancing exchange for a uniform optimal prefix code

↑ **Parent:** [Optimal prefix code](#optimal-prefix-code)

For an equiprobable source, an optimal binary prefix tree has leaf depths differing by at most one. If one leaf has depth $t$ and a deepest sibling pair has depth $s\ge t+2$, split the shallow leaf into two children and collapse the deep pair into its parent. The number of leaves is unchanged and their total depth decreases by $s-t-1>0$, contradicting optimality.

// Target: probability-and-statistics.bigb

#### Expected codeword length

↑ **Parent:** [Optimal prefix code](#optimal-prefix-code)

For a source symbol $X$ and a code $c$, the expected codeword length is

$$
L(c)=\mathbb E[|c(X)|]=\sum_xP(X=x)|c(x)|.
$$

#### Probability monotonicity of optimal prefix-code lengths

↑ **Parent:** [Optimal prefix code](#optimal-prefix-code)

If symbols of probabilities $p_i>p_j$ have codeword lengths $l_i$ and $l_j$ in an optimal prefix code, then $l_i\leq l_j$. Otherwise, exchanging their codewords preserves the prefix property and changes the expected length by

$$
(p_i-p_j)(l_j-l_i)<0,
$$

contradicting optimality.

#### Deepest sibling property of an optimal prefix code

↑ **Parent:** [Optimal prefix code](#optimal-prefix-code)

Every optimal binary prefix code has two codewords of maximal length that differ only in their final bit. Indeed, choose a deepest leaf in the prefix tree. If its sibling were not a codeword, maximality of the depth would make that sibling subtree empty, so the chosen word could be shortened by deleting its final bit. This would preserve prefix-freeness and reduce expected length.

#### Nonunique optimal prefix code

↑ **Parent:** [Optimal prefix code](#optimal-prefix-code)

Distinct tree shapes can have the same minimum expected length, particularly when Huffman merges have ties.

### Huffman codeword length bounds

↑ **Parent:** [Huffman coding](#huffman-coding)

For a largest binary-symbol probability $p_1$, $p_1<1/3$ prevents a length-one word, while $p_1>2/5$ forces one in a Huffman tree.

## Bernoulli source

↑ **Parent:** [Information theory](information-theory.md)

A Bernoulli information source emits [independent symbols with one fixed probability distribution](random-variable.md#independent-and-identically-distributed-random-variables).

## Information rate

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_rate)

The information rate is the limiting entropy per emitted symbol, when that limit exists.

### Reliable source encoding at a rate

↑ **Parent:** [Information rate](#information-rate)

A source is reliably encodable at rate $r$ if there are block encoders with at most $2^{nr}$ outputs and corresponding decoders whose probability of reconstructing the first $n$ source symbols incorrectly tends to zero as $n\to\infty$.

#### Strong converse for fixed-rate source coding

↑ **Parent:** [Reliable source encoding at a rate](#reliable-source-encoding-at-a-rate)

For a finite-alphabet IID source of entropy $H$, fixed-length block codes of rate $R<H$ have reconstruction success probability tending to zero. At most $2^{nR}$ strings can be correctly reconstructed. Their typical probability is at most $2^{nR}2^{-n(H-\delta)}$, and the atypical probability tends to zero; choose $0<\delta<H-R$.

// Target: algebra.bigb

### Information rate under fixed-length blocking

↑ **Parent:** [Information rate](#information-rate)

For a source $(X_n)$ and fixed positive integer $N$, form the block source $Y_i=(X_{(i-1)N+1},\ldots,X_{iN})$. Whenever the original information rate $h$ exists, the blocked source has information rate $Nh$, because

$$
\frac1mH(Y_1,\ldots,Y_m)
=N\frac1{mN}H(X_1,\ldots,X_{mN}).
$$

## Asymptotic equipartition property

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_equipartition_property)

For a stationary source, typical long blocks have probability approximately $2^{-nH}$; equivalently normalized self-information converges to the entropy rate.

### Typical set

↑ **Parent:** [Asymptotic equipartition property](#asymptotic-equipartition-property)

For an IID source, the epsilon-typical set consists of words $u^n$ satisfying $|-(1/n)\log p(u^n)-H(U)|\leq\varepsilon$. Its probability tends to one, and its cardinality is at most $2^{n(H(U)+\varepsilon)}$.

#### Typical sequence theorem

↑ **Parent:** [Typical set](#typical-set)

For a [memoryless classical information source](#memoryless-classical-information-source), the [typical set](#typical-set) consists of positive-probability words with $|-(1/n)\log_2p(u^n)-H(U)|\leq\varepsilon$. The [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) applied to $-\log_2p(U_j)$ proves its probability tends to one. Every typical word has probability between $2^{-n(H+\varepsilon)}$ and $2^{-n(H-\varepsilon)}$. Summing the lower bound gives the displayed cardinality upper bound; if the set has probability at least $1-\delta$, summing the upper bound gives cardinality at least $(1-\delta)2^{n(H-\varepsilon)}$.

To compress at any rate $R>H(U)$, choose $0<\varepsilon<R-H(U)$, assign one fixed-length binary index to each typical word, and reserve one additional index for all atypical words. At most $\lceil nR\rceil$ bits suffice for all large $n$. Decoding inverts the typical-word indices and makes an arbitrary output for the reserved index. The reconstruction error is at most the probability of the atypical set and tends to zero.

#### Weakly typical sequence

↑ **Parent:** [Typical set](#typical-set)

For an [IID random variable](random-variable.md#independent-and-identically-distributed-random-variables) source with [probability mass function](probability-theory.md#probability-mass-function) $p$, a word $x^n$ is weakly typical when $|-(1/n)\log_2p(x^n)-H(X)|\leq\varepsilon$. It has probability on the scale $2^{-nH(X)}$. The [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) makes the [typical set](#typical-set) probable, but does not make every word in it representative: for a uniform source every possible word is weakly typical.

#### Typical-set cardinality bounds

↑ **Parent:** [Typical set](#typical-set)

For a [typical set](#typical-set) of probability at least $1-\delta$,

$$
(1-\delta)2^{n(H-\varepsilon)}\leq|T_\varepsilon^{(n)}|\leq2^{n(H+\varepsilon)}.
$$

The upper bound sums the lower probability bound for each word; the lower bound sums the upper probability bound and uses the set's total probability. These bounds turn the [asymptotic equipartition property](#asymptotic-equipartition-property) into exponential estimates of source-coding dimension.

##### Minimal high-probability source-set exponent

↑ **Parent:** [Typical-set cardinality bounds](#typical-set-cardinality-bounds)

For a finite-alphabet IID source and fixed $0<\varepsilon<1$, the smallest set of length-$n$ strings carrying probability at least $1-\varepsilon$ has size $2^{n(H(U)+o(1))}$. The [typical set](#typical-set) bounds give the upper estimate. For the lower estimate, any such set intersects the typical set in probability bounded away from zero, while each typical string has probability at most $2^{-n(H(U)-\delta)}$.

// Target: probability-and-statistics.bigb

### Strongly typical sequence

↑ **Parent:** [Asymptotic equipartition property](#asymptotic-equipartition-property)

For a finite-alphabet [IID random variable](random-variable.md#independent-and-identically-distributed-random-variables) source, a strongly typical word has empirical symbol frequencies within the chosen tolerance of every $p(x)$, and contains no zero-probability symbols. Unlike a [weakly typical sequence](#weakly-typical-sequence), this definition controls the individual symbol counts. Both definitions give sets whose probability tends to one for fixed positive tolerance.

## Lossless source coding

↑ **Parent:** [Information theory](information-theory.md)

[Lossless source coding](#lossless-source-coding) encodes source messages so they can be recovered exactly. [Shannon's source coding theorem](coding-theory.md#shannon-s-source-coding-theorem) relates its achievable average code length to [information entropy](#information-entropy).

### Code-distribution correspondence

↑ **Parent:** [Lossless source coding](#lossless-source-coding)

Lengths of a binary prefix code satisfy $K=\sum_x2^{-L(x)}\leq1$ and therefore define the probability mass function $R(x)=2^{-L(x)}/K$. Conversely, a mass function gives ideal lengths $-\log_2R(x)$ and integer prefix lengths after rounding.

### Fixed-rate source-coding error exponent

↑ **Parent:** [Lossless source coding](#lossless-source-coding)

For an IID finite-alphabet source $Q$ encoded at rate $R>H(Q)$, the optimal block error probability has exponential rate

$$
\min_{P:H(P)\geq R}D(P\Vert Q).
$$

## Unicity distance

↑ **Parent:** [Information theory](information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unicity_distance)

Unicity distance is the ciphertext length at which key equivocation reaches zero and the key becomes uniquely determined under the source model.

### Key equivocation

↑ **Parent:** [Unicity distance](#unicity-distance)

Key equivocation is the conditional entropy $H(K\mid C^n)$ remaining about a key after observing $n$ ciphertext symbols.

### Source redundancy in cryptanalysis

↑ **Parent:** [Unicity distance](#unicity-distance)

For ciphertext alphabet $\Sigma$ and source entropy $H$, each symbol has redundancy $\log|\Sigma|-H$, leading in Shannon's ideal model to $U=\log|K|/(\log|\Sigma|-H)$.

### Infinite unicity distance from a source symmetry

↑ **Parent:** [Unicity distance](#unicity-distance)

If distinct keys transform every ciphertext into equally probable plaintexts through a probability-preserving source symmetry, key equivocation never vanishes and unicity distance is infinite.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
