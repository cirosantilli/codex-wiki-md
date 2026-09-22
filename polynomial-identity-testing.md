# Polynomial identity testing

↑ **Parent:** [Randomized algorithm](randomized-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_identity_testing)

Polynomial identity testing asks whether a polynomial represented implicitly, such as by an arithmetic circuit or a remainder computation, is the zero polynomial.

Here zero means that every [coefficient](coefficient.md) vanishes after collecting equal [monomials](monomial.md) in the [polynomial ring](polynomial-ring.md). Testing equality of two [polynomials](polynomial-split.md) $A,B$ amounts to testing $P=A-B$ for zero. An [arithmetic circuit](arithmetic-circuit.md) can permit cheap [polynomial evaluation](polynomial-evaluation.md) even when expanding all [monomials](monomial.md) is expensive. The [random evaluation test for a polynomial identity](random-evaluation-test-for-a-polynomial-identity.md) exploits this: one nonzero value disproves the [polynomial identity](polynomial-identity.md), while a known [total degree](total-degree-of-a-polynomial.md) limits how often a nonzero [polynomial](polynomial-split.md) can evade detection.[CPSC 536N: Randomized Algorithms; Lecture 9: Polynomial Identity Testing by the Schwartz-Zippel Lemma, §1: formal zero means all coefficients vanish; representations and evaluation access](cpsc-536n-randomized-algorithms/lecture-9-polynomial-identity-testing-by-the-schwartz-zippel-lemma.md)

For example, for an [integer](integer-split.md) $n\ge1$, $\prod_{i=1}^n(1+x_i)$ has $2^n$ distinct [monomials](monomial.md), one for each [subset](subset.md) of the $n$ [variables](variable-mathematics.md). Its factored expression needs only $n$ [additions](addition.md) and $n-1$ [multiplications](multiplication.md) for one [polynomial evaluation](polynomial-evaluation.md). Evaluating the compact expression avoids creating its expanded list of [coefficients](coefficient.md). The saving is especially attractive in many [variables](variable-mathematics.md); it does not make a zero result into a proof of identity.

**Table of contents**

- [Polynomial identity testing over a finite field](polynomial-identity-testing-over-a-finite-field.md)
- [Random evaluation test for a polynomial identity](random-evaluation-test-for-a-polynomial-identity.md)
- [Independent repetition of a polynomial identity test](independent-repetition-of-a-polynomial-identity-test.md)

## ↑ Ancestors (4)

1. [Randomized algorithm](randomized-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [One-sided error](one-sided-error.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-124/4/iii/solution.md)
- [Randomized algorithm](randomized-algorithm.md)
