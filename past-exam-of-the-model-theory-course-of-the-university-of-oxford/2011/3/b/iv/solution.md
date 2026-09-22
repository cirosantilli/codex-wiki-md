<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $P_1$ and $P_3$ be the sets of primes congruent to one and three modulo four. Both are infinite. For $P_1$, if a finite list contained them all, put $N=(2p_1\cdots p_r)^2+1$. Any prime divisor $q$ of this odd number is new and has minus one as a square modulo $q$, hence belongs to $P_1$ by the given criterion. For $P_3$, use $N=4p_1\cdots p_r-1$. It is three modulo four, so at least one of its odd prime divisors is three modulo four; none of the listed primes divides $N$. These are elementary [Euclidean proofs of infinitely many primes in each odd residue class modulo four](../../../../../euclidean-proofs-of-infinitely-many-primes-in-each-odd-residue-class-modulo-four.md).

On the set of all primes, the cofinite sets together with $P_1$ have the [finite intersection property](../../../../../finite-intersection-property.md); so do the cofinite sets together with $P_3$. Extend the generated filters to [ultrafilters](../../../../../ultrafilter.md) $\mathcal U_1$ and $\mathcal U_3$ using the [ultrafilter lemma](../../../../../ultrafilter-lemma.md). They are nonprincipal because they contain every cofinite set, including the complement of any singleton. Form

$$
\boxed{F_1=\prod_p\mathbb F_p/\mathcal U_1,\qquad F_2=\prod_p\mathbb F_p/\mathcal U_3.}
$$

Every sentence of $\Sigma$ has a cofinite truth set, hence belongs to both [ultrafilters](../../../../../ultrafilter.md). The [Łoś theorem](../../../../../los-theorem.md) shows $F_1,F_2\models\Sigma$. In particular they are fields, since each field axiom holds in every factor.

For each fixed positive integer $n$, the sentence $n\cdot1\ne0$ holds in $\mathbb F_p$ unless $p$ divides $n$. Its truth set is cofinite, so both fields satisfy it. Therefore $\boxed{\operatorname{char}F_1=\operatorname{char}F_2=0}$.

Finally the sentence $\exists x(x^2+1=0)$ holds at exactly the primes in $P_1\cup\{2\}$. This set belongs to $\mathcal U_1$, whereas its complement contains $P_3$ and belongs to $\mathcal U_3$. Łoś therefore gives

$$
\boxed{F_1\models\exists x(x^2+1=0),\qquad F_2\models\neg\exists x(x^2+1=0).}
$$

Thus minus one is a square in the first characteristic-zero [first-order model](../../../../../model-of-a-first-order-theory.md) of $\Sigma$ and is not a square in the second. The construction also shows why eventual truth over all primes need not decide a sentence whose truth splits along two infinite prime subsequences.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
