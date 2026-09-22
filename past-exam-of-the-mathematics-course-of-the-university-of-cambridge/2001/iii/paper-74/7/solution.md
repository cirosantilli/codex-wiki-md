<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The original PDF has cube roots throughout this question; the ninth roots in the converted TeX are transcription errors. Put $\alpha=\sqrt[3]{m_1m_2^2}$ and $\beta=\alpha^2/m_2$. The given condition excludes the trivial cube case. Both generators are integral, because

$$
\alpha^3=m_1m_2^2,\qquad\beta^3=m_1^2m_2.
$$

Moreover

$$
\alpha^2=m_2\beta,\qquad\beta^2=m_1\alpha,\qquad\alpha\beta=m_1m_2,
$$

so $A=\mathbb Z+\mathbb Z\alpha+\mathbb Z\beta$ is an order in the cubic field. The [field traces](../../../../../field-trace.md) of $\alpha,\beta,\alpha^2,\beta^2$ are zero, while $\operatorname{Tr}(\alpha\beta)=3m_1m_2$. Thus the [trace pairing](../../../../../trace-pairing.md) matrix of this basis is

$$
\begin{pmatrix}3&0&0\\0&0&3m_1m_2\\0&3m_1m_2&0\end{pmatrix},\qquad\operatorname{disc}(A)=-27m_1^2m_2^2.
$$

We must prove that this is the maximal order, not just compute the discriminant of a suborder. The [discriminant-index formula for an integral lattice](../../../../../discriminant-index-formula-for-an-integral-lattice.md) restricts any index prime to those dividing $3m_1m_2$. If $p\mid m_1$, the cubic for $\alpha$ is [Eisenstein](../../../../../eisenstein-criterion.md) at $p$, while $m_2$ is a unit there and $A\otimes\mathbb Z_p=\mathbb Z_p[\alpha]$. If $p\mid m_2$, use instead the [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) for $\beta$, and $\alpha=\beta^2/m_1$. In either case an [Eisenstein](../../../../../eisenstein-criterion.md) generator is a [uniformizer](../../../../../uniformizer.md) of the totally ramified local field and generates its full valuation ring. Indeed expansion in powers of that uniformizer using base residue representatives, and grouping powers modulo three, expresses every integral local element in its power basis.

These arguments also cover three when $3\mid m_1m_2$. If $3\nmid m_1m_2$, every unit modulo nine has cube congruent to $1$ or $-1$. Therefore the condition $m_1\not\equiv\pm m_2\pmod9$ implies $m_1m_2^2\not\equiv\pm1\pmod9$: multiply a contrary congruence by the inverse of $m_2^2$ and use $m_2^3\equiv\pm1$. Choose $r\in\{1,-1\}$ with $r^3\equiv m_1m_2^2\pmod3$. The polynomial

$$
(X+r)^3-m_1m_2^2=X^3+3rX^2+3r^2X+(r^3-m_1m_2^2)
$$

is [Eisenstein](../../../../../eisenstein-criterion.md) at three, since its constant term is divisible by three but not nine. Its root $\alpha-r$ again generates the full local valuation ring. There is no index prime left. We have proved the [integral basis of a cubefree pure cubic field](../../../../../integral-basis-of-a-cubefree-pure-cubic-field.md) and the requested discriminant:

$$
\boxed{\mathcal O_K=\mathbb Z\oplus\mathbb Z\alpha\oplus\mathbb Z\beta,\qquad d_K=-27m_1^2m_2^2.}
$$

For $K=\mathbb Q(\sqrt[3]{6})$ write $\alpha^3=6$. Here $\mathcal O_K=\mathbb Z[\alpha]$ and $d_K=-972$. The norm of $x+y\alpha+z\alpha^2$ is the determinant of its multiplication matrix, giving

$$
N(x+y\alpha+z\alpha^2)=x^3+6y^3+36z^3-18xyz.
$$

In particular

$$
\boxed{u=1-6\alpha+3\alpha^2\text{ is a nontrivial unit},\qquad N(u)=1.}
$$

An integral element of norm one has an integral inverse, by its monic characteristic polynomial. Here direct multiplication gives $u^{-1}=109+60\alpha+33\alpha^2$. Nontriviality also follows from linear independence of $1,\alpha,\alpha^2$.

The signature is $(1,1)$, so the [Minkowski bound for ideal classes](../../../../../minkowski-s-bound.md) is

$$
\frac4\pi\frac{3!}{3^3}\sqrt{972}=\frac{16\sqrt3}{\pi}<9.
$$

Every class therefore has an integral representative of norm at most eight. Its prime factors have norms at most eight, and lie above $2,3,5,7$. Since the index of $\mathbb Z[\alpha]$ is one, reduction of $X^3-6$ gives their factorizations by the [Kummer-Dedekind theorem](../../../../../kummer-dedekind-theorem.md). At two and three the polynomial is $X^3$, so there is one prime of norm $2$ or $3$, respectively. They are principal, because

$$
|N(\alpha-2)|=2,\qquad N(3+2\alpha+\alpha^2)=3.
$$

At five the factorization is $(X-1)(X^2+X+1)$ with the quadratic irreducible. The norm-five prime is $(\alpha-1)$ because $N(\alpha-1)=5$; the norm-twenty-five prime is outside the bound.

At seven the roots are $3,5,6$, giving three primes $\mathfrak q_r=(7,\alpha-r)$ of norm seven. The elements $\alpha+1$ and $\alpha^2+\alpha-5$ have norm seven and vanish at roots six and three, respectively; hence they generate $\mathfrak q_6$ and $\mathfrak q_3$. Since $\mathfrak q_3\mathfrak q_5\mathfrak q_6=(7)$, the remaining prime is principal too. Every prime which can divide a Minkowski representative is now principal, so

$$
\boxed{h_{\mathbb Q(\sqrt[3]{6})}=1.}
$$

This proves [class number one for Q of cube root six](../../../../../class-number-one-for-q-of-cube-root-six.md) with all primes within the bound accounted for.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
