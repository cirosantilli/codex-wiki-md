<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [polynomial ring](../../../polynomial-ring.md), use the [Euclidean function](../../../euclidean-function.md) $\delta(f)=\deg f$ on nonzero [polynomials](../../../polynomial-split.md). If $a,b\in F[X]$ and $b\ne0$, subtract the multiple of $b$ that cancels the leading term of $a$. The leading [coefficient](../../../coefficient.md) of $b$ is invertible in the [field](../../../field.md), and every subtraction strictly lowers the degree of the remainder. This process terminates with $a=qb+r$ and either $r=0$ or $\deg r<\deg b$. Thus $\boxed{F[X]\text{ is a Euclidean domain}}$.

For the [Gauss lemma for polynomials](../../../gauss-lemma-for-polynomials.md), call an [integer](../../../integer-split.md) [polynomial](../../../polynomial-split.md) [primitive](../../../primitive-polynomial.md) when its [coefficient](../../../coefficient.md) gcd is one. If two [primitive](../../../primitive-polynomial.md) [polynomials](../../../polynomial-split.md) had a nonprimitive product, a prime $p$ would divide every product [coefficient](../../../coefficient.md). Reducing modulo $p$ would give a zero product of two nonzero [polynomials](../../../polynomial-split.md) in the [integral domain](../../../integral-domain.md) $\mathbb F_p[X]$, a contradiction. Therefore **the product of [primitive](../../../primitive-polynomial.md) [integer](../../../integer-split.md) [polynomials](../../../polynomial-split.md) is [primitive](../../../primitive-polynomial.md)**.

To transfer a rational factorization, write each nonzero rational factor as a rational scalar times a [primitive](../../../primitive-polynomial.md) [integer](../../../integer-split.md) [polynomial](../../../polynomial-split.md) by clearing denominators and removing the [coefficient](../../../coefficient.md) gcd. Thus $f=qAB$ with [primitive](../../../primitive-polynomial.md) $A,B\in\mathbb Z[X]$ and $q\in\mathbb Q$. Their product is [primitive](../../../primitive-polynomial.md) by the lemma. If $q=m/n$ in lowest terms, integrality of every [coefficient](../../../coefficient.md) of $f$ forces $n$ to divide every [coefficient](../../../coefficient.md) of $AB$, so $n=1$. Hence $q\in\mathbb Z$; absorbing $q$ into either factor produces the required [integer](../../../integer-split.md) factorization with the same positive factor degrees. In particular irreducibility of a [primitive polynomial](../../../primitive-polynomial.md) over $\mathbb Z$ and over $\mathbb Q$ is equivalent.

Finally, let $a/b$ in lowest terms, $b>0$, be a rational root of a monic degree-$d$ [integer](../../../integer-split.md) [polynomial](../../../polynomial-split.md). Multiplying the equation by $b^d$ shows $b\mid a^d$. [Coprimality](../../../coprime-integers.md) forces $b=1$. Thus $\boxed{\text{every rational root of a monic integer polynomial is an integer}}$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2008 printed variant](../../2008-printed-variant-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
