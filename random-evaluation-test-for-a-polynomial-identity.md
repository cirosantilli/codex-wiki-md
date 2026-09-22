# Random evaluation test for a polynomial identity

↑ **Parent:** [Polynomial identity testing](polynomial-identity-testing.md)

Let $P$ be a nonzero [multivariate polynomial](multivariate-polynomial.md) over a [field](field.md) $K$, with [total degree](total-degree-of-a-polynomial.md) at most $d\ge0$. Choose a nonempty [finite set](finite-set.md) $S\subseteq K$. For [independent random variables](independent-random-variables.md) $a_1,\ldots,a_n$, each with a [uniform distribution on a finite set](discrete-uniform-distribution.md) on $S$, the [Schwartz-Zippel lemma](schwartz-zippel-lemma.md) gives

$$
\mathbb P\bigl(P(a_1,\ldots,a_n)=0\bigr)\le\min\{1,d/|S|\}.
$$

Nonzeroness is essential; the zero [polynomial](polynomial-split.md) always evaluates to zero. The [total degree](total-degree-of-a-polynomial.md) sums exponents within each [monomial](monomial.md), rather than taking their maximum: $x^2y^3+y$ has [total degree](total-degree-of-a-polynomial.md) five. The [field](field.md) need not be finite, but $S$ must be finite. The estimate reduces error only when $d/|S|<1$.[CMPT 710 and CMPT 407 - Computational Complexity - Fall 2007; CMPT 710 - Complexity Theory: Lecture 18, §3.1, pp. 3–4: Lemma 4 and its inductive proof](cmpt-710-and-cmpt-407-computational-complexity-fall-2007/cmpt-710-complexity-theory-lecture-18.md)

The proof begins with the [root bound for a polynomial](lagrange-root-bound-over-a-field.md). For several [variables](variable-mathematics.md), write $P=\sum_{j=0}^m Q_j(x_1,\ldots,x_{n-1})x_n^j$, with $Q_m\ne0$. The [total degree](total-degree-of-a-polynomial.md) of $Q_m$ is at most $d-m$. By [induction](mathematical-induction.md), $Q_m$ vanishes with [probability](probability.md) at most $(d-m)/|S|$. Otherwise the remaining univariate [polynomial](polynomial-split.md) has at most $m$ [polynomial roots](root-of-a-polynomial.md). Adding the two contributions gives $d/|S|$.[CMPT 710 and CMPT 407 - Computational Complexity - Fall 2007; CMPT 710 - Complexity Theory: Lecture 18, §3.1, pp. 3–4: split by the leading coefficient in the last variable](cmpt-710-and-cmpt-407-computational-complexity-fall-2007/cmpt-710-complexity-theory-lecture-18.md)

The [algorithm](algorithm-split.md) samples a point, performs exact [polynomial evaluation](polynomial-evaluation.md), rejects the identity if the value is nonzero, and otherwise accepts. The lemma bounds false acceptance for every fixed nonzero [input](input-computer-science.md). For the [polynomial identity testing over a finite field](polynomial-identity-testing-over-a-finite-field.md) example, $G$ has $d=2$ and $|S|=5$, so its exact $2/5$ error attains the bound. Numerical near-zero values from [floating-point arithmetic](floating-point-arithmetic-split.md) do not satisfy this exact algebraic contract. A [polynomial-time algorithm](polynomial-time-algorithm.md) claim additionally needs efficient sampling and evaluation, including the [bit](bit.md) cost of representing and operating on [field](field.md) elements. Counting [field](field.md) operations alone does not establish that cost.

## ↑ Ancestors (5)

1. [Polynomial identity testing](polynomial-identity-testing.md)
2. [Randomized algorithm](randomized-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Independent repetition of a polynomial identity test](independent-repetition-of-a-polynomial-identity-test.md)
- [One-sided error](one-sided-error.md)
- [Polynomial identity testing](polynomial-identity-testing.md)
