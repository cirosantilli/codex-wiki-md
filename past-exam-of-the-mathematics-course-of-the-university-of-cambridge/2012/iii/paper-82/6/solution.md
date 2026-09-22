<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use a [Boolean circuit](../../../../../boolean-circuit.md) of unbounded-fan-in AND and OR gates, with negations pushed to the input [Boolean literals](../../../../../boolean-literal.md). Its [circuit depth](../../../../../depth-of-a-boolean-circuit.md) is the largest number of AND/OR gates on an input-to-output path, and its [circuit size](../../../../../circuit-size.md) $M$ counts these gates. Constants and [Boolean literals](../../../../../boolean-literal.md) may be supplied as inputs. Equivalent standard size conventions only enlarge the absolute constants. One can merge adjacent gates of the same type; the depth-reduction argument below keeps the two possible normal forms available at each gate.

A [random restriction](../../../../../random-restriction-of-a-boolean-function.md) with parameter $p$ independently leaves each variable live with [probability](../../../../../probability.md) $p$ and otherwise fixes it to zero or one with [probability](../../../../../probability.md) $(1-p)/2$ each. The [Håstad switching lemma](../../../../../hastad-switching-lemma.md) states that for a width-$w$ [DNF](../../../../../disjunctive-normal-form.md) or [conjunctive normal form](../../../../../conjunctive-normal-form.md) $F$,

$$
\mathbb P_{\rho\sim\mathcal R_p}\bigl(\operatorname{DTdepth}(F_\rho)>s\bigr)\le(5pw)^s.
$$

Width bounds [Boolean literals](../../../../../boolean-literal.md) in a term or clause, not the number of terms. A [decision tree](../../../../../decision-tree.md) of depth at most $s$ has both a [DNF](../../../../../disjunctive-normal-form.md) and a [conjunctive normal form](../../../../../conjunctive-normal-form.md) of width at most $s$ and has real multilinear degree at most $s$. Indeed every leaf condition is a product of at most $s$ factors $x_i$ or $1-x_i$; sum the accepting leaves. The switching lemma controls the canonical [decision tree](../../../../../decision-tree.md), hence implies this representation bound.

We detail the [Boolean circuit](../../../../../boolean-circuit.md) simplification parameters. First use a $1/10$-random restriction. For a bottom AND gate, let $X$ count its live [Boolean literals](../../../../../boolean-literal.md) on the event that no fixed [Boolean literal](../../../../../boolean-literal.md) kills it. For $w$ distinct [Boolean literals](../../../../../boolean-literal.md),

$$
\mathbb E\bigl[5^X\mathbf1_{\{\text{not killed}\}}\bigr]
=\bigl(9/20+5/10\bigr)^w=(19/20)^w\le1.
$$

Thus the [probability](../../../../../probability.md) of retaining more than $s$ live [Boolean literals](../../../../../boolean-literal.md) without becoming constant is at most $5^{-s}$. The same calculation applies to bottom OR gates, with the opposite killing value. Repeated [Boolean literals](../../../../../boolean-literal.md) are removed and contradictory [Boolean literals](../../../../../boolean-literal.md) make a constant gate. A union bound makes all nonconstant bottom gates width at most $s$, except with [probability](../../../../../probability.md) at most $M_0 5^{-s}$.

Now apply $d-1$ successive restrictions, each retaining [probability](../../../../../probability.md) $1/(10s)$ of the remaining variables. At a two-layer gate, the current bottom forms are width-$s$ [DNFs](../../../../../disjunctive-normal-form.md) or [conjunctive normal forms](../../../../../conjunctive-normal-form.md). The [Håstad switching lemma](../../../../../hastad-switching-lemma.md) bounds its [probability](../../../../../probability.md) of failing to reduce to decision-tree depth at most $s$ by $2^{-s}$. Convert the successful [decision tree](../../../../../decision-tree.md) into the opposite normal form, whose terms or clauses have width at most $s$, and merge its outer gate with the adjacent gate of the same type. This removes one layer. Repeat upwards until the output has a depth-$s$ [decision tree](../../../../../decision-tree.md).

The bookkeeping matters: although a [decision tree](../../../../../decision-tree.md) may give $2^s$ clauses, each subsequent switching event is charged to the corresponding original [Boolean circuit](../../../../../boolean-circuit.md) gate, not to each newly created clause. The lemma permits any number of terms. Each original gate is charged once, so the sum of the failure probabilities is at most $M2^{-s}$, without an extra exponential size factor. Conditioning on successful preceding stages is harmless because each next restriction is fresh and the width bound holds for every preceding success. For a general [Boolean circuit](../../../../../boolean-circuit.md) the [conjunctive normal form](../../../../../conjunctive-normal-form.md) or [DNF](../../../../../disjunctive-normal-form.md) representation at a shared gate can be chosen separately for each outgoing use; no extra gates need to be counted as switching targets.

