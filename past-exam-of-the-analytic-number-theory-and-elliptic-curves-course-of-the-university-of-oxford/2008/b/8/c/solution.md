<h1 id="b/8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [prescribing a factor by elliptic-curve tripling](../../../../../prescribing-a-factor-by-elliptic-curve-tripling.md), [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives $(3/p)=1$ when $p\equiv1\pmod{12}$. Choose $r\in\mathbb F_p$ with $r^2=3$ and choose an [integer](../../../../../integer-split.md) $a$ by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) so that

$$
a\equiv-3+2r\pmod p,\qquad a\equiv1\pmod q.
$$

Then $a^2+6a-3\equiv0\pmod p$ and it is four modulo $q$.

The curve $E:y^2=x^3+ax-a$ has [discriminant](../../../../../discriminant.md) $-16a^2(4a+27)$. At $p$, $a\ne0$, since otherwise $r=3/2$ would force $p=3$. Also $4a+27=15+8r$ cannot vanish: squaring $8r=-15$ would give $192=225\pmod p$, forcing $p=3$ or 11, neither in the required class. At $q$, $a=1$ makes $a(4a+27)=31$, and $q\equiv5\pmod{12}$ excludes $q=31$. Thus both reductions are nonsingular.

The point $P=(1,1)$ is on every curve in this family. Doubling it uses the invertible denominator two and gives

$$
x(2P)=\frac{a^2+6a+1}4,\qquad x(2P)-x(P)=\frac{a^2+6a-3}4.
$$

Modulo $p$ this difference vanishes, and the doubling ordinate is $-1$, so $2P=-P$ and $3P$ is the identity. Modulo $q$, taking $a=1$ gives $x(2P)=2$, so $2P$ and $P$ have distinct abscissas and their sum is a finite point.

Consequently the attempted addition computing $3P$ modulo $N$ asks to invert a denominator divisible by $p$ and not by $q$. Its numerator is nonzero modulo $p$, since the two ordinates there are minus one and one, so this is not a removable coincidence. The Euclidean gcd used for inversion returns

$$
\boxed{\gcd(a^2+6a-3,N)=p,}
$$

a proper factor. Thus the specified elliptic-curve computation successfully factors $N$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
