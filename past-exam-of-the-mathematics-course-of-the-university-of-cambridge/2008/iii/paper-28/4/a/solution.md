<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [congruent number](../../../../../../congruent-number.md) is a positive integer which occurs as the area of a [right triangle](../../../../../../right-triangle.md) with positive rational side lengths. Scaling a triangle by a nonzero rational factor multiplies its area by a rational square, so the essential parameter is its positive square class; integer parameters can be reduced to [square-free integers](../../../../../../square-free-integer.md). For example $6$ is congruent by the triangle $(3,4,5)$, and $5$ is congruent by $(3/2,20/3,41/6)$.

The connection with [elliptic curves](../../../../../../elliptic-curve.md) comes from the [congruent number elliptic curve](../../../../../../congruent-number-elliptic-curve.md) in the model

$$
E_N:\quad y^2=x^3-N^2x.
$$

From a rational point with $y\ne0$, define

$$
a=\left|\frac{x^2-N^2}{y}\right|,\qquad
b=\left|\frac{2Nx}{y}\right|,\qquad
c=\left|\frac{x^2+N^2}{y}\right|.
$$

Direct squaring gives $a^2+b^2=c^2$, and its area is

$$
\frac{ab}{2}=\frac{N|x(x^2-N^2)|}{y^2}=N.
$$

Conversely, from a positive rational triangle $(a,b,c)$ of area $N$, put

$$
x=N\frac{c+a}{b},\qquad y=2N^2\frac{c+a}{b^2}.
$$

Substitution using $c^2=a^2+b^2$ and $ab=2N$ gives $y^2=x^3-N^2x$ and $y\ne0$. Thus

$$
\boxed{N\text{ congruent}\iff E_N(\mathbb Q)\text{ has a point with }y\ne0.}
$$

The standard [rational torsion of a congruent number curve](../../../../../../rational-torsion-of-a-congruent-number-curve.md) consists of $O,(0,0),(N,0),(-N,0)$. One way to see the torsion restriction is to use good primes $p\equiv3\pmod4$. The character sum cancels at $x$ and $-x$, giving $\#E_N(\mathbb F_p)=p+1$. For any odd prime $\ell$, the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) supplies good primes with $p\equiv3\pmod4$ and $p\equiv1\pmod\ell$, so the [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) excludes $\ell$-torsion. Good primes $p\equiv3\pmod8$ similarly bound the two-primary torsion by four, and the four displayed points give equality. Consequently the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) turns the criterion into **positive rank of $E_N(\mathbb Q)$**. Arithmetic [two-descent on an elliptic curve](../../../../../../two-descent-on-an-elliptic-curve.md) and local obstructions are therefore tools for the congruent number problem, and a nontorsion point gives [infinitely many rational right triangles from a nontorsion point](../../../../../../infinitely-many-rational-right-triangles-from-a-nontorsion-point.md) by taking multiples.

We now give elementary proofs for $1$ and $2$, including the descent steps. Recall the [primitive Pythagorean parametrization](../../../../../../primitive-pythagorean-parametrization.md)

$$
A=2mn,\qquad B=m^2-n^2,\qquad C=m^2+n^2,
$$

where $m>n>0$ are coprime and of opposite parity. To derive it, in a primitive [Pythagorean triple](../../../../../../pythagorean-triple.md) put the even leg at $A$. The relatively prime integers $(C+B)/2,(C-B)/2$ have product $(A/2)^2$, so each is a square, say $m^2,n^2$. This gives the formulas and the parity condition. The area is $mn(m-n)(m+n)$, and its four factors are pairwise coprime: their common divisors reduce to divisors of $m,n$ or of two, while $m\pm n$ are odd.

**Area one is impossible.** Clearing denominators of a hypothetical rational triangle of area one gives an integer triangle with square area. Dividing out its common factor leaves a primitive integer triangle whose area is still a rational square; an integer which is a rational square is an integer square. Choose such a triangle with smallest hypotenuse. Pairwise coprimality in the area product forces

