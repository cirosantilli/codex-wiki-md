# Divisibility

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisibility)

For [integers](integer-split.md) $d,n$, **$d$ divides $n$** when [multiplication](multiplication.md) by some [integer](integer-split.md) $k$ takes $d$ to $n$:

$$
d\mid n\quad\Longleftrightarrow\quad \text{there exists }k\in\mathbb Z\text{ such that }n=dk.
$$

Then $d$ is a [divisor](divisor.md) of $n$, and $n$ is an [integer multiple](integer-multiple.md) of $d$. The notation $d\nmid n$ means that no such [integer](integer-split.md) $k$ exists. For $d\ne0$, this is equivalent to saying that the [quotient](quotient.md) $n/d$ is an [integer](integer-split.md), or that [Euclidean division](euclidean-division.md) by $|d|$ leaves [remainder](remainder.md) zero.

For example, $3\mid12$ because $12=3\cdot4$, whereas $5\nmid12$ because $12=5\cdot2+2$. Signs do not change [divisibility](divisibility-split.md): $-3\mid12$ because $12=(-3)(-4)$, and $3\mid-12$ because $-12=3(-4)$. In general, changing the sign of either input preserves the relation.

The definition here permits zero as either input. Every [integer](integer-split.md) divides zero, since $0=d\cdot0$. In particular, **$0\mid0$**; however, $0\nmid n$ whenever $n\ne0$, since $0k$ is always zero. This is a statement about [multiplication](multiplication.md), and assigns no meaning to [division](division-mathematics.md) by zero: $0/0$ remains undefined.

Two useful properties come directly from the defining [multiplication](multiplication.md). [Divisibility](divisibility-split.md) is a [reflexive relation](reflexive-relation.md), since $n=n\cdot1$, and a [transitive relation](transitive-relation.md): if $b=ar$ and $c=bs$, then $c=a(rs)$. Moreover, a shared [divisor](divisor.md) divides every [integer](integer-split.md) [linear combination](linear-combination.md):

$$
d\mid a,\quad d\mid b\quad\Longrightarrow\quad d\mid(ax+by)\qquad(x,y\in\mathbb Z).
$$

Indeed, writing $a=du$ and $b=dv$ gives $ax+by=d(ux+vy)$. For example, $6\mid12$ and $6\mid18$ imply $6\mid(18-12)$. This small observation explains why the [Euclidean algorithm](euclidean-algorithm.md) preserves common [divisors](divisor.md), and why [Bézout's identity](bezout-s-identity.md) can certify a [greatest common divisor](greatest-common-divisor.md).

On the [positive integers](positive-integer.md), [divisibility](divisibility-split.md) is a [partial order](partially-ordered-set.md): if $a\mid b$ and $b\mid a$, then $a=b$. The restriction matters, since $3\mid-3$ and $-3\mid3$ although $3\ne-3$. The [prime factorization](fundamental-theorem-of-arithmetic.md) viewpoint makes this order concrete: $d\mid n$ exactly when every [prime valuation](prime-valuation.md) of $d$ is at most the corresponding [prime valuation](prime-valuation.md) of $n$. Thus one relation connects equal grouping, [prime factorization](fundamental-theorem-of-arithmetic.md), and [modular arithmetic](modular-arithmetic-split.md).

Book VII, definitions 3 and 5 of [Euclid's Elements](euclid-s-elements.md) describe the corresponding positive-number relation through one number measuring another and through [integer multiples](integer-multiple.md). The sign and zero conventions above belong to the present [integer](integer-split.md) formulation, rather than to those ancient definitions. [Euclid, Elements VII, definitions 3 and 5, T. L. Heath translation](https://geometor.github.io/euclid/heath/VII/index.html)

**Table of contents**

- [Common divisor](common-divisor.md)
- [Divisibility rule](divisibility-rule.md)
  - [Decimal digit-sum divisibility test](decimal-digit-sum-divisibility-test.md)
- [Semidivisible number](semidivisible-number.md)
- [Integer multiple](integer-multiple.md)
- [Divisor](divisor.md)
  - [Divisor lattice](divisor-lattice.md)
  - [Bi-unitary divisor](bi-unitary-divisor.md)
  - [Unitary divisor](unitary-divisor.md)
    - [Greatest common unitary divisor](greatest-common-unitary-divisor.md)
  - [Factor pair](factor-pair.md)
  - [Proper divisor](proper-divisor.md)
  - [Squarefree divisor](squarefree-divisor.md)
- [Greatest common divisor](greatest-common-divisor.md)
  - [Scaling identity for greatest common divisors](scaling-identity-for-greatest-common-divisors.md)
  - [Coprime integers](coprime-integers.md)
    - [Pairwise coprimality](pairwise-coprimality.md)
    - [Joint coprimality](joint-coprimality.md)
- [Least common multiple](least-common-multiple.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (56)

- [Algebraic number theory](algebraic-number-theory-split.md)
- [Cancellation of a common factor in a congruence](cancellation-of-a-common-factor-in-a-congruence.md)
- [Carmichael function](carmichael-function.md)
- [Circular prime](circular-prime.md)
- [Continuum many one-types of the integer ring](continuum-many-one-types-of-the-integer-ring.md)
- [Contrapositive](contrapositive.md)
- [Converse implication](converse-implication.md)
- [Coprime integers](coprime-integers.md)
- [Coresilience](coresilience.md)
- [Decimal digit-sum divisibility test](decimal-digit-sum-divisibility-test.md)
- [Divisibility](divisibility-split.md)
- [Divisor](divisor.md)
- [Divisor function](divisor-function.md)
- [Equivalence relation](equivalence-relation.md)
- [Euclid's lemma](euclid-s-lemma.md)
- [Extended Euclidean algorithm](extended-euclidean-algorithm.md)
- [Fermat little theorem](fermat-little-theorem.md)
- [Fermat number](fermat-number.md)
- [Field norm](field-norm.md)
- [Finite-state machine](finite-state-machine.md)
- [Fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md)
- [Inclusion-exclusion principle](inclusion-exclusion-principle.md)
- [Integer congruence](integer-congruence.md)
- [Legendre's formula](legendre-s-formula.md)
- [Linear congruence](linear-congruence.md)
- [Logical implication](logical-implication.md)
- [Modular arithmetic](modular-arithmetic-split.md)
- [Modular congruence](modular-congruence.md)
- [Nonzero residue permutation](nonzero-residue-permutation.md)
- [Number theory](number-theory-split.md)
- [p-adic absolute value](p-adic-absolute-value.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2006/algebra/3/b/solution.md)
- [Solution](past-exam-of-the-history-of-mathematics-course-of-the-university-of-oxford/2023/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/18h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-i/6/a/i/solution.md)
- [Solution](past-exam-of-the-model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford/2008/b/5/iv/solution.md)
- [Solution](past-exam-of-the-model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford/2008/b/7/v/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2005/c/2/b/i/solution.md)
- [Solution](past-exam-of-the-philosophy-of-science-supplementary-subject-of-the-university-of-oxford/2019/8/solution.md)
- [Solution](past-exam-of-the-rings-and-modules-course-of-the-university-of-oxford/2021/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation/6/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/3/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability/3/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability/3/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/1/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/1/c/ii/solution.md)
- [Prime divisor of a Fermat number](prime-divisor-of-a-fermat-number.md)
- [Prime number](prime-number-split.md)
- [Prime valuation](prime-valuation.md)
- [Radical of an integer](radical-of-an-integer.md)
- [Ring of integers](ring-of-integers.md)
- [Totient divisibility along divisors](totient-divisibility-along-divisors.md)
- [Tribonacci number](tribonacci-number.md)