The composed restriction has live-variable [probability](../../../../../probability.md)

$$
p=\frac1{10}\left(\frac1{10s}\right)^{d-1}=\frac1{10^d s^{d-1}}.
$$

Fixed values are still unbiased and coordinates independent. We have proved the useful intermediate estimate

$$
\boxed{\mathbb P_{\rho\sim\mathcal R_p}(\deg f_\rho>s)\le M2^{-s}.}
$$

For $d=1$, the initial bottom-gate argument alone gives this conclusion. This is a depth-reduction estimate, not the desired Fourier-tail theorem used as a black box.

Next derive exactly how restrictions affect the [Fourier-Walsh transform](../../../../../fourier-walsh-transform.md). Let $J$ be the random live set and $a$ the fixed assignment outside $J$. With $\chi_S(x)=(-1)^{\sum_{i\in S}x_i}$, the restricted coefficient at $U\subset J$ is

$$
\widehat{f_{J,a}}(U)=\sum_{B\subset J^c}\widehat f(U\cup B)\chi_B(a).
$$

Orthogonality of the fixed-coordinate characters eliminates cross terms after averaging over $a$. Therefore

$$
\mathbb E_a|\widehat{f_{J,a}}(U)|^2=\sum_{B\subset J^c}|\widehat f(U\cup B)|^2,
$$

and then averaging over $J$ gives the [expected Fourier weight after a random restriction](../../../../../expected-fourier-weight-after-a-random-restriction.md) identity

$$
\boxed{\mathbb E_\rho\sum_{|U|>s}|\widehat{f_\rho}(U)|^2
=\sum_S|\widehat f(S)|^2\mathbb P\bigl(\operatorname{Bin}(|S|,p)>s\bigr).}
$$

**The original high-degree tail is not preserved:** each original coefficient is weighted by a [binomial distribution](../../../../../binomial-distribution.md) survival [probability](../../../../../probability.md). On successful restrictions the left-hand tail vanishes; on failures it is at most one by [Parseval's identity](../../../../../parseval-identity.md) and $0\le f_\rho\le1$. Hence its expectation is at most $M2^{-s}$.

Put $u=t^{1/d}$. If $u\ge40$, choose $s=\lfloor u/40\rfloor\ge1$ and the preceding value of $p$. For every $|S|>t$, the [binomial distribution](../../../../../binomial-distribution.md) mean satisfies

$$
\mu=p|S|>\frac{u^d}{10^d s^{d-1}}\ge4^d s\ge4s.
$$

Its [variance](../../../../../variance-split.md) is at most $\mu$. The [Chebyshev inequality](../../../../../chebyshev-inequality.md) gives

$$
\mathbb P(\operatorname{Bin}(|S|,p)\le s)
\le\frac\mu{(\mu-s)^2}\le\frac4{9s}<\frac12.
$$

Thus the exact expectation identity bounds at least half the original tail above $t$, and

$$
\sum_{|S|>t}|\widehat f(S)|^2\le2M2^{-s}\le4M2^{-t^{1/d}/40}.
$$

When $u<40$ the same bound follows from the trivial total-weight bound $\sum_S|\widehat f(S)|^2\le1$. We obtain explicit absolute constants,

$$
\boxed{\sum_{|r|>t}|\widehat f(r)|^2\le4M\,2^{-t^{1/d}/40}.}
$$

This supplies the requested overview of the [Linial-Mansour-Nisan theorem](../../../../../linial-mansour-nisan-theorem.md) with the actual switching scale, gate-count bookkeeping and restriction-to-Fourier calculation. The argument uses the unbounded-fan-in AND/OR [Boolean circuit](../../../../../boolean-circuit.md) basis; allowing arbitrary gates would make the theorem false, since one parity gate could have all its nonconstant [Fourier weight](../../../../../fourier-weight.md) at level $n$. The original theorem is [Linial, Mansour and Nisan's circuit Fourier bound](https://doi.org/10.1145/174130.174138).

## ↑ Ancestors (11)

1. [6](../6.md)
2. [Section C](../section-c.md)
3. [Paper 82](../../paper-82-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