$$
m=r^2,\qquad n=s^2,\qquad m+n=u^2,\qquad m-n=v^2.
$$

The positive integers $u,v$ are odd and coprime. If $m$ were even, then $n$ would be odd and $u^2-v^2=2s^2$ would be $2$ modulo eight, whereas two odd squares have difference zero modulo eight. Hence $m$ is odd, $n$ is even and $s$ is even.

Now set $a=(u+v)/2$ and $b=(u-v)/2$. These are positive coprime integers and

$$
a^2+b^2=\frac{u^2+v^2}{2}=m=r^2,\qquad
\frac{ab}{2}=\frac{u^2-v^2}{8}=\frac{s^2}{4}.
$$

Thus $(a,b,r)$ is another integer [right triangle](../../../../../../right-triangle.md) with square area and hypotenuse $r$, strictly smaller than $m^2+n^2$. This contradicts the minimal choice and proves the [Fermat right triangle theorem](../../../../../../fermat-right-triangle-theorem.md). In particular **$1$ is not a congruent number**.

For area two we first establish the auxiliary descent [fourth-power sum cannot be a square](../../../../../../fourth-power-sum-cannot-be-a-square.md). Suppose $x^4+y^4=z^2$ with positive integers, and choose a primitive solution with smallest $z$. Two odd fourth powers sum to $2$ modulo sixteen, so after exchange $x$ is odd and $y$ is even. Parametrize the primitive triangle $(x^2,y^2,z)$:

$$
x^2=m^2-n^2,\qquad y^2=2mn,\qquad z=m^2+n^2.
$$

The case $m$ even, $n$ odd makes $x^2\equiv3\pmod4$, so $m$ is odd and $n$ even. Coprimality then gives $m=u^2$ and $n=2v^2$. Consequently

$$
x^2+(2v^2)^2=(u^2)^2.
$$

This second triangle is primitive, since $x$ is odd and $\gcd(x,v)=1$. Parametrize it as $x=r^2-s^2$, $2v^2=2rs$, $u^2=r^2+s^2$, with $r,s$ coprime. The equality $v^2=rs$ makes $r=a^2$, $s=b^2$. Thus

$$
a^4+b^4=u^2,
$$

a new positive solution with smaller hypotenuse $u<z=u^4+4v^4$. This contradicts [infinite descent](../../../../../../infinite-descent.md), proving the auxiliary assertion.

**Area two is also impossible.** Clearing denominators and removing a common factor now gives a primitive integer triangle with area twice an integer square. Indeed, if an integer is $2(a/b)^2$ with $\gcd(a,b)=1$, then $b^2$ divides two, forcing $b=1$. Its area product would satisfy

$$
mn(m-n)(m+n)=2t^2.
$$

The odd factors must be squares and the unique even factor twice a square. As in the preceding modulo-eight argument, $m$ even would force $m+n=c^2$, $m-n=d^2$ and $n=b^2$ odd, with $c^2-d^2=2b^2$, impossible modulo eight. Thus

$$
m=a^2,\qquad n=2b^2,\qquad m+n=c^2,\qquad m-n=d^2.
$$

The integers $u=(c+d)/2$ and $v=(c-d)/2$ are positive and coprime, and $uv=(c^2-d^2)/4=b^2$. Hence $u=r^2$, $v=s^2$. But

$$
a^2=m=\frac{c^2+d^2}{2}=u^2+v^2=r^4+s^4,
$$

contradicting the auxiliary descent. This proves [two is not a congruent number](../../../../../../two-is-not-a-congruent-number.md), and concludes

$$
\boxed{1\text{ and }2\text{ are not congruent numbers}.}
$$

The two obstructions are global arithmetic descents. The elliptic-curve correspondence organizes the wider problem, but by itself is not a substitute for proving these particular nonexistence assertions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
