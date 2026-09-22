# Representation theory of the symmetric group

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Representation_theory_of_the_symmetric_group)

The representation theory of $S_n$ is organized by a [partition of an integer](#partition-of-an-integer). Over the complex numbers, partitions label the irreducible Specht modules; over positive-characteristic fields, the simple modules are labelled by regular partitions.

**Table of contents**

- [Induction ring of symmetric-group characters](#induction-ring-of-symmetric-group-characters)
- [Symmetric-group characters are integer-valued](#symmetric-group-characters-are-integer-valued)
- [Young subgroup](#young-subgroup)
- [Skew representation of a symmetric group](#skew-representation-of-a-symmetric-group)
- [Deletion projection for a symmetric group](#deletion-projection-for-a-symmetric-group)
- [Gelfand–Tsetlin algebra](#gelfand-tsetlin-algebra)
  - [Jucys–Murphy element](#jucys-murphy-element)
    - [Jucys–Murphy description of the center of a symmetric-group algebra](#jucys-murphy-description-of-the-center-of-a-symmetric-group-algebra)
    - [Cycle-sum identity for Young–Jucys–Murphy elements](#cycle-sum-identity-for-young-jucys-murphy-elements)
    - [Local spectral rules for Young–Jucys–Murphy elements](#local-spectral-rules-for-young-jucys-murphy-elements)
    - [Olshanskii centralizer lemma](#olshanskii-centralizer-lemma)
  - [Gelfand–Tsetlin basis](#gelfand-tsetlin-basis)
    - [Young seminormal form](#young-seminormal-form)
      - [Young orthogonal form](#young-orthogonal-form)
- [Sign representation](#sign-representation)
- [Tensor identity for an induced character](#tensor-identity-for-an-induced-character)
  - [Prime-degree irreducible Kronecker product criterion for a symmetric group](#prime-degree-irreducible-kronecker-product-criterion-for-a-symmetric-group)
  - [Induced-tensor decomposition for the symmetric group on four points](#induced-tensor-decomposition-for-the-symmetric-group-on-four-points)
- [Partition of an integer](#partition-of-an-integer)
  - [Reverse lexicographic order on partitions](#reverse-lexicographic-order-on-partitions)
  - [Glaisher partition bijection](#glaisher-partition-bijection)
  - [Dictionary order on integer partitions](#dictionary-order-on-integer-partitions)
  - [Young's lattice](#young-s-lattice)
    - [Young branching graph](#young-branching-graph)
      - [Oscillating path in the Young lattice](#oscillating-path-in-the-young-lattice)
  - [Generating function for partitions with bounded parts](#generating-function-for-partitions-with-bounded-parts)
  - [Self-conjugate partition and distinct odd parts](#self-conjugate-partition-and-distinct-odd-parts)
  - [Young diagram](#young-diagram)
    - [Skew Young diagram](#skew-young-diagram)
      - [Standard skew Young tableau](#standard-skew-young-tableau)
        - [Standard skew tableau determinant](#standard-skew-tableau-determinant)
      - [Horizontal strip](#horizontal-strip)
      - [Totally disconnected skew Young diagram](#totally-disconnected-skew-young-diagram)
    - [Hook partition](#hook-partition)
    - [Addable node of a Young diagram](#addable-node-of-a-young-diagram)
    - [Removable node of a Young diagram](#removable-node-of-a-young-diagram)
    - [Conjugate partition](#conjugate-partition)
    - [Hook of a Young diagram](#hook-of-a-young-diagram)
      - [Hook length](#hook-length)
        - [Hook graph of a partition](#hook-graph-of-a-partition)
          - [Hook product of a partition](#hook-product-of-a-partition)
      - [Hook-interval decomposition at a Young-diagram cell](#hook-interval-decomposition-at-a-young-diagram-cell)
      - [Divisor closure of hook lengths](#divisor-closure-of-hook-lengths)
      - [Rim hook](#rim-hook)
        - [Border-strip tableau](#border-strip-tableau)
    - [Content of a Young-diagram cell](#content-of-a-young-diagram-cell)
    - [Principal hook lengths of a partition](#principal-hook-lengths-of-a-partition)
  - [Beta set of a partition](#beta-set-of-a-partition)
    - [Beta number of a partition](#beta-number-of-a-partition)
    - [Beta-set hook-product identity](#beta-set-hook-product-identity)
      - [Square-sum identity for shifted partition coordinates](#square-sum-identity-for-shifted-partition-coordinates)
    - [Hook criterion in a beta set](#hook-criterion-in-a-beta-set)
    - [Abacus of a partition](#abacus-of-a-partition)
      - [Core-quotient bijection for partitions](#core-quotient-bijection-for-partitions)
      - [Core of a partition](#core-of-a-partition)
        - [Weight of a partition](#weight-of-a-partition)
        - [Odd-minus-even hook count of a partition](#odd-minus-even-hook-count-of-a-partition)
      - [Quotient of a partition](#quotient-of-a-partition)
        - [Hooks divisible by the abacus modulus](#hooks-divisible-by-the-abacus-modulus)
      - [Quotient tower of a partition](#quotient-tower-of-a-partition)
        - [Four-quotient of the partition three-one](#four-quotient-of-the-partition-three-one)
        - [Two-quotient tower of the partition three-one](#two-quotient-tower-of-the-partition-three-one)
        - [Iterated quotient equals a power quotient up to permutation](#iterated-quotient-equals-a-power-quotient-up-to-permutation)
      - [Core tower of a partition](#core-tower-of-a-partition)
        - [Power-core truncation of a prime-core tower](#power-core-truncation-of-a-prime-core-tower)
        - [P-adic valuation of a symmetric-group character degree from the core tower](#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower)
          - [Character degree coprime to p from the core tower](#character-degree-coprime-to-p-from-the-core-tower)
          - [Character-degree valuation does not increase on taking the p-core](#character-degree-valuation-does-not-increase-on-taking-the-p-core)
      - [Residue content of a partition](#residue-content-of-a-partition)
  - [Young tableau](#young-tableau)
    - [Young symmetrizer](#young-symmetrizer)
      - [Row-column collision lemma](#row-column-collision-lemma)
    - [Robinson–Schensted correspondence](#robinson-schensted-correspondence)
      - [Robinson-Schensted-Knuth correspondence](#robinson-schensted-knuth-correspondence)
        - [RSK growth-diagram local rule](#rsk-growth-diagram-local-rule)
          - [Trace and odd columns in symmetric RSK](#trace-and-odd-columns-in-symmetric-rsk)
      - [Dual Robinson–Schensted–Knuth correspondence](#dual-robinson-schensted-knuth-correspondence)
    - [Row insertion](#row-insertion)
      - [Row-insertion bumping-path monotonicity](#row-insertion-bumping-path-monotonicity)
    - [Near Young tableau](#near-young-tableau)
    - [Standard Young tableau](#standard-young-tableau)
      - [Column-reading order of standard Young tableaux](#column-reading-order-of-standard-young-tableaux)
        - [Triangular vanishing of Young-symmetrizer products](#triangular-vanishing-of-young-symmetrizer-products)
      - [Admissible adjacent swap of a standard Young tableau](#admissible-adjacent-swap-of-a-standard-young-tableau)
      - [Content vector of a standard Young tableau](#content-vector-of-a-standard-young-tableau)
        - [Axial distance in a Young tableau](#axial-distance-in-a-young-tableau)
    - [Semistandard Young tableau](#semistandard-young-tableau)
      - [Bender-Knuth involution](#bender-knuth-involution)
      - [Lattice word](#lattice-word)
    - [Row and column stabilizers of a Young tableau](#row-and-column-stabilizers-of-a-young-tableau)
    - [Tabloid](#tabloid)
      - [Young permutation module](#young-permutation-module)
        - [Character of a Young permutation module](#character-of-a-young-permutation-module)
        - [Signed Young permutation module](#signed-young-permutation-module)
        - [Young's rule](#young-s-rule)
          - [Vershik linear relations](#vershik-linear-relations)
          - [Two-row Young permutation module decomposition](#two-row-young-permutation-module-decomposition)
          - [Kostka number](#kostka-number)
        - [Specht filtration of the ordered-pair permutation module](#specht-filtration-of-the-ordered-pair-permutation-module)
      - [Polytabloid](#polytabloid)
        - [Column antisymmetrizer of a Young tableau](#column-antisymmetrizer-of-a-young-tableau)
          - [Dominance from a nonzero column antisymmetrizer](#dominance-from-a-nonzero-column-antisymmetrizer)
          - [Nonzero column antisymmetrizer criterion](#nonzero-column-antisymmetrizer-criterion)
        - [Specht module](#specht-module)
          - [Standard polytabloid basis](#standard-polytabloid-basis)
            - [Garnir relation](#garnir-relation)
          - [Semistandard homomorphism theorem](#semistandard-homomorphism-theorem)
          - [Kernel intersection theorem for Specht modules](#kernel-intersection-theorem-for-specht-modules)
            - [Invariant vector criterion for a Specht module](#invariant-vector-criterion-for-a-specht-module)
          - [Alternating-group restriction of Specht modules](#alternating-group-restriction-of-specht-modules)
            - [Smallest non-linear ordinary degree of an alternating group](#smallest-non-linear-ordinary-degree-of-an-alternating-group)
          - [Generalized Specht module](#generalized-specht-module)
            - [Pair of partitions for a generalized Specht module](#pair-of-partitions-for-a-generalized-specht-module)
              - [Good-letter matching in a tableau word](#good-letter-matching-in-a-tableau-word)
          - [Specht filtration](#specht-filtration)
            - [Littlewood–Richardson rule](#littlewood-richardson-rule)
              - [Littlewood–Richardson coefficient](#littlewood-richardson-coefficient)
              - [Pieri rule](#pieri-rule)
          - [Specht modules as minimal left ideals](#specht-modules-as-minimal-left-ideals)
          - [James submodule theorem](#james-submodule-theorem)
          - [Conjugate Specht module as a sign-twisted dual](#conjugate-specht-module-as-a-sign-twisted-dual)
          - [Restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group)
            - [Standard-character multiplicity in a Specht self-product](#standard-character-multiplicity-in-a-specht-self-product)
          - [Linear independence of standard polytabloids](#linear-independence-of-standard-polytabloids)
          - [Hook-length formula](#hook-length-formula)
            - [Least non-linear ordinary degree of a symmetric group](#least-non-linear-ordinary-degree-of-a-symmetric-group)
            - [Trace computation of Specht module dimension](#trace-computation-of-specht-module-dimension)
            - [Determinant formula for Specht module dimension](#determinant-formula-for-specht-module-dimension)
            - [Greene–Nijenhuis–Wilf hook walk](#greene-nijenhuis-wilf-hook-walk)
              - [Hook walk terminal probability](#hook-walk-terminal-probability)
          - [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)
            - [Power-sum border-strip multiplication](#power-sum-border-strip-multiplication)
              - [Staircase Schur functions use only odd power sums](#staircase-schur-functions-use-only-odd-power-sums)
            - [Maximal p-hook character formula](#maximal-p-hook-character-formula)
            - [Sign of an abacus hook-removal sequence](#sign-of-an-abacus-hook-removal-sequence)
            - [Two-row alternating character cancellation](#two-row-alternating-character-cancellation)
            - [Principal-hook character value of a symmetric group](#principal-hook-character-value-of-a-symmetric-group)
            - [Staircase-character vanishing criterion](#staircase-character-vanishing-criterion)
            - [Conjugate Specht character](#conjugate-specht-character)
            - [Straightening of a symmetric-group character indexed by a composition](#straightening-of-a-symmetric-group-character-indexed-by-a-composition)
          - [Modular Specht module](#modular-specht-module)
            - [Tabloid bilinear form](#tabloid-bilinear-form)
            - [Regular partition](#regular-partition)
              - [Regular label of the modular sign representation](#regular-label-of-the-modular-sign-representation)
              - [Simple symmetric-group module from a regular partition](#simple-symmetric-group-module-from-a-regular-partition)
                - [Absolute irreducibility of the Specht radical quotient](#absolute-irreducibility-of-the-specht-radical-quotient)
              - [Endomorphism theorem for a regular Specht module](#endomorphism-theorem-for-a-regular-specht-module)
  - [Dominance order on partitions](#dominance-order-on-partitions)
    - [Single-box up-move](#single-box-up-move)
- [Brauer defect-zero vanishing theorem](#brauer-defect-zero-vanishing-theorem)
- [Symmetric-group character co-degree vanishing criterion](#symmetric-group-character-co-degree-vanishing-criterion)

## Induction ring of symmetric-group characters

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

The graded abelian group $\bigoplus_{n\ge0}R(S_n)$ of ordinary virtual [characters](representation-theory.md#character-of-a-representation) has product $\chi\star\psi=\operatorname{Ind}_{S_m\times S_n}^{S_{m+n}}(\chi\boxtimes\psi)$ for degrees $m,n$. Its unit is the trivial degree-zero character. Associativity follows by transitivity of [induced representations](representation-theory.md#induced-representation) through the three-factor Young subgroup; commutativity follows by conjugating the block positions. The [Frobenius characteristic map](combinatorics.md#frobenius-characteristic-map) identifies this ring with the ring of [symmetric functions](combinatorics.md#symmetric-function), sending irreducible Specht characters to [Schur functions](combinatorics.md#schur-polynomial). This product is different from pointwise multiplication of characters of the same symmetric group.

## Symmetric-group characters are integer-valued

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

The character of a [Young permutation module](#young-permutation-module) counts fixed [tabloids](#tabloid) and is integer-valued. [Dominance order on partitions](#dominance-order-on-partitions) makes its decomposition into [Specht modules](#specht-module) triangular with diagonal multiplicity one. Descending induction in any order refining dominance therefore expresses each irreducible Specht character as an integer combination of permutation characters, proving integrality.

## Young subgroup

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

For a composition $\lambda$ of $n$, a Young subgroup permutes independently the blocks of a set partition of $\{1,\ldots,n\}$ with sizes $\lambda_i$, and is isomorphic to $S_{\lambda_1}\times\cdots\times S_{\lambda_r}$. Reordering the block sizes gives a conjugate subgroup. Inducing its [trivial representation](representation-theory.md#trivial-representation) gives a [Young permutation module](#young-permutation-module).

## Skew representation of a symmetric group

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

For $|\lambda|=n$, $|\mu|=m$, and $k=n-m$, define

$$
V^{\lambda/\mu}=\operatorname{Hom}_{S_m}(V^\mu,\operatorname{Res}^{S_n}_{S_m}V^\lambda).
$$

The copy of $S_k$ acting on the last $k$ letters commutes with $S_m$ and acts on this multiplicity space. Iterated [restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group) supplies a basis indexed by [standard skew Young tableaux](#standard-skew-young-tableau). Every such basis vector is a [cyclic vector for a group representation](representation-theory.md#cyclic-vector-for-a-group-representation): admissible swaps connect all tableaux, and their off-diagonal coefficients in the [Young orthogonal form](#young-orthogonal-form) are nonzero.

## Deletion projection for a symmetric group

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

Delete $n$ from the cycle notation of a [permutation](combinatorics.md#permutation) in $S_n$ to obtain a permutation in $S_{n-1}$. Extend this set map linearly to $\Pi_n:\mathbb C S_n\to\mathbb C S_{n-1}$. It is an $S_{n-1}$-bimodule map and the identity on $\mathbb C S_{n-1}$, but is not in general an algebra homomorphism. In particular,

$$
\Pi_n(X_n)=(n-1)1,\qquad \Pi_n(X_n^2)=(n-1)1+2\sum_{i<j<n}(i\ j).
$$

For $n\geq5$ it is the unique bimodule-equivariant set map $S_n\to S_{n-1}$; at $n=4$ another such map exists because $C_{S_3}(S_2)=S_2$.

<h2 id="gelfand-tsetlin-algebra">Gelfand–Tsetlin algebra</h2>

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

For the chain $S_0\subset\cdots\subset S_n$, the Gelfand–Tsetlin algebra in $\mathbb C S_n$ is generated by the centers of $\mathbb C S_r$ for $0\leq r\leq n$. [Multiplicity-free restriction](representation-theory.md#multiplicity-free-restriction) makes its joint eigenspaces one-dimensional in each [irreducible representation](representation-theory.md#irreducible-representation). Products of the central [primitive idempotents](commutative-algebra.md#primitive-idempotent) along restriction paths give its minimal projections. Thus it is a [maximal commutative subalgebra](associative-algebra.md#maximal-commutative-subalgebra) and a [semisimple algebra](associative-algebra.md#semisimple-algebra), isomorphic to a finite product of copies of $\mathbb C$.

<h3 id="jucys-murphy-element">Jucys–Murphy element</h3>

↑ **Parent:** [Gelfand–Tsetlin algebra](#gelfand-tsetlin-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jucys–Murphy_element)

In the [group algebra](associative-algebra.md#group-algebra) $\mathbb C S_n$, set

$$
X_1=0,\qquad X_r=\sum_{j<r}(j\ r).
$$

These elements commute: for each triple $a<i<j$, the only overlapping contributions cancel as $[(a\ i),(i\ j)+(a\ j)]=0$. They generate the [Gelfand–Tsetlin algebra](#gelfand-tsetlin-algebra), and on a [standard Young tableau](#standard-young-tableau) vector $X_r$ acts by the [Content of a Young-diagram cell](#content-of-a-young-diagram-cell) containing $r$.

<h4 id="jucys-murphy-description-of-the-center-of-a-symmetric-group-algebra">Jucys–Murphy description of the center of a symmetric-group algebra</h4>

↑ **Parent:** [Jucys–Murphy element](#jucys-murphy-element)

The [Young–Jucys–Murphy elements](#jucys-murphy-element) commute, and [symmetric polynomials](polynomial.md#symmetric-polynomial) in them are central. The full center theorem holds integrally as well as over [fields](algebra.md#field), so it survives modular reduction. On an ordinary [Specht module](#specht-module), the scalar of such a [polynomial](polynomial.md) is its value on the cell-content multiset. The integral generation step is stronger than knowing this description only over a characteristic-zero [field](algebra.md#field) and is essential in the modular block argument.

<h4 id="cycle-sum-identity-for-young-jucys-murphy-elements">Cycle-sum identity for Young–Jucys–Murphy elements</h4>

↑ **Parent:** [Jucys–Murphy element](#jucys-murphy-element)

In the [group algebra](associative-algebra.md#group-algebra) of $S_n$, the product of the [Young–Jucys–Murphy elements](#jucys-murphy-element) $X_2,\ldots,X_n$ is the sum of all $n$-cycles, each with coefficient one. To prove it, multiply the sum of all $m$-cycles by $X_{m+1}$. Right multiplication by $(j\ m+1)$ inserts $m+1$ immediately after $j$ in the cycle. Every $(m+1)$-cycle has a unique predecessor of $m+1$, so deletion inverts this insertion bijectively. Induction starts at $X_2=(1\ 2)$. The identity turns a product of cell contents into a [central character value of a conjugacy-class sum](representation-theory.md#central-character-value-of-a-conjugacy-class-sum).

<h4 id="local-spectral-rules-for-young-jucys-murphy-elements">Local spectral rules for Young–Jucys–Murphy elements</h4>

↑ **Parent:** [Jucys–Murphy element](#jucys-murphy-element)

For the [joint spectrum](mathematics.md#joint-spectrum) of the [Young–Jucys–Murphy elements](#jucys-murphy-element), adjacent coordinates $a_i,a_{i+1}$ are distinct. If $a_{i+1}-a_i=\pm1$, the adjacent [transposition](combinatorics.md#transposition-permutation) $s_i$ acts on that line by $\pm1$. Otherwise interchanging the coordinates gives a spectral vector in the same [irreducible representation](representation-theory.md#irreducible-representation). These rules follow from $s_iX_is_i+s_i=X_{i+1}$ and its two-dimensional eigenspace calculation. Together with the [braid relation in a Coxeter group](lie-theory.md#braid-relation-in-a-coxeter-group), they exclude the consecutive patterns $(a,a\pm1,a)$.

#### Olshanskii centralizer lemma

↑ **Parent:** [Jucys–Murphy element](#jucys-murphy-element)

For the standard inclusion $S_{n-1}\subset S_n$, over the [complex numbers](complex-analysis.md#complex-number),

$$
C_{\mathbb C S_n}(\mathbb C S_{n-1})=\operatorname{alg}(Z(\mathbb C S_{n-1}),X_n).
$$

Here $X_n$ is a [Young–Jucys–Murphy element](#jucys-murphy-element). One way to see generation is to use [multiplicity-free restriction](representation-theory.md#multiplicity-free-restriction): a central idempotent of $S_{n-1}$ selects a preceding shape, and the distinct contents of its [addable nodes of a Young diagram](#addable-node-of-a-young-diagram) distinguish all possible succeeding shapes. Polynomial interpolation in $X_n$ supplies every diagonal projection in the [centralizer of a subalgebra](associative-algebra.md#centralizer-of-a-subalgebra).

<h3 id="gelfand-tsetlin-basis">Gelfand–Tsetlin basis</h3>

↑ **Parent:** [Gelfand–Tsetlin algebra](#gelfand-tsetlin-algebra)

Successively decompose an [irreducible representation](representation-theory.md#irreducible-representation) along a subgroup chain with [multiplicity-free restriction](representation-theory.md#multiplicity-free-restriction). A complete path selects a one-dimensional subspace; choosing one nonzero vector on each path gives a Gelfand–Tsetlin basis. For a [symmetric group](finite-group-theory.md#symmetric-group) over the [complex numbers](complex-analysis.md#complex-number), paths are [standard Young tableaux](#standard-young-tableau), and the [Young–Jucys–Murphy elements](#jucys-murphy-element) act diagonally with their cell contents.

#### Young seminormal form

↑ **Parent:** [Gelfand–Tsetlin basis](#gelfand-tsetlin-basis)

Let $T$ be a [standard Young tableau](#standard-young-tableau), $s_i=(i\ i+1)$, and $d=c_T(i+1)-c_T(i)$. A suitable [Gelfand–Tsetlin basis](#gelfand-tsetlin-basis) has, for an admissible pair $R=s_iT$ with tableau length increasing,

$$
s_iv_T=d^{-1}v_T+v_R,\qquad s_iv_R=(1-d^{-2})v_T-d^{-1}v_R.
$$

For a nonadmissible swap the scalar is $+1$ in a row and $-1$ in a column. The diagonal coefficient follows from the [Young–Jucys–Murphy element](#jucys-murphy-element) relation $s_iX_is_i+s_i=X_{i+1}$, and $s_i^2=1$ forces the product of off-diagonal coefficients. One global normalization is $v_T=P_T\pi_Tv_{T_0}$ from the row-reading tableau: a reduced admissible path makes this vector nonzero and gives coefficient one on every length-increasing edge.

##### Young orthogonal form

↑ **Parent:** [Young seminormal form](#young-seminormal-form)

Normalizing the tableau lines in a compatible real phase convention gives the [orthonormal basis](linear-algebra.md#orthonormal-basis) form

$$
s_i\big|_{\operatorname{span}(w_T,w_{s_iT})}
=\begin{pmatrix}d^{-1}&\sqrt{1-d^{-2}}\\\sqrt{1-d^{-2}}&-d^{-1}\end{pmatrix},
\qquad d=c_T(i+1)-c_T(i).
$$

Admissible swaps have $|d|\geq2$. Nonadmissible swaps act by $+1$ within a row and $-1$ within a column. The symmetric matrix is an orthogonal involution and is useful for making the [unitary representation](representation-theory.md#unitary-representation) and its phases explicit.

## Sign representation

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sign_representation)

The sign representation of $S_n$ is the one-dimensional representation in which a permutation acts by its sign. Tensoring a representation by it multiplies its character value at $g$ by $\operatorname{sgn}(g)$.

## Tensor identity for an induced character

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

For a subgroup $H\leq G$, a character $\chi$ of $G$ and a character $\phi$ of $H$,

$$
\chi\,\operatorname{Ind}_H^G\phi
=\operatorname{Ind}_H^G\bigl((\operatorname{Res}_H^G\chi)\phi\bigr).
$$

It follows directly from the induced-character formula because $\chi(g)=\chi(x^{-1}gx)$.

### Prime-degree irreducible Kronecker product criterion for a symmetric group

↑ **Parent:** [Tensor identity for an induced character](#tensor-identity-for-an-induced-character)

Let $n$ be prime. If the Kronecker product $\chi^\alpha\chi^\beta$ of two irreducible characters of $S_n$ is irreducible, then one of $\alpha,\beta$ is $(n)$ or $(1^n)$. Comparing the two self-products shows that only one may contain the standard character; the restriction branching rule then makes one partition rectangular, and primality makes that rectangle a single row or column.

### Induced-tensor decomposition for the symmetric group on four points

↑ **Parent:** [Tensor identity for an induced character](#tensor-identity-for-an-induced-character)

For the standard inclusions $S_2,S_3\leq S_4$,

$$
\left(S^{(2)}\!\uparrow_{S_2}^{S_4}\right)
\otimes
\left(S^{(1^3)}\!\uparrow_{S_3}^{S_4}\right)
\cong S^{(4)}\oplus5S^{(3,1)}\oplus4S^{(2,2)}\oplus7S^{(2,1,1)}\oplus3S^{(1^4)}.
$$

## Partition of an integer

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partition_of_an_integer)

A partition $\lambda\vdash n$ is a weakly decreasing sequence $\lambda_1\geq\lambda_2\geq\cdots\geq0$ with sum $n$.

### Reverse lexicographic order on partitions

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

Pad partitions with trailing zeros. In the descending-dictionary convention used for symmetric-function reverse lexicographic ordering, the partition with the larger first differing part precedes the other. This is the reverse of increasing [dictionary order on integer partitions](#dictionary-order-on-integer-partitions), and is a total order. It is distinct from comparing the last differing part in a [monomial](polynomial.md#monomial) reverse-lexicographic order.

### Glaisher partition bijection

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

Fix a prime $p$. Replace each part $p^a m$, with $p\nmid m$, by $p^a$ copies of $m$. This is a size-preserving bijection from [regular partitions](#regular-partition) to [partitions of an integer](#partition-of-an-integer) whose parts are not divisible by $p$. To invert it, write each multiplicity of a part $m$ not divisible by $p$ in base $p$ and use its digit in position $a$ as the multiplicity of $p^a m$. Every resulting multiplicity is below $p$. The bijection explains why the number of simple symmetric-group [modules](module-theory.md#module-mathematics) equals the number of [p-regular elements](representation-theory.md#p-regular-element)' [conjugacy classes](group-theory.md#conjugacy-class).

### Dictionary order on integer partitions

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

Pad partitions with trailing zeros and compare their first unequal parts. A partition is larger in [dictionary order on integer partitions](#dictionary-order-on-integer-partitions) when that first unequal part is larger. This is a total order, whereas [dominance order on partitions](#dominance-order-on-partitions) compares every prefix sum and is generally partial. The [row-column collision lemma](#row-column-collision-lemma) links these two orders.

<h3 id="young-s-lattice">Young's lattice</h3>

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young's_lattice)

The Young lattice is a [partially ordered set](set.md#partially-ordered-set) whose elements are integer partitions, including the empty partition. Each [partition of an integer](#partition-of-an-integer) is identified with its diagram, and the order is inclusion of [Young diagrams](#young-diagram). A cover adds exactly one box. A saturated path from the empty diagram to $\lambda$ is equivalent to a [standard Young tableau](#standard-young-tableau) of shape $\lambda$.

#### Young branching graph

↑ **Parent:** [Young's lattice](#young-s-lattice)

The Young branching graph is the graded cover graph of the [Young lattice](#young-s-lattice). Its level $n$ consists of partitions of $n$, and its edges add one box. It is also the branching graph for complex [Specht modules](#specht-module) under the [restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group).

##### Oscillating path in the Young lattice

↑ **Parent:** [Young branching graph](#young-branching-graph)

An oscillating tableau is a sequence of [Young diagrams](#young-diagram), each obtained from its predecessor by adding or removing one box. These are paths in the [Young branching graph](#young-branching-graph) with both directions allowed. A path of length $\ell$ from the empty diagram to $\lambda\vdash n$, with $\ell-n=2m\geq0$, has count $\ell!f_\lambda/(2^m n!m!)$. This differs from a saturated upward path, whose length must equal $n$.

### Generating function for partitions with bounded parts

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

The generating function for partitions whose parts are at most $e$ is

$$
\prod_{i=1}^e\frac1{1-x^i}.
$$

Conjugating Young diagrams shows that it also counts partitions with at most $e$ parts. Multiplication by $x^e$ gives the generating function for partitions with exactly $e$ positive parts.

### Self-conjugate partition and distinct odd parts

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

A self-conjugate partition is determined by the hook lengths of its diagonal cells. These are distinct odd positive integers, and every partition into distinct odd parts arises uniquely this way. Hence their generating function is

$$
\prod_{i=1}^\infty(1+x^{2i-1}).
$$

### Young diagram

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young_diagram)

The Young diagram of $\lambda$ is the set of cells $(i,j)$ with $1\leq j\leq\lambda_i$.

#### Skew Young diagram

↑ **Parent:** [Young diagram](#young-diagram)

For diagram inclusion $\mu\subseteq\lambda$, the skew Young diagram $\lambda/\mu$ consists of the cells of $\lambda$ outside $\mu$. Diagram inclusion is not the [dominance order on partitions](#dominance-order-on-partitions). Edge adjacency defines its connected components, and a connected skew diagram without a $2\times2$ square is a [rim hook](#rim-hook).

##### Standard skew Young tableau

↑ **Parent:** [Skew Young diagram](#skew-young-diagram)

A standard skew Young tableau fills the $k$ cells of a [skew Young diagram](#skew-young-diagram) bijectively with $1,\ldots,k$, increasing along each row and column. Equivalently it is a [linear extension of a partially ordered set](set.md#linear-extension) formed from the row and column inequalities. Interchanging consecutive labels preserves standardness exactly when their cells are incomparable in that partial order.

###### Standard skew tableau determinant

↑ **Parent:** [Standard skew Young tableau](#standard-skew-young-tableau)

Here $n=|\lambda|-|\mu|$, with zero entries for negative factorial arguments. Extract the squarefree [monomial](polynomial.md#monomial) $x_1\cdots x_n$ from the skew [Jacobi–Trudi identity](combinatorics.md#jacobi-trudi-identity). A product $h_{r_1}\cdots h_{r_\ell}$ contributes $n!/\prod r_i!$ because its distinct labels are assigned to the factors in that many ways. Summing [determinant](linear-algebra.md#determinant) signs proves the formula, since a squarefree [semistandard Young tableau](#semistandard-young-tableau) is a [standard skew Young tableau](#standard-skew-young-tableau).

##### Horizontal strip

↑ **Parent:** [Skew Young diagram](#skew-young-diagram)

A horizontal strip is a [skew Young diagram](#skew-young-diagram) containing at most one cell in each column. Equivalently, $\lambda/\mu$ is a horizontal strip when $\lambda_i\geq\mu_i\geq\lambda_{i+1}$ for all $i$. The multiplicity of the [trivial representation](representation-theory.md#trivial-representation) in the associated [skew representation of a symmetric group](#skew-representation-of-a-symmetric-group) is one for horizontal strips and zero otherwise. A column with two cells supplies a cyclic tableau vector on which an adjacent [transposition](combinatorics.md#transposition-permutation) acts by $-1$, excluding invariants.

##### Totally disconnected skew Young diagram

↑ **Parent:** [Skew Young diagram](#skew-young-diagram)

Under edge adjacency, a [skew Young diagram](#skew-young-diagram) is totally disconnected when every component has one cell. This means that no two cells share an edge. It is stronger than being a [horizontal strip](#horizontal-strip), which excludes repeated columns but permits adjacent cells in one row. The trivial-constituent criterion for a [skew representation of a symmetric group](#skew-representation-of-a-symmetric-group) concerns horizontal strips, not total disconnection in this sense.

#### Hook partition

↑ **Parent:** [Young diagram](#young-diagram)

A hook partition has shape $(n-k,1^k)$, $0\leq k\leq n-1$. Equivalently its [Young diagram](#young-diagram) has no cell $(2,2)$, so its only cell of content zero is $(1,1)$. Its [standard Young tableaux](#standard-young-tableau) are counted by $\binom{n-1}{k}$: choose the $k$ entries below the initial $1$, then the column and remaining row orders are forced.

#### Addable node of a Young diagram

↑ **Parent:** [Young diagram](#young-diagram)

An addable node is a cell outside a [Young diagram](#young-diagram) whose insertion leaves a Young diagram. Its left and upper predecessors, when present in the positive-coordinate grid, must already belong to the diagram. Different addable nodes have distinct [Young-diagram cell contents](#content-of-a-young-diagram-cell).

#### Removable node of a Young diagram

↑ **Parent:** [Young diagram](#young-diagram)

A removable node is a cell whose deletion leaves a [Young diagram](#young-diagram). The set $\lambda^-$ consists of the distinct partitions obtained by deleting one removable node from $\lambda$.

#### Conjugate partition

↑ **Parent:** [Young diagram](#young-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_partition)

The conjugate partition $\lambda'$ is obtained by reflecting the Young diagram across its main diagonal; thus $\lambda'_j$ is the number of parts of $\lambda$ at least $j$.

#### Hook of a Young diagram

↑ **Parent:** [Young diagram](#young-diagram)

The hook $H_{i,j}(\lambda)$ consists of $(i,j)$, the cells to its right in row $i$, and the cells below it in column $j$. Its hook length is

$$
h_{i,j}(\lambda)=\lambda_i-j+\lambda'_j-i+1.
$$

##### Hook length

↑ **Parent:** [Hook of a Young diagram](#hook-of-a-young-diagram)

The hook length of cell $(i,j)$ in the [Young diagram](#young-diagram) of a [partition of an integer](#partition-of-an-integer) $\lambda$ is the number of cells in its [Young-diagram hook](#hook-of-a-young-diagram):

$$
h_{i,j}(\lambda)=\lambda_i-j+\lambda'_j-i+1.
$$

Here $\lambda'$ is the [conjugate partition](#conjugate-partition). There is one hook length for every cell, so the [multiset](set.md#multiset) of hook lengths has [cardinality](set-theory.md#cardinality) $|\lambda|$.

###### Hook graph of a partition

↑ **Parent:** [Hook length](#hook-length)

The hook graph is the [Young diagram](#young-diagram) with the [hook length](#hook-length) written in each box. It displays the hook product and thus the [hook-length formula](#hook-length-formula) for the corresponding [Specht module](#specht-module). This use of the name is recorded in [Frame, Robinson and Thrall's original hook-graph paper](https://doi.org/10.4153/CJM-1954-030-1); it refers to a labeled array, not a directed hook-walk graph.

###### Hook product of a partition

↑ **Parent:** [Hook graph of a partition](#hook-graph-of-a-partition)

The product of all [hook lengths](#hook-length) in a [Young diagram](#young-diagram) is the denominator in the [hook-length formula](#hook-length-formula), and the scalar in the quasi-idempotence identity for its [Young symmetrizer](#young-symmetrizer).

##### Hook-interval decomposition at a Young-diagram cell

↑ **Parent:** [Hook of a Young diagram](#hook-of-a-young-diagram)

For $(i,j)\in Y(\lambda)$, the integers from one through $h_{i,j}$ split as the disjoint union

$$
\{h_{i,y}:j\leq y\leq\lambda_i\}
\sqcup
\{h_{i,j}-h_{x,j}:i<x\leq\lambda'_j\}.
$$

Tracing the southeast boundary of the hook records the first set at horizontal steps and the second at vertical steps.

##### Divisor closure of hook lengths

↑ **Parent:** [Hook of a Young diagram](#hook-of-a-young-diagram)

If a partition has a hook of length $ef$, it has a hook of length $e$. In a beta set, the first hook is a bead-gap pair at distance $ef$; along the arithmetic progression with step $e$, some consecutive pair changes from a bead to a gap.

##### Rim hook

↑ **Parent:** [Hook of a Young diagram](#hook-of-a-young-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rim_hook)

A rim hook, or border strip, is a connected skew Young diagram containing no $2\times2$ square. Its leg length is one less than its number of occupied rows.

###### Border-strip tableau

↑ **Parent:** [Rim hook](#rim-hook)

For a type $\alpha$, each successive difference is a [rim hook](#rim-hook) of size $\alpha_i$; zero parts give empty differences of height zero. Label its cells by $i$. Such fillings are weakly increasing along rows and columns, and the height is the sum of the occupied strips' numbers of rows minus one. Empty parts are omitted from the associated product of positive power sums; the finite-variable degree-zero power sum is not inserted.

#### Content of a Young-diagram cell

↑ **Parent:** [Young diagram](#young-diagram)

The content of the cell $(i,j)$ is $c_{i,j}=j-i$. Transposing the diagram negates every content and preserves every hook length.

#### Principal hook lengths of a partition

↑ **Parent:** [Young diagram](#young-diagram)

The principal hook lengths are $h_{1,1},h_{2,2},\ldots$ along the main diagonal. They are strictly decreasing positive integers, and their sum is the size of the partition.

### Beta set of a partition

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

For $m\geq\ell(\lambda)$, a beta set is

$$
\{\lambda_i+m-i:1\leq i\leq m\}.
$$

A hook of length $h$ corresponds to a bead $b$ and an empty position $b-h$; removing the hook moves the bead to that gap.

#### Beta number of a partition

↑ **Parent:** [Beta set of a partition](#beta-set-of-a-partition)

For a partition padded to $l$ rows, its [beta numbers](#beta-number-of-a-partition) are the distinct nonnegative integers $\lambda_i+l-i$. They are its occupied [abacus of a partition](#abacus-of-a-partition) positions. With exactly the positive row count, they equal the first-column [hook lengths](#hook-length); extra zero rows change the [representation](representation-theory.md#group-representation) of the [beta set](#beta-set-of-a-partition) while preserving the partition. Individual [beta numbers](#beta-number-of-a-partition) describe bead positions, whereas the [beta set](#beta-set-of-a-partition) is the collection of all these numbers.

#### Beta-set hook-product identity

↑ **Parent:** [Beta set of a partition](#beta-set-of-a-partition)

For $\ell_i=\lambda_i+m-i$, the hook lengths in row $i$ are $\ell_i-q$, where $q$ runs over the non-beta numbers in $[0,\ell_i-1]$. Their product is $\ell_i!/\prod_{k>i}(\ell_i-\ell_k)$. Multiplying over rows proves the identity and converts the [hook-length formula](#hook-length-formula) into a [Vandermonde determinant](galois-theory.md#vandermonde-determinant) divided by factorials. Padding the partition with zero rows changes the beta set but not the hook product.

##### Square-sum identity for shifted partition coordinates

↑ **Parent:** [Beta-set hook-product identity](#beta-set-hook-product-identity)

Repeated coordinates contribute zero. Sorting a distinct tuple and subtracting the staircase gives a partition of $m$, and its $m!$ orderings have identical squared summands. The [beta-set hook-product identity](#beta-set-hook-product-identity) turns each summand into $(\dim S^\lambda/m!)^2$. Summing and using the [Artin–Wedderburn theorem](associative-algebra.md#artin-wedderburn-theorem) for $\mathbb CS_m$ gives $m!\sum_{\lambda\vdash m}(\dim S^\lambda)^2/(m!)^2=1$. This is a normalized [group algebra](associative-algebra.md#group-algebra) dimension identity.

#### Hook criterion in a beta set

↑ **Parent:** [Beta set of a partition](#beta-set-of-a-partition)

Let $X=\{h_1,\ldots,h_m\}$ be a beta set and let $H_i(\lambda)$ be the hook lengths in row $i$. Then

$$
h\in H_i(\lambda)
\quad\Longleftrightarrow\quad
h_i-h\geq0\text{ and }h_i-h\notin X.
$$

Thus hooks are exactly bead-gap pairs on the partition abacus.

#### Abacus of a partition

↑ **Parent:** [Beta set of a partition](#beta-set-of-a-partition)

An $e$-runner abacus arranges the nonnegative integers by their residues modulo $e$ and places beads at the positions in a beta set. Moving a bead up one place on its runner removes an $e$-hook.

An abacus represents the [beta set of a partition](#beta-set-of-a-partition) by beads at integer positions. Positions with the same residue modulo the chosen runner count lie on one runner; moving a bead to an empty position above it represents the corresponding rim-hook removal.

##### Core-quotient bijection for partitions

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

Fix a positive integer $e$. A [partition of an integer](#partition-of-an-integer) is uniquely specified by its [core of a partition](#core-of-a-partition) for modulus $e$ and its ordered [quotient of a partition](#quotient-of-a-partition) for that modulus. More precisely, for every $e$-core $\gamma$ and ordered tuple $(\nu_0,\ldots,\nu_{e-1})$ of partitions, there is a unique partition $\lambda$ such that

$$
C_e(\lambda)=\gamma,\qquad Q_e(\lambda)=(\nu_0,\ldots,\nu_{e-1}),
\qquad |\lambda|=|\gamma|+e\sum_i|\nu_i|.
$$

The ordered runners use the usual [abacus of a partition](#abacus-of-a-partition) convention with a number of beads divisible by $e$. Adding $e$ beads preserves both the tuple and its runner labels. The core fixes the relative runner offsets, and each component partition fixes the displacement of the beads on that runner, giving existence and uniqueness.

##### Core of a partition

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

The $e$-core is obtained by repeatedly removing hooks of length $e$. On an $e$-runner abacus it is obtained by sliding every bead as high as possible, which proves independence of the order of removals.

###### Weight of a partition

↑ **Parent:** [Core of a partition](#core-of-a-partition)

The $e$-weight is the number of $e$-hooks removed to reach the $e$-core. It satisfies

$$
|\lambda|=|C_e(\lambda)|+e w_e(\lambda)
$$

and equals the total size of the partitions in the $e$-quotient.

###### Odd-minus-even hook count of a partition

↑ **Parent:** [Core of a partition](#core-of-a-partition)

Removing a rim hook of length two preserves the number of odd hook lengths minus the number of even hook lengths. If the 2-core is the staircase $(r,r-1,\ldots,1)$, every one of its $r(r+1)/2$ hooks is odd. Hence the difference for the original partition is

$$
\binom{r+1}{2}.
$$

##### Quotient of a partition

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

The $e$-quotient $Q_e(\lambda)=(\lambda^{(0)},\ldots,\lambda^{(e-1)})$ is the tuple of partitions represented by the individual runners after their positions are divided by $e$.

###### Hooks divisible by the abacus modulus

↑ **Parent:** [Quotient of a partition](#quotient-of-a-partition)

Hooks of $\lambda$ whose lengths are divisible by $e$ correspond bijectively to hooks in the $e$-quotient. A bead-gap pair on one runner with distance $eh$ becomes a bead-gap pair of distance $h$ in that runner partition, and hook removal commutes with this correspondence.

##### Quotient tower of a partition

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

The $e$-quotient tower recursively takes the $e$-quotient of every partition at the preceding level. For $e>1$, the sum of the sizes at each new level is at most $1/e$ times the preceding sum, so every partition has finite depth. For $e=1$, the quotient is the original partition and the tower has finite depth only for the empty partition.

###### Four-quotient of the partition three-one

↑ **Parent:** [Quotient tower of a partition](#quotient-tower-of-a-partition)

With runners ordered by residues $0,1,2,3$, an abacus for $(3,1)$ gives

$$
Q_4(3,1)=(\varnothing,\varnothing,(1),\varnothing).
$$

###### Two-quotient tower of the partition three-one

↑ **Parent:** [Quotient tower of a partition](#quotient-tower-of-a-partition)

The nonempty levels of the 2-quotient tower of $(3,1)$ are

$$
TQ_2(3,1)_0=((3,1)),\qquad
TQ_2(3,1)_1=((2),\varnothing),
$$

and

$$
TQ_2(3,1)_2=(\varnothing,(1),\varnothing,\varnothing).
$$

###### Iterated quotient equals a power quotient up to permutation

↑ **Parent:** [Quotient tower of a partition](#quotient-tower-of-a-partition)

For every $e,k\geq1$, the $e^k$-quotient $Q_{e^k}(\lambda)$ is a permutation of level $k$ of the $e$-quotient tower. Writing a runner residue modulo $e^k$ in base $e$ shows that taking one quotient chooses one digit at a time; iteration may reverse the order of those digits but selects the same runner partitions.

##### Core tower of a partition

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

The $p$-core tower places at level $r$ the $p$-cores of all partitions at level $r$ of the [quotient tower of a partition](#quotient-tower-of-a-partition). If $q_r$ is the sum of the sizes at quotient level $r$ and $c_r$ the sum at core level $r$, then

$$
q_r=c_r+p q_{r+1}.
$$

###### Power-core truncation of a prime-core tower

↑ **Parent:** [Core tower of a partition](#core-tower-of-a-partition)

For a [prime number](number-theory.md#prime-number) $p$, integer $k\geq1$, and $\gamma=C_{p^k}(\lambda)$, taking the $p^k$-[core of a partition](#core-of-a-partition) preserves the entries of the [core tower of a partition](#core-tower-of-a-partition) at levels $0,\ldots,k-1$ and makes every level at least $k$ empty. Also the [weight of a partition](#weight-of-a-partition) $w_{p^k}(\lambda)$ equals the total size at level $k$ of the [quotient tower of a partition](#quotient-tower-of-a-partition).

For the first claim, a removable [rim hook](#rim-hook) of length $p^k$ is a bead move by $p^k$ on the [abacus of a partition](#abacus-of-a-partition). It preserves the numbers of beads on the $p$ runners and hence the $p$-core. Under the [abacus divisible-hook correspondence](#hooks-divisible-by-the-abacus-modulus), it becomes removal of a $p^{k-1}$-hook in one quotient component; iteration preserves the cores at the next $k-1$ levels. After all $p^k$-hooks are removed, every component at quotient level $k$ is empty, so every higher core level is empty as well. The weight assertion follows from [iterated quotient equals a power quotient up to permutation](#iterated-quotient-equals-a-power-quotient-up-to-permutation) and the size formula for the [quotient of a partition](#quotient-of-a-partition).

###### P-adic valuation of a symmetric-group character degree from the core tower

↑ **Parent:** [Core tower of a partition](#core-tower-of-a-partition)

If $n=|\lambda|$ and $d_p(n)$ is its base-$p$ digit sum, then

$$
v_p(\chi^\lambda(1))
=\frac{\sum_{r\geq0}|TC_p(\lambda)_r|-d_p(n)}{p-1}.
$$

This combines the [Hook-length formula](#hook-length-formula), [Legendre formula](number-theory.md#legendre-s-formula), the [abacus divisible-hook correspondence](#hooks-divisible-by-the-abacus-modulus), and the recurrence $q_r=c_r+pq_{r+1}$.

###### Character degree coprime to p from the core tower

↑ **Parent:** [P-adic valuation of a symmetric-group character degree from the core tower](#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower)

Let $p$ be a [prime number](number-theory.md#prime-number), let $n=\sum_r\alpha_rp^r$ with $0\leq\alpha_r<p$, and let $c_r$ be the sum of partition sizes at level $r$ of the [core tower of a partition](#core-tower-of-a-partition) $\lambda\vdash n$. Then

$$
\boxed{p\nmid\chi^\lambda(1)\quad\Longleftrightarrow\quad c_r=\alpha_r\text{ for every }r.}
$$

Indeed $n=\sum_rc_rp^r$. Carrying $p$ units from position $r$ to position $r+1$ decreases $\sum_rc_r$ by $p-1$. Normalization to the base-$p$ digits therefore gives $\sum_rc_r\geq\sum_r\alpha_r$, with equality exactly when no carry is needed. The [P-adic valuation of a symmetric-group character degree from the core tower](#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower) is the difference divided by $p-1$.

###### Character-degree valuation does not increase on taking the p-core

↑ **Parent:** [P-adic valuation of a symmetric-group character degree from the core tower](#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower)

For every partition $\lambda$,

$$
v_p(\chi^\lambda(1))\geq v_p(\chi^{C_p(\lambda)}(1)).
$$

The core-tower formula reduces this to subadditivity of the base-$p$ digit sum across the sizes of the quotient partitions.

##### Residue content of a partition

↑ **Parent:** [Abacus of a partition](#abacus-of-a-partition)

The $e$-residue of a cell $(i,j)$ is $j-i$ modulo $e$, and the $e$-content is the multiset of cell residues. Removing an $e$-hook removes exactly one cell of each residue. Among partitions of a fixed size, two partitions have the same $e$-content exactly when they have the same $e$-core.

### Young tableau

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young_tableau)

A Young tableau of shape $\lambda$ is a bijective filling of the cells of its Young diagram by $1,\ldots,n$.

#### Young symmetrizer

↑ **Parent:** [Young tableau](#young-tableau)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young_symmetrizer)

For a [Young tableau](#young-tableau) $t$, let $r_t$ sum its row permutations and $c_t$ be the signed sum of its column permutations in the [group algebra](associative-algebra.md#group-algebra) of the [symmetric group](finite-group-theory.md#symmetric-group). The product $h_t=c_tr_t$ is a Young symmetrizer. The other order is another conventional realization. It satisfies $h_t^2=H_\lambda h_t$, where $H_\lambda$ is the [hook product of a partition](#hook-product-of-a-partition), so division by that scalar gives a primitive [idempotent](commutative-algebra.md#idempotent) in characteristic zero. Acting on a [tensor power](linear-algebra.md#tensor-power) constructs a [Schur module](lie-theory.md#schur-module).

##### Row-column collision lemma

↑ **Parent:** [Young symmetrizer](#young-symmetrizer)

If the rows of a [Young tableau](#young-tableau) of shape $\lambda$ have no repeated intersection with the columns of one of shape $\mu$, then $\sum_{i\leq k}\lambda_i\leq\sum_{i\leq k}\mu_i$ for every $k$. If also $\lambda\geq\mu$ in [dictionary order on integer partitions](#dictionary-order-on-integer-partitions), the shapes are equal. Saturation of the prefix bounds places one entry of each eligible row in each column, giving $u=rct$ with $r\in R(t)$ and $c\in C(t)$. A collision instead gives a [transposition](combinatorics.md#transposition-permutation) that makes row symmetrization followed by the relevant column antisymmetrization vanish.

<h4 id="robinson-schensted-correspondence">Robinson–Schensted correspondence</h4>

↑ **Parent:** [Young tableau](#young-tableau)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Robinson–Schensted_correspondence)

Insert the successive letters of a [permutation](combinatorics.md#permutation) by [row insertion](#row-insertion) to obtain an insertion tableau $P$, recording the insertion times in the new boxes of $Q$. This is a [bijection](function.md#bijection) between permutations and pairs of [standard Young tableaux](#standard-young-tableau) of a common shape. Reverse insertion removes the box marked by the latest recording time. The first row of $P$ has length equal to the [longest increasing subsequence](combinatorics.md#longest-increasing-subsequence).

##### Robinson-Schensted-Knuth correspondence

↑ **Parent:** [Robinson–Schensted correspondence](#robinson-schensted-correspondence)

List each pair $(i,j)$ with multiplicity $a_{ij}$, sorted first by $i$ and then by $j$. Apply [row insertion](#row-insertion) to the lower letters $j$, and record the upper letters $i$ in the new cells. The [row insertion](#row-insertion) comparison is strictly greater than the carried entry. The result is a pair of [Semistandard Young tableaux](#semistandard-young-tableau) of the same shape. Reverse insertion removes the rightmost cell containing the largest recording entry, then replaces the rightmost strictly smaller entry in each preceding row. It reconstructs the ordered list, proving the [bijection](function.md#bijection). The insertion and recording contents are respectively the column sums and row sums of $A$.

###### RSK growth-diagram local rule

↑ **Parent:** [Robinson-Schensted-Knuth correspondence](#robinson-schensted-knuth-correspondence)

At one [matrix](vector-space.md#matrix) entry $a$, let $\rho,\mu,\nu,\lambda$ be the shapes of the northwest, northeast, southwest and southeast [matrix](vector-space.md#matrix) prefixes under the [RSK correspondence](#robinson-schensted-knuth-correspondence). The displayed row-length recurrence expresses merged insertion paths: the new entry supplies the first-row carry, and the overlap of the two incoming row extensions beyond the northwest shape is bumped into the next row. Zero boundary shapes determine the whole diagram. Transposing the [matrix](vector-space.md#matrix) exchanges $\mu,\nu$, leaving the rule invariant.

###### Trace and odd columns in symmetric RSK

↑ **Parent:** [RSK growth-diagram local rule](#rsk-growth-diagram-local-rule)

For a symmetric nonnegative integer [matrix](vector-space.md#matrix), the two neighboring prefix shapes along the diagonal are equal. In the [RSK growth-diagram local rule](#rsk-growth-diagram-local-rule), set $\mu=\nu$ and take alternating sums of row lengths. The two occurrences of the alternating sum of $\mu$ cancel, leaving $o(\lambda)=o(\rho)+a_{ii}$. Induction along the diagonal proves the formula. Each column contributes one to this alternating sum exactly when its length is odd.

<h5 id="dual-robinson-schensted-knuth-correspondence">Dual Robinson–Schensted–Knuth correspondence</h5>

↑ **Parent:** [Robinson–Schensted correspondence](#robinson-schensted-correspondence)

For a finite $0$-$1$ matrix, list its occupied pairs by increasing top entry and decreasing bottom entry within a top-entry tie. Perform ordinary semistandard [row insertion](#row-insertion) on the bottom entries and record top entries in the new cells. The result is a [bijection](function.md#bijection) with same-shape tableaux $T,U$ for which $T$ and $U^t$ are [Semistandard Young tableaux](#semistandard-young-tableau). The types of $T$ and $U$ are respectively the column-sum and row-sum vectors of the matrix.

#### Row insertion

↑ **Parent:** [Young tableau](#young-tableau)

Insert $x$ into the first row of a [Young tableau](#young-tableau) by replacing its leftmost entry strictly greater than $x$, and carry the displaced entry into the next row. If no entry is greater, append $x$ and stop. The procedure preserves a [semistandard Young tableau](#semistandard-young-tableau); when all entries are distinct it preserves a [near Young tableau](#near-young-tableau). It underlies the [Robinson–Schensted correspondence](#robinson-schensted-correspondence).

##### Row-insertion bumping-path monotonicity

↑ **Parent:** [Row insertion](#row-insertion)

During [row insertion](#row-insertion) into a [near Young tableau](#near-young-tableau), the successive carried entries strictly increase while the columns in which they are bumped weakly decrease. Every old cell keeps its entry or receives a smaller one. These facts follow from increasing rows and strictly increasing columns.

#### Near Young tableau

↑ **Parent:** [Young tableau](#young-tableau)

A near Young tableau fills a [Young diagram](#young-diagram) with distinct entries from a totally ordered alphabet, increasing along rows and down columns. Its entries need not be the initial interval $1,\ldots,n$. It is the natural intermediate object for [row insertion](#row-insertion) of a new entry.

#### Standard Young tableau

↑ **Parent:** [Young tableau](#young-tableau)

A standard [Young tableau](#young-tableau) fills a [Young diagram](#young-diagram) bijectively with $1,\ldots,n$, increasing along rows and down columns. The cells occupied by the first $r$ entries form a diagram, so a tableau is equivalently a path formed by adjoining one [addable node of a Young diagram](#addable-node-of-a-young-diagram) at each step. The number of standard tableaux of shape $\lambda$ is the dimension of the complex [Specht module](#specht-module) $S^\lambda$.

##### Column-reading order of standard Young tableaux

↑ **Parent:** [Standard Young tableau](#standard-young-tableau)

Read each column from top to bottom, with columns ordered from left to right, and compare the resulting words lexicographically. With [Young symmetrizer](#young-symmetrizer) convention $h_t=c_tr_t$, this order gives [triangular vanishing of Young-symmetrizer products](#triangular-vanishing-of-young-symmetrizer-products). Changing the symmetrizer product convention requires a compatible order, rather than retaining a fixed vanishing direction automatically.

###### Triangular vanishing of Young-symmetrizer products

↑ **Parent:** [Column-reading order of standard Young tableaux](#column-reading-order-of-standard-young-tableaux)

For [standard tableaux](#standard-young-tableau) of the same shape and $h_t=c_tr_t$, $t>u$ in [column-reading order of standard Young tableaux](#column-reading-order-of-standard-young-tableaux) implies $h_th_u=0$. If there were no row-column collision, each column of $u$ would select one entry from each eligible row of $t$. Its sorted first column is componentwise at least the row minima of $t$; equality fixes those selected entries and permits induction after deleting the column. Thus no collision implies $u\geq t$. A collision gives $r_tc_u=0$.

##### Admissible adjacent swap of a standard Young tableau

↑ **Parent:** [Standard Young tableau](#standard-young-tableau)

Swapping consecutive labels $i,i+1$ preserves a [standard Young tableau](#standard-young-tableau) exactly when their cells are incomparable in the row-and-column order. Their contents then differ by more than one in absolute value. These admissible swaps connect all standard tableaux of any fixed shape, as adjacent swaps connect [linear extensions of a partially ordered set](set.md#linear-extension).

##### Content vector of a standard Young tableau

↑ **Parent:** [Standard Young tableau](#standard-young-tableau)

The content vector of a [standard Young tableau](#standard-young-tableau) $T$ is $(c_T(1),\ldots,c_T(n))$, where $c_T(r)$ is the [Content of a Young-diagram cell](#content-of-a-young-diagram-cell) containing $r$. Such vectors are exactly the integer vectors satisfying: the first coordinate is zero; each subsequent coordinate has an earlier neighbor differing by one; between two occurrences of $a$ both $a-1$ and $a+1$ occur. To reconstruct the tableau, insert each entry in the next available cell on its prescribed diagonal. The neighbor conditions supply its required predecessors, so each insertion is an [addable node of a Young diagram](#addable-node-of-a-young-diagram).

###### Axial distance in a Young tableau

↑ **Parent:** [Content vector of a standard Young tableau](#content-vector-of-a-standard-young-tableau)

The axial distance from label $j$ to label $i$ in a [standard Young tableau](#standard-young-tableau) is the difference of their [Young-diagram cell contents](#content-of-a-young-diagram-cell). This sign convention makes $c_T(r+1)-c_T(r)$ equal to $+1$ for consecutive entries in a row and $-1$ in a column. The reciprocal distance supplies the diagonal coefficient of [Young orthogonal form](#young-orthogonal-form).

#### Semistandard Young tableau

↑ **Parent:** [Young tableau](#young-tableau)

A semistandard Young tableau fills a [Young diagram](#young-diagram) with positive [integers](number-theory.md#integer), permitting repeated entries, so that entries weakly increase along rows and strictly increase down columns. Its content records the number of occurrences of each entry. The [Kostka number](#kostka-number) $K_{\lambda\mu}$ counts such fillings of shape $\lambda$ and content $\mu$.

##### Bender-Knuth involution

↑ **Parent:** [Semistandard Young tableau](#semistandard-young-tableau)

For adjacent letters $i,i+1$, pair entries in the same column and leave those pairs fixed. In each row, interchange the numbers of unpaired $i$ and $i+1$ entries, preserving their weak order. Strict columns are preserved: a letter that could obstruct a change from $i$ to $i+1$, or conversely, would already have been paired. Applying the operation twice restores the tableau. The paired letters contribute equal amounts to the two contents, so the involution swaps their total multiplicities.

##### Lattice word

↑ **Parent:** [Semistandard Young tableau](#semistandard-young-tableau)

A word in positive integers is a [lattice word](#lattice-word) if every initial segment has at least as many $i$'s as $(i+1)$'s for every $i$. This is the reading-word condition in the [Littlewood–Richardson rule](#littlewood-richardson-rule). Under [good-letter matching in a tableau word](#good-letter-matching-in-a-tableau-word), every letter of a [lattice word](#lattice-word) is good.

#### Row and column stabilizers of a Young tableau

↑ **Parent:** [Young tableau](#young-tableau)

The row stabilizer $R(t)$ permutes entries within each row, while the column stabilizer $C(t)$ permutes entries within each column. Their intersection is trivial.

#### Tabloid

↑ **Parent:** [Young tableau](#young-tableau)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tabloid)

A tabloid is an equivalence class of tableaux under permutations within rows. The tabloids of shape $\lambda$ form a transitive $S_n$-set.

##### Young permutation module

↑ **Parent:** [Tabloid](#tabloid)

The Young permutation module is the permutation module on the $\lambda$-tabloids.

###### Character of a Young permutation module

↑ **Parent:** [Young permutation module](#young-permutation-module)

A [tabloid](#tabloid) is fixed by a permutation exactly when each of its cycles lies wholly within one row. Assigning the distinct length-$q$ cycles to rows gives the displayed coefficient. More explicitly, sum $\prod_q m_q!/\prod_j a_{qj}!$ over nonnegative integers $a_{qj}$ with $\sum_j a_{qj}=m_q$ and $\sum_q q a_{qj}=\lambda_j$. Equal-length rows remain distinguished. Thus the [character](representation-theory.md#character-of-a-representation) counts fixed ordered row sets, rather than unordered set partitions.

###### Signed Young permutation module

↑ **Parent:** [Young permutation module](#young-permutation-module)

Over the [complex numbers](complex-analysis.md#complex-number), the signed Young permutation module is

$$
\widetilde M^\lambda=\operatorname{Ind}_{S_\lambda}^{S_n}\operatorname{sgn}
\cong\operatorname{sgn}\otimes M^\lambda.
$$

The isomorphism is the [tensor identity for induced representations](representation-theory.md#tensor-identity-for-induced-representations). The partition index is unchanged by this twist; conjugation instead changes the labels of its irreducible constituents. For the [conjugate partition](#conjugate-partition) $\lambda'$, the [character inner product](representation-theory.md#character-inner-product) of $M^\lambda$ and $\widetilde M^{\lambda'}$ is one: [Mackey restriction formula](representation-theory.md#mackey-restriction-formula) reduces it to the unique zero-one matrix with row margins $\lambda$ and column margins $\lambda'$.

<h6 id="young-s-rule">Young's rule</h6>

↑ **Parent:** [Young permutation module](#young-permutation-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young's_rule)

Over the complex numbers,

$$
M^\lambda\cong\bigoplus_{\alpha\vdash n}
(S^\alpha)^{\oplus K_{\alpha\lambda}},
$$

where the [Kostka number](#kostka-number) $K_{\alpha\lambda}$ counts semistandard tableaux of shape $\alpha$ and content $\lambda$. It is nonzero only when $\alpha$ dominates $\lambda$.

###### Vershik linear relations

↑ **Parent:** [Young's rule](#young-s-rule)

Let $M(\mu,\lambda)$ be the multiplicity of $V^\mu$ in the complex [Young permutation module](#young-permutation-module) $M^\lambda$. For $\lambda\vdash n$ and $\rho\vdash n-1$,

$$
\sum_{\mu:\rho\nearrow\mu}M(\mu,\lambda)
=\sum_{i:\lambda_i>0}M(\rho,\operatorname{sort}(\lambda-e_i)).
$$

Here $\nearrow$ means adding one cell, and zero parts are omitted. Equal row lengths contribute separately on the right. Restrict $M^\lambda$ to $S_{n-1}$ and separate the [tabloid](#tabloid) orbits by the row containing $n$ to obtain the right side. Decompose into irreducibles and use the [restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group) to obtain the left side. Equating multiplicities proves the formula.

###### Two-row Young permutation module decomposition

↑ **Parent:** [Young's rule](#young-s-rule)

For $0\leq k\leq n/2$, over the [complex numbers](complex-analysis.md#complex-number),

$$
\boxed{M^{(n-k,k)}\cong\bigoplus_{j=0}^k S^{(n-j,j)}.}
$$

By [Young's rule](#young-s-rule), the multiplicity is the [Kostka number](#kostka-number) for content $(n-k,k)$. A [semistandard Young tableau](#semistandard-young-tableau) on just the entries $1,2$ has at most two rows. For shape $(n-j,j)$, every lower entry is $2$ and every entry above it is $1$; the remaining top row is uniquely fixed by the content. Such a filling exists precisely for $j\leq k$. Thus each displayed [Specht module](#specht-module) occurs once. A zero second part is omitted.

###### Kostka number

↑ **Parent:** [Young's rule](#young-s-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kostka_number)

The Kostka number $K_{\alpha\lambda}$ is the number of semistandard Young tableaux of shape $\alpha$ and content $\lambda$: rows are weakly increasing and columns are strictly increasing.

###### Specht filtration of the ordered-pair permutation module

↑ **Parent:** [Young permutation module](#young-permutation-module)

For $n\geq4$, identify $M^{(n-2,1^2)}$ with the permutation module on ordered pairs $(i,j)$ with $i\ne j$. Let $p_1(i,j)=e_i$, $p_2(i,j)=e_j$, and $q(i,j)=\{i,j\}$. With $U=\ker p_1$ and $V=U\cap\ker p_2$, one has a Specht filtration

$$
0<S^{(n-2,1^2)}=\ker(q|_V)<V<U<\ker\varepsilon<M^{(n-2,1^2)}
$$

whose successive quotients are

$$
S^{(n-2,1^2)},\quad S^{(n-2,2)},\quad
S^{(n-1,1)},\quad S^{(n-1,1)},\quad S^{(n)}.
$$

The same construction for $n=3$ omits the zero $S^{(n-2,2)}$ factor.

##### Polytabloid

↑ **Parent:** [Tabloid](#tabloid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polytabloid)

For a tableau $t$, its polytabloid is

$$
e(t)=\sum_{\pi\in C(t)}\operatorname{sgn}(\pi)\{\pi t\}.
$$

###### Column antisymmetrizer of a Young tableau

↑ **Parent:** [Polytabloid](#polytabloid)

The column antisymmetrizer of a [Young tableau](#young-tableau) $t$ is the [group algebra](associative-algebra.md#group-algebra) element

$$
b_t=\sum_{g\in C(t)}\operatorname{sgn}(g)g.
$$

On the Young permutation module it has one-dimensional image $\mathbb F e(t)$.

###### Dominance from a nonzero column antisymmetrizer

↑ **Parent:** [Column antisymmetrizer of a Young tableau](#column-antisymmetrizer-of-a-young-tableau)

Let $t$ be a [Young tableau](#young-tableau) of shape $\lambda$, and let $u$ be a [Young tableau](#young-tableau) of shape $\mu$, both on $n$ entries. If the [Column antisymmetrizer of a Young tableau](#column-antisymmetrizer-of-a-young-tableau) $b_t$ satisfies $b_t\{u\}\ne0$ over any [field](algebra.md#field), then $\lambda$ dominates $\mu$ in the [dominance order on partitions](#dominance-order-on-partitions).

If two entries from one column of $t$ lie in the same row of $u$, their transposition fixes the [tabloid](#tabloid) $\{u\}$. Pairing terms of $b_t$ by this transposition gives $b_t\{u\}=0$, including in [characteristic](algebra.md#characteristic-of-a-field) two. Otherwise the first $r$ rows of $u$ contain at most $\min(r,\lambda'_j)$ entries from column $j$ of $t$. Thus

$$
\sum_{i=1}^r\mu_i\leq\sum_j\min(r,\lambda'_j)=\sum_{i=1}^r\lambda_i
$$

for every $r$, proving dominance.

###### Nonzero column antisymmetrizer criterion

↑ **Parent:** [Column antisymmetrizer of a Young tableau](#column-antisymmetrizer-of-a-young-tableau)

For tableaux $v,w$ of the same shape, $b_v\{w\}\ne0$ exactly when no row of $w$ contains two entries from one column of $v$. In that case a column permutation $h\in C(v)$ satisfies $h\{v\}=\{w\}$, and $b_v\{w\}=\pm e(v)$.

###### Specht module

↑ **Parent:** [Polytabloid](#polytabloid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Specht_module)

The Specht module $S^\lambda$ is the span of the polytabloids of shape $\lambda$. It is cyclic, generated by any one polytabloid, and over $\mathbb C$ it is irreducible.

###### Standard polytabloid basis

↑ **Parent:** [Specht module](#specht-module)

The [polytabloids](#polytabloid) $e_t$ indexed by [standard Young tableaux](#standard-young-tableau) of shape $\lambda$ form a basis of $S^\lambda$ over every [field](algebra.md#field), and a basis of its integral lattice over $\mathbb Z$. Column antisymmetry and [Garnir relations](#garnir-relation) straighten any [polytabloid](#polytabloid) into this set. Ordering leading [tabloids](#tabloid) by the rows containing successive entries makes the corresponding coefficient matrix triangular with diagonal entries one, proving independence. In particular the [dimension](vector-space.md#dimension-vector-space) is the standard-tableau count in every characteristic.

###### Garnir relation

↑ **Parent:** [Standard polytabloid basis](#standard-polytabloid-basis)

Take two adjacent columns of a numbered [Young tableau](#young-tableau), with a bottom segment $A$ of the left column and a top segment $B$ of the right column such that $|A|+|B|$ exceeds the height of the left column. Alternating over [permutations](combinatorics.md#permutation) of $A\cup B$, modulo [permutations](combinatorics.md#permutation) preserving $A$ and $B$ separately, gives a signed relation among [polytabloids](#polytabloid). The full alternation vanishes because each [tabloid](#tabloid) has two of these entries in one row. Solving for a nonstandard [polytabloid](#polytabloid) replaces its offending row inversion by earlier column-standard tableaux. The relation is proved over the free integral [tabloid](#tabloid) lattice, where cancellation and division by nonzero integer factors are valid; reduction then makes it valid in every characteristic. Together with column antisymmetry these relations give the [standard polytabloid basis](#standard-polytabloid-basis).

###### Semistandard homomorphism theorem

↑ **Parent:** [Specht module](#specht-module)

A filling $T$ of shape $\lambda$ and content $\alpha$ defines a [module homomorphism](module-theory.md#module-homomorphism) $\Theta_T:M^\lambda\to M^\alpha$: given a numbered tableau, sum over distinct assignments obtained by permuting $T$ within its rows, and put each numbered entry into output row $j$ when its assigned label is $j$. Restricting to $S^\lambda$ gives $\widehat\Theta_T$. For [Semistandard Young tableaux](#semistandard-young-tableau) $T$, these restrictions are linearly independent over every [field](algebra.md#field). They form a basis of $\operatorname{Hom}_{FS_n}(S^\lambda,M^\alpha)$ if the [characteristic of a field](algebra.md#characteristic-of-a-field) is not two, or if $\lambda$ is a two-regular [partition of an integer](#partition-of-an-integer). For two-singular shapes in [characteristic two](algebra.md#characteristic-two), they need not span. Column antisymmetrization and triangular leading [tabloids](#tabloid) establish independence; straightening the images of a cyclic [polytabloid](#polytabloid) establishes spanning under the stated hypotheses.

###### Kernel intersection theorem for Specht modules

↑ **Parent:** [Specht module](#specht-module)

For a [partition of an integer](#partition-of-an-integer) $\lambda$, let $\psi_{i,v}:M^\lambda\to M^{\lambda(i,v)}$ sum all [tabloids](#tabloid) obtained by retaining $v$ elements of row $i+1$ and moving its other $\lambda_{i+1}-v$ elements into row $i$, leaving the other row sets unchanged. Here $0\le v<\lambda_{i+1}$ and $\lambda(i,v)$ replaces $(\lambda_i,\lambda_{i+1})$ by $(\lambda_i+\lambda_{i+1}-v,v)$; [Young permutation modules](#young-permutation-module) are defined for compositions too. Then $S^\lambda=\bigcap_{i,v}\ker\psi_{i,v}$ over every [field](algebra.md#field). Pairwise column cancellation gives inclusion of the [Specht module](#specht-module) in each kernel. The reverse inclusion follows by straightening the [tabloid](#tabloid) coefficients using these adjacent-row relations: the remaining free leading coefficients are exactly those of the [standard polytabloid basis](#standard-polytabloid-basis).

###### Invariant vector criterion for a Specht module

↑ **Parent:** [Kernel intersection theorem for Specht modules](#kernel-intersection-theorem-for-specht-modules)

In positive [characteristic](algebra.md#characteristic-of-a-field) $p$, $(S^\lambda)^{S_n}$ is nonzero exactly when $\lambda_i\equiv-1\pmod{p^{t_i}}$ for every adjacent pair, where $t_i$ is least with $\lambda_{i+1}<p^{t_i}$. The only invariant line in $M^\lambda$ is generated by the sum $z_\lambda$ of all [tabloids](#tabloid). The map $\psi_{i,v}$ sends it to $\binom{\lambda_i+\lambda_{i+1}-v}{\lambda_i}z_{\lambda(i,v)}$. Thus the [kernel intersection theorem for Specht modules](#kernel-intersection-theorem-for-specht-modules) gives vanishing of $\binom{\lambda_i+j}{j}$ modulo $p$ for $1\le j\le\lambda_{i+1}$. By [Lucas's theorem](combinatorics.md#lucas-s-theorem), all these [binomial coefficients](combinatorics.md#binomial-coefficient) vanish exactly when the last $t_i$ base-$p$ digits of $\lambda_i$ are $p-1$.

###### Alternating-group restriction of Specht modules

↑ **Parent:** [Specht module](#specht-module)

An ordinary [Specht module](#specht-module) of non-self-conjugate shape stays [irreducible](representation-theory.md#irreducible-representation) on the [alternating group](finite-group-theory.md#alternating-group), and conjugate shapes give the same restriction. A self-conjugate shape splits into two [irreducibles](representation-theory.md#irreducible-representation) of equal degree, interchanged by an odd [permutation](combinatorics.md#permutation). The index-two inner-product identity is $\langle\chi^\lambda\downarrow,\chi^\mu\downarrow\rangle=\delta_{\lambda\mu}+\delta_{\lambda'\mu}$, and [Frobenius reciprocity](representation-theory.md#frobenius-reciprocity) proves exhaustion. The statement applies for $n\ge2$; $A_1$ is trivial.

###### Smallest non-linear ordinary degree of an alternating group

↑ **Parent:** [Alternating-group restriction of Specht modules](#alternating-group-restriction-of-specht-modules)

For $A_n$, the least non-linear ordinary degree is $3$ at $n=4,5$ and $n-1$ for $n\ge6$. For $n\le3$ no non-linear [irreducible](representation-theory.md#irreducible-representation) exists. The degree-$n-1$ [representation](representation-theory.md#group-representation) is unique for $n\ge2$, except $n=3$ where it does not exist and $n=6$ where two distinct degree-five [irreducibles](representation-theory.md#irreducible-representation) occur. The proof uses tableau branching to bound the degrees of nonstandard shapes and of the half-degree constituents of self-conjugate shapes, with the small cases checked by the [hook-length formula](#hook-length-formula).

###### Generalized Specht module

↑ **Parent:** [Specht module](#specht-module)

For a row composition $b$ and a weakly decreasing marking $a$ with $0\le a_i\le b_i$, mark the first $a_i$ cells of each row. Antisymmetrize within the marked columns and span the resulting [polytabloids](#polytabloid) in the [Young permutation module](#young-permutation-module) $M^b$. This gives $S^{a,b}$; $S^{0,b}=M^b$ and $S^{b,b}=S^b$ for a proper partition $b$. Its characteristic-independent [Specht filtration](#specht-filtration) is obtained by successively marking a cell or raising an unmarked row tail, with column-cancellation maps and the good-letter counting recursion.

###### Pair of partitions for a generalized Specht module

↑ **Parent:** [Generalized Specht module](#generalized-specht-module)

The first component is a proper partition marking an initial segment of each row of the second component. The second component may be a composition rather than a decreasing partition. This convention specifies a [generalized Specht module](#generalized-specht-module) and differs from specifying a [skew shape](#skew-young-diagram) by two nested proper partitions.

###### Good-letter matching in a tableau word

↑ **Parent:** [Pair of partitions for a generalized Specht module](#pair-of-partitions-for-a-generalized-specht-module)

Read a word of type $b$ from the left. Every $1$ is good; an $i+1$ is good when the number of previous good $i$'s exceeds the number of previous good $(i+1)$'s. The set $s(a,b)$ contains words with at least $a_i$ good $i$'s for each $i$. Their matched chains yield independent marked-column [polytabloids](#polytabloid); column antisymmetrization and the add-or-raise recursion give $\dim S^{a,b}=|s(a,b)|$ over every [field](algebra.md#field).

###### Specht filtration

↑ **Parent:** [Specht module](#specht-module)

A [Specht filtration](#specht-filtration) is a finite chain of [submodules](module-theory.md#submodule) whose successive quotients are [Specht modules](#specht-module). In positive [characteristic](algebra.md#characteristic-of-a-field) it need not split and is not a [composition series](finite-group-theory.md#composition-series), because its Specht factors may themselves be reducible. [Dimensions](vector-space.md#dimension-vector-space) and ordinary lifted [characters](representation-theory.md#character-of-a-representation) can still be added along the filtration.

<h6 id="littlewood-richardson-rule">Littlewood–Richardson rule</h6>

↑ **Parent:** [Specht filtration](#specht-filtration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Littlewood–Richardson_rule)

For induction of $S^\mu\boxtimes S^\lambda$ to the [symmetric group](finite-group-theory.md#symmetric-group) on $|\mu|+|\lambda|$ letters, the [Specht filtration](#specht-filtration) multiplicity of $S^\nu$ is the number of [Semistandard Young tableaux](#semistandard-young-tableau) of [skew shape](#skew-young-diagram) $\nu/\mu$, content $\lambda$, and [lattice word](#lattice-word) read from right to left in each row, taking rows from top to bottom. In [characteristic](algebra.md#characteristic-of-a-field) zero these are [irreducible](representation-theory.md#irreducible-representation) constituents; in positive [characteristic](algebra.md#characteristic-of-a-field) they remain Specht factors rather than simple constituents. Content $(1)$ gives the add-one-cell induction rule.

<h6 id="littlewood-richardson-coefficient">Littlewood–Richardson coefficient</h6>

↑ **Parent:** [Littlewood–Richardson rule](#littlewood-richardson-rule)

The nonnegative integer $c_{\alpha\beta}^\nu$ is the multiplicity of $S^\nu$ in $\operatorname{Ind}_{S_{|\alpha|}\times S_{|\beta|}}^{S_{|\nu|}}(S^\alpha\boxtimes S^\beta)$ in characteristic zero. The [Littlewood–Richardson rule](#littlewood-richardson-rule) counts it by [Semistandard Young tableaux](#semistandard-young-tableau) of skew shape $\nu/\alpha$, content $\beta$, and [lattice word](#lattice-word) in right-to-left, top-to-bottom reading order. For example $c_{(3,2,1),(3,2)}^{(5,3,2,1)}=3$: the two new top cells must be ones, and the remaining reading letters can be $122,212,221$. This coefficient also multiplies [Schur functions](combinatorics.md#schur-polynomial) in the [induction ring of symmetric-group characters](#induction-ring-of-symmetric-group-characters).

###### Pieri rule

↑ **Parent:** [Littlewood–Richardson rule](#littlewood-richardson-rule)

In the induction ring of ordinary symmetric-group [characters](representation-theory.md#character-of-a-representation), $[\lambda][r]$ is the sum, with multiplicity one, of $[\nu]$ for which $\nu/\lambda$ is a [horizontal strip](#horizontal-strip) of $r$ cells. Here $[r]$ is the [trivial representation](representation-theory.md#trivial-representation) of $S_r$. In the [Littlewood–Richardson rule](#littlewood-richardson-rule), content $(r)$ means every skew entry is $1$; strict column increase is possible exactly when there is at most one new cell in every column. This proves the rule.

###### Specht modules as minimal left ideals

↑ **Parent:** [Specht module](#specht-module)

In the complex symmetric-group algebra, normalize a [Young symmetrizer](#young-symmetrizer) by $e_t=h_t/H_\lambda$. The [row-column collision lemma](#row-column-collision-lemma) proves $e_tAe_t=\mathbb Ce_t$, so $e_t$ is a [primitive idempotent](commutative-algebra.md#primitive-idempotent) and $Ae_t$ is an irreducible left module. Different shapes are separated by the vanishing corner $h_\lambda A h_\mu=0$ for $\lambda>\mu$. Counting [conjugacy classes](group-theory.md#conjugacy-class) then proves that these modules exhaust the [simple modules](module-theory.md#irreducible-module).

###### James submodule theorem

↑ **Parent:** [Specht module](#specht-module)

Let $U$ be a submodule of the Young permutation module $M^\lambda$ over any field. Then either

$$
S^\lambda\subseteq U
\qquad\text{or}\qquad
U\subseteq(S^\lambda)^\perp
$$

for the [tabloid bilinear form](#tabloid-bilinear-form). The key identity is $b_tu=\langle u,e(t)\rangle e(t)$: if one pairing is nonzero, the cyclic generator $e(t)$ and hence the whole Specht module lies in $U$.

###### Conjugate Specht module as a sign-twisted dual

↑ **Parent:** [Specht module](#specht-module)

Over a field of characteristic zero,

$$
S^\lambda\otimes S^{(1^n)}\cong(S^{\lambda'})^*.
$$

The map from $M^{\lambda'}$ sending the tabloid of $g t'$ to $g e(t)\otimes g e(u)$ is a surjection whose kernel is $(S^{\lambda'})^\perp$.

###### Restriction branching rule for a symmetric group

↑ **Parent:** [Specht module](#specht-module)

Over the complex numbers, restriction from $S_n$ to $S_{n-1}$ is multiplicity-free:

$$
\operatorname{Res}^{S_n}_{S_{n-1}}S^\lambda
\cong\bigoplus_{\mu\in\lambda^-}S^\mu.
$$

Equivalently, one removes one [Removable node of a Young diagram](#removable-node-of-a-young-diagram) in every possible distinct way.

###### Standard-character multiplicity in a Specht self-product

↑ **Parent:** [Restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group)

For $\lambda\vdash n$ with $n\geq2$,

$$
\langle\chi^\lambda\chi^\lambda,\chi^{(n-1,1)}\rangle=|\lambda^-|-1.
$$

Indeed, adjoining the trivial character to the standard character gives the point-permutation character, and [Frobenius reciprocity](representation-theory.md#frobenius-reciprocity) turns its multiplicity in the self-product into the norm of the multiplicity-free restriction.

###### Linear independence of standard polytabloids

↑ **Parent:** [Specht module](#specht-module)

Order tabloids lexicographically by the row containing $1$, then the row containing $2$, and so on. For a standard tableau $t$, the tabloid $\{t\}$ occurs with coefficient one in $e(t)$ and precedes every other tabloid occurring in it. Distinct standard tableaux have distinct leading tabloids, so their polytabloids are linearly independent.

###### Hook-length formula

↑ **Parent:** [Specht module](#specht-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hook-length_formula)

The degree of the complex irreducible character labelled by $\lambda\vdash n$ is

$$
f^\lambda=\frac{n!}{\prod_{(i,j)\in\lambda}h_{i,j}(\lambda)}.
$$

###### Least non-linear ordinary degree of a symmetric group

↑ **Parent:** [Hook-length formula](#hook-length-formula)

For $n\ge3$, the least ordinary [irreducible](representation-theory.md#irreducible-representation) [dimension](vector-space.md#dimension-vector-space) exceeding one is $n-1$, except at $n=4$, where $S^{(2,2)}$ has [dimension](vector-space.md#dimension-vector-space) two. The dimension-$n-1$ shapes are $(n-1,1)$ and its [conjugate partition](#conjugate-partition), with the additional shapes $(3,3)$ and $(2,2,2)$ at $n=6$. For $n=2$ there is no non-linear [irreducible](representation-theory.md#irreducible-representation). A proof uses the [restriction branching rule for a symmetric group](#restriction-branching-rule-for-a-symmetric-group): a nonstandard shape with at least two corners has two non-linear predecessors, and a rectangular shape has one predecessor which in turn has two non-linear predecessors. This bounds its degree strictly above $n-1$ once $n\ge9$; the smaller cases follow directly from the [hook-length formula](#hook-length-formula).

###### Trace computation of Specht module dimension

↑ **Parent:** [Hook-length formula](#hook-length-formula)

Right multiplication by $e_t=h_t/H_\lambda$ on the [group algebra](associative-algebra.md#group-algebra) is an [idempotent](commutative-algebra.md#idempotent) with image $Ae_t$. Every diagonal entry in the [permutation](combinatorics.md#permutation) basis is the coefficient of the identity in $e_t$, namely $1/H_\lambda$. Thus its rank equals its trace, giving $\dim S^\lambda=n!/H_\lambda$. Triangular standard-tableau ideals and the [Robinson–Schensted correspondence](#robinson-schensted-correspondence) identify this dimension with the standard-tableau count.

###### Determinant formula for Specht module dimension

↑ **Parent:** [Hook-length formula](#hook-length-formula)

For a partition $\lambda\vdash n$ with $k$ positive parts, the number of [standard Young tableaux](#standard-young-tableau), and hence the dimension of its complex [Specht module](#specht-module), is $n!\det(1/(\lambda_i-i+j)!)$. Negative factorial arguments give zero entries. Setting $L_i=\lambda_i+k-i$ turns the determinant into $\prod_{i<j}(L_i-L_j)/\prod_iL_i!$ by the [Vandermonde determinant](galois-theory.md#vandermonde-determinant), matching the [hook-length formula](#hook-length-formula).

<h6 id="greene-nijenhuis-wilf-hook-walk">Greene–Nijenhuis–Wilf hook walk</h6>

↑ **Parent:** [Hook-length formula](#hook-length-formula)

At a noncorner cell of a [Young diagram](#young-diagram), this random walk chooses uniformly one of the other cells in its [hook of a Young diagram](#hook-of-a-young-diagram). It stops at a corner. Every step moves right or down, so it terminates. Its corner probabilities provide a probabilistic proof of the [hook-length formula](#hook-length-formula).

###### Hook walk terminal probability

↑ **Parent:** [Greene–Nijenhuis–Wilf hook walk](#greene-nijenhuis-wilf-hook-walk)

For a target corner $(\alpha,\beta)$ in the [Greene–Nijenhuis–Wilf hook walk](#greene-nijenhuis-wilf-hook-walk), put $A_i=h(i,\beta)-1$ and $B_j=h(\alpha,j)-1$. The probability of terminating there from $(a,b)$ factors as $F_aG_b$, where $F_\alpha=G_\beta=1$, $F_a=A_a^{-1}\prod_{i=a+1}^{\alpha-1}(1+A_i^{-1})$ for $a<\alpha$, and $G_b=B_b^{-1}\prod_{j=b+1}^{\beta-1}(1+B_j^{-1})$ for $b<\beta$. It is zero when the start is outside the target's northwest rectangle. The factorization uses $h(i,j)-1=A_i+B_j$ and the first-step recurrence.

<h6 id="murnaghan-nakayama-rule">Murnaghan–Nakayama rule</h6>

↑ **Parent:** [Specht module](#specht-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Murnaghan–Nakayama_rule)

If a permutation has a $k$-cycle and remaining cycle type $\rho$, then

$$
\chi^\lambda(k,\rho)=
\sum_H(-1)^{\operatorname{leg}(H)}\chi^{\lambda\setminus H}(\rho),
$$

where the sum is over removable rim hooks of length $k$.

###### Power-sum border-strip multiplication

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

Multiplication of an [alternant](polynomial.md#monomial-alternant) by $p_r$ is the sum of alternants obtained by raising one row exponent by $r$. Equal exponents give zero. Otherwise sort the shifted [beta number of a partition](#beta-number-of-a-partition) back into decreasing order. The resulting partition adds a size-$r$ [rim hook](#rim-hook); the number of crossed exponents is its height and supplies the [determinant](linear-algebra.md#determinant) sign. This proves the formula through the [bialternant formula](combinatorics.md#bialternant-formula). Iteration counts signed [border-strip tableaux](#border-strip-tableau).

###### Staircase Schur functions use only odd power sums

↑ **Parent:** [Power-sum border-strip multiplication](#power-sum-border-strip-multiplication)

With $m$ beta numbers, the staircase has set $\{0,2,\ldots,2m-2\}$. Lowering a bead by a positive even number either hits an occupied bead or a negative position, so no even-size [rim hook](#rim-hook) can be removed. The adjoint of multiplication by $p_r$ under the [Hall inner product of symmetric functions](combinatorics.md#hall-inner-product-of-symmetric-functions) is $r\,\partial/\partial p_r$. The [power-sum border-strip multiplication](#power-sum-border-strip-multiplication) formula therefore gives zero derivative with respect to every even power sum. Since the rational symmetric-function algebra is freely generated by the power sums, the stated conclusion follows.

###### Maximal p-hook character formula

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

Let $\kappa$ be the [core of a partition](#core-of-a-partition) $\lambda$ at prime modulus $p$, with quotient component sizes $w_i$ and total weight $w$. Complete $p$-hook removal sequences number $N_p(\lambda)=\binom{w}{w_0,\ldots,w_{p-1}}\prod_if^{\lambda^{(i)}}$. Their signs agree because abacus bead-crossing parities telescope to the [permutation](combinatorics.md#permutation) taking the initial labeled beads to the packed core order. Repeated [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule) gives the displayed formula for any [permutation](combinatorics.md#permutation) $\pi$ on the remaining letters.

###### Sign of an abacus hook-removal sequence

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

The parity of the sum of the leg lengths in any sequence that removes all $e$-hooks from $\lambda$ is independent of the sequence. Its sign $\varepsilon_e(\lambda)$ is therefore well defined and supplies the common sign in repeated applications of the [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule).

###### Two-row alternating character cancellation

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

For even $n$, the [virtual character](representation-theory.md#virtual-character)

$$
F_n=\sum_{r=0}^{n/2}(-1)^r\chi^{(n-r,r)}
$$

vanishes on every permutation having an odd cycle. Under the [Frobenius characteristic map](combinatorics.md#frobenius-characteristic-map), the [Jacobi–Trudi identity](combinatorics.md#jacobi-trudi-identity) identifies its characteristic with the degree-$n$ part of $H(t)H(-t)$, which contains only products of even-indexed power sums.

###### Principal-hook character value of a symmetric group

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

At a permutation whose cycle lengths are the principal hook lengths of $\lambda$, the Murnaghan–Nakayama rule has a unique complete removal sequence. Consequently $\chi^\lambda$ has value $1$ or $-1$ there.

###### Staircase-character vanishing criterion

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

For a partition $\lambda$, the irreducible character $\chi^\lambda$ vanishes on every cycle type containing an even part exactly when $\lambda$ is a staircase $(m,m-1,\ldots,1)$. A staircase has only odd hook lengths. Conversely, vanishing first forces $\lambda$ to be self-conjugate; applying the Murnaghan–Nakayama rule at the largest even hooks then forces consecutive row lengths.

###### Conjugate Specht character

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

Conjugating a Young diagram twists its complex Specht module by the sign representation:

$$
S^{\lambda'}\cong S^\lambda\otimes\operatorname{sgn},
\qquad
\chi^{\lambda'}=\chi^\lambda\operatorname{sgn}.
$$

###### Straightening of a symmetric-group character indexed by a composition

↑ **Parent:** [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule)

For the alternating expression $\psi^\lambda$ indexed by an integer composition, swapping two adjacent entries of $\lambda-\mathrm{id}$ negates $\psi^\lambda$. If two entries coincide the expression vanishes; otherwise sorting produces, up to sign, the irreducible character indexed by the resulting partition.

###### Modular Specht module

↑ **Parent:** [Specht module](#specht-module)

Over a field of characteristic $p$, the invariant tabloid form on $S^\lambda$ may be degenerate. Its radical is $S^\lambda\cap(S^\lambda)^\perp$.

###### Tabloid bilinear form

↑ **Parent:** [Modular Specht module](#modular-specht-module)

The tabloid bilinear form makes the tabloid basis orthonormal and restricts to an invariant [bilinear form](linear-algebra.md#bilinear-form) on each [Specht module](#specht-module). In positive [characteristic of a field](algebra.md#characteristic-of-a-field), its radical controls the corresponding simple quotient.

###### Regular partition

↑ **Parent:** [Modular Specht module](#modular-specht-module)

A partition is $p$-regular when no part occurs $p$ or more times.

###### Regular label of the modular sign representation

↑ **Parent:** [Regular partition](#regular-partition)

Write $n=q(p-1)+r$, $0\le r<p-1$. The [regular partition](#regular-partition) labelling the [sign representation](#sign-representation) in characteristic $p>0$ is $\lambda=((q+1)^r,q^{p-1-r})$, with zero parts removed. Its [conjugate partition](#conjugate-partition) is $((p-1)^q,r)$, which satisfies the [invariant vector criterion for a Specht module](#invariant-vector-criterion-for-a-specht-module). The sign-twisted duality of [Specht modules](#specht-module) turns this invariant line into a sign quotient of $S^\lambda$, necessarily its unique simple [head](module-theory.md#head-of-a-module). Conversely, regularity says consecutive column heights differ by less than $p$; combining this with the invariant congruences forces these heights to be $p-1$ except possibly the last. For $p=2$, the label is $(n)$ because sign equals the [trivial representation](representation-theory.md#trivial-representation).

###### Simple symmetric-group module from a regular partition

↑ **Parent:** [Regular partition](#regular-partition)

For a $p$-regular partition,

$$
D^\lambda=S^\lambda/(S^\lambda\cap(S^\lambda)^\perp)
$$

is nonzero and absolutely irreducible. Distinct $p$-regular partitions label nonisomorphic simple modules.

###### Absolute irreducibility of the Specht radical quotient

↑ **Parent:** [Simple symmetric-group module from a regular partition](#simple-symmetric-group-module-from-a-regular-partition)

The [James submodule theorem](#james-submodule-theorem) follows from $\kappa_tv=\langle v,e_t\rangle e_t$. A nonzero restricted form therefore gives a simple radical quotient. If $m_j$ counts equal-length rows, all integral [polytabloid](#polytabloid) pairings are divisible by $\prod_jm_j!$, while pairing with row reversal gives $\prod_j(m_j!)^j$. Thus the form is nonzero modulo $p$ exactly for [regular partitions](#regular-partition). The construction and the proof commute with every [field extension](algebra.md#field-extension), so the quotient is absolutely [irreducible](representation-theory.md#irreducible-representation), including over the [prime field](algebra.md#prime-field).

###### Endomorphism theorem for a regular Specht module

↑ **Parent:** [Regular partition](#regular-partition)

If $\lambda=(n^{a_n},\ldots,1^{a_1})$ is $p$-regular, then

$$
\operatorname{End}_{\mathbb F S_n}(S^\lambda)=\mathbb F.
$$

For a tableau $t$ and its row reversal $t^*$,

$$
\langle e(t),e(t^*)\rangle=\prod_j(a_j!)^j,
$$

which is nonzero in characteristic $p$. Applying a column antisymmetrizer to an endomorphism at $e(t^*)$ therefore forces its value on the cyclic generator $e(t)$ to be scalar.

### Dominance order on partitions

↑ **Parent:** [Partition of an integer](#partition-of-an-integer)

For partitions of the same integer, $\lambda$ dominates $\mu$ when

$$
\sum_{i=1}^r\lambda_i\geq\sum_{i=1}^r\mu_i
$$

for every $r$.

#### Single-box up-move

↑ **Parent:** [Dominance order on partitions](#dominance-order-on-partitions)

A single-box up-move changes a [partition of an integer](#partition-of-an-integer) by adding one to row $i$ and subtracting one from row $j>i$, provided the result remains a partition. It increases exactly the partial sums ending between rows $i$ and $j-1$. A partition $\mu$ dominates $\lambda$ precisely when it is obtainable from $\lambda$ by a sequence of these moves: fill the first deficient row from the row at the first return of the cumulative deficit to zero. This preserves the partition inequalities and decreases the distance to $\mu$.

## Brauer defect-zero vanishing theorem

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

If an irreducible character has $p$-defect zero, it vanishes on every element whose order is divisible by $p$. Consequently, $\chi(g)\ne0$ implies that the square-free part of the order of $g$ divides $|G|/\chi(1)$.

## Symmetric-group character co-degree vanishing criterion

↑ **Parent:** [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)

For $\chi\in\operatorname{Irr}(S_n)$, if the order of $g\in S_n$ does not divide $|S_n|/\chi(1)$, then $\chi(g)=0$. The [Hook-length formula](#hook-length-formula) turns the co-degree into a product of hook lengths, while the [Murnaghan–Nakayama rule](#murnaghan-nakayama-rule) detects a cycle whose required prime-power hook cannot be removed.

## ↑ Ancestors (5)

1. [Representation theory](representation-theory.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Standard representation of the symmetric group](representation-theory.md#standard-representation-of-the-symmetric-group)
