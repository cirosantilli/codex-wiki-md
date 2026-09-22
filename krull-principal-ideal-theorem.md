# Krull principal ideal theorem

↑ **Parent:** [Height of an ideal](height-of-an-ideal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull_principal_ideal_theorem)

In a [Noetherian ring](noetherian-ring.md), every [prime ideal](prime-ideal.md) minimal over a proper principal ideal has height at most one.

For a proof, suppose instead that $\mathfrak p_0\subsetneq\mathfrak q\subsetneq\mathfrak p$ and that $\mathfrak p$ is minimal over $(a)$. Quotient by $\mathfrak p_0$ and localize at $\mathfrak p$; one may assume that $R$ is a Noetherian local domain, $0\subsetneq\mathfrak q\subsetneq\mathfrak p$ with $\mathfrak p$ maximal, and $\mathfrak p$ is the only prime containing $(a)$. For the symbolic powers

$$
\mathfrak q^{(n)}=\mathfrak q^nR_{\mathfrak q}\cap R,
$$

each $\mathfrak q^{(n)}$ is $\mathfrak q$-primary. The quotient $R/(a)$ is a zero-dimensional [Noetherian ring](noetherian-ring.md) and hence [Artinian](artinian-ring.md), so the descending chain $(\mathfrak q^{(n)}+(a))/(a)$ stabilizes. For large $n$, writing an element of $\mathfrak q^{(n)}$ modulo $\mathfrak q^{(n+1)}$ and using $a\notin\mathfrak q$ gives

$$
\mathfrak q^{(n)}=\mathfrak q^{(n+1)}+a\mathfrak q^{(n)}.
$$

The [Nakayama lemma](nakayama-lemma.md) applied to $\mathfrak q^{(n)}/\mathfrak q^{(n+1)}$ gives $\mathfrak q^{(n)}=\mathfrak q^{(n+1)}$. Localizing at $\mathfrak q$ would therefore make the powers of the nonzero maximal ideal $\mathfrak qR_{\mathfrak q}$ stabilize at a nonzero ideal, contradicting the [Krull intersection theorem](krull-intersection-theorem.md) for the Noetherian local domain $R_{\mathfrak q}$.

**Table of contents**

- [Principal prime in a Noetherian local ring lemma](principal-prime-in-a-noetherian-local-ring-lemma.md)
- [Krull height theorem](krull-height-theorem.md)
  - [Generator bound for primary-ideal length](generator-bound-for-primary-ideal-length.md)
- [Prime ideals between a three-prime chain](prime-ideals-between-a-three-prime-chain.md)
  - [Infinitude of intermediate-height prime ideals](infinitude-of-intermediate-height-prime-ideals.md)

## ↑ Ancestors (7)

1. [Height of an ideal](height-of-an-ideal.md)
2. [Krull dimension](krull-dimension.md)
3. [Commutative algebra](commutative-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Krull height theorem](krull-height-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-13/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-16/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-113/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-148/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-101/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-101/5/i/solution.md)
- [Prime ideals between a three-prime chain](prime-ideals-between-a-three-prime-chain.md)
