# Quadratic reciprocity

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_reciprocity)

Quadratic reciprocity compares two questions: is the [prime number](prime-number-split.md) $p$ a [quadratic residue](quadratic-residue-split.md) modulo $q$, and is $q$ a [quadratic residue](quadratic-residue-split.md) modulo $p$? Let $p,q$ be **distinct [odd primes](odd-prime.md)**. In terms of the [Legendre symbol](legendre-symbol.md),

$$
\left(\frac pq\right)\left(\frac qp\right)
=(-1)^{\frac{p-1}{2}\frac{q-1}{2}}.
$$

**The two [Legendre symbols](legendre-symbol.md) have opposite signs exactly when both [primes](prime-number-split.md) are $3$ modulo $4$; otherwise they are equal.** Their values are nonzero because the [primes](prime-number-split.md) are distinct. Equal signs can mean two [quadratic residues](quadratic-residue-split.md) or two [quadratic nonresidues](quadratic-nonresidue.md): reciprocity compares the answers rather than declaring either answer positive.[T. M. Apostol, Chapter 27, §27.9, equation 27.9.3: distinct odd prime hypotheses and reciprocity law](nist-digital-library-of-mathematical-functions.md)

For a direct computation, the nonzero [quadratic residues](quadratic-residue-split.md) modulo $3,5,7$ are respectively $\{1\}$, $\{1,4\}$, and $\{1,2,4\}$. Squaring just $1,\ldots,(p-1)/2$ suffices because $x$ and $p-x$ have the same square modulo an [odd prime](odd-prime.md) $p$.

$$
\begin{aligned}
\left(\frac37\right)&=-1,&\qquad \left(\frac73\right)&=\left(\frac13\right)=1,\\
\left(\frac57\right)&=-1,&\qquad \left(\frac75\right)&=\left(\frac25\right)=-1.
\end{aligned}
$$

The pair $3,7$ has a sign flip, whereas $5,7$ has two negative signs. These small [quadratic residue](quadratic-residue-split.md) tables make the distinction tangible.

<a id="image-small-prime-square-residue-tables-distinguish-opposite-and-equal-legendre-symbol-signs"></a>
![](quadratic-reciprocity-small-prime-residues.png)

**[Figure 17](#image-small-prime-square-residue-tables-distinguish-opposite-and-equal-legendre-symbol-signs). Small prime square-residue tables distinguish opposite and equal Legendre symbol signs**. Each row uses half the nonzero inputs; the missing entries are unnecessary. The comparisons $3,7$ and $5,7$ are exact finite examples of [quadratic reciprocity](quadratic-reciprocity.md), not evidence by themselves for every [prime](prime-number-split.md) pair.

The [first supplementary law for quadratic reciprocity](first-supplementary-law-for-quadratic-reciprocity.md) handles numerator $-1$, and the [second supplementary law for quadratic reciprocity](second-supplementary-law-for-quadratic-reciprocity.md) handles numerator $2$:

$$
\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2},\qquad
\left(\frac2p\right)=(-1)^{(p^2-1)/8}.
$$

For an [odd prime](odd-prime.md) $p$, $-1$ is a [quadratic residue](quadratic-residue-split.md) exactly when $p\equiv1\pmod4$, while $2$ is a [quadratic residue](quadratic-residue-split.md) exactly when $p\equiv1,7\pmod8$. The remaining odd [congruence classes](congruence-class.md) modulo $8$, namely $3,5$, make $2$ a [quadratic nonresidue](quadratic-nonresidue.md). These laws fill the cases excluded from swapping distinct [odd primes](odd-prime.md).[T. M. Apostol, Chapter 27, §27.9, equations 27.9.1–27.9.2: supplementary values](nist-digital-library-of-mathematical-functions.md)

**Table of contents**

- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Lattice-point count for quadratic reciprocity](lattice-point-count-for-quadratic-reciprocity.md)
- [Quadratic character of minus three](quadratic-character-of-minus-three.md)
  - [Cube roots of minus one modulo an odd prime](cube-roots-of-minus-one-modulo-an-odd-prime.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Jacobi reciprocity law](jacobi-reciprocity-law.md)
- [Lattice-point count for quadratic reciprocity](lattice-point-count-for-quadratic-reciprocity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-25/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/11i/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/10g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/1g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3/1g/solution.md)
- [Pépin's test](pepin-s-test.md)
- [Primes represented by x squared plus three y squared](primes-represented-by-x-squared-plus-three-y-squared.md)
- [Quadratic reciprocity](quadratic-reciprocity.md)
