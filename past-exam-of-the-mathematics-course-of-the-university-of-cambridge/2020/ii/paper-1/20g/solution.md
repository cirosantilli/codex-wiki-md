<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

The [Minkowski convex body theorem](../../../../../minkowski-s-theorem.md) states that if $\Lambda\subset\mathbb R^n$ is a full [lattice](../../../../../lattice.md) and $C$ is a measurable, convex, centrally symmetric set with

$$
\operatorname{vol}(C)>2^n\operatorname{covol}(\Lambda),
$$

then $C$ contains a nonzero point of $\Lambda$.

Here $d\not\equiv3\pmod4$, so the [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) is

$$
\mathcal O_K=\mathbb Z[\sqrt{-d}].
$$

Under its complex embedding it has real-lattice covolume $\sqrt d$. An integral ideal $I$ has index $N(I)$ in $\mathcal O_K$, so its covolume is $\sqrt d\,N(I)$. Apply Minkowski's theorem to the disk $|z|\le R$, whose area is $\pi R^2$. Taking $R^2$ down to $4\sqrt d\,N(I)/\pi$ gives a nonzero $\alpha\in I$ with

$$
|\alpha|^2\le\frac{4\sqrt d}{\pi}N(I).
$$

Since the [field norm](../../../../../field-norm.md) is $N_{K/\mathbb Q}(\alpha)=|\alpha|^2$ in this imaginary quadratic field, this proves the [imaginary quadratic Minkowski disk bound](../../../../../imaginary-quadratic-minkowski-disk-bound.md)

$$
\boxed{0<|N_{K/\mathbb Q}(\alpha)|
\le\frac{4\sqrt d}{\pi}N(I)}.
$$

Because $(\alpha)\subseteq I$, the ideal

$$
J=(\alpha)I^{-1}
$$

is integral, represents the inverse class of $I$, and has

$$
N(J)=\frac{|N_{K/\mathbb Q}(\alpha)|}{N(I)}
\le\frac{4\sqrt d}{\pi}.
$$

Thus every ideal class has a [bounded-norm representative](../../../../../bounded-norm-ideal-representatives.md). Only finitely many integral ideals have bounded norm, proving the [finiteness of the ideal class group](../../../../../finiteness-of-the-ideal-class-group.md).

Now take $K=\mathbb Q(\sqrt{-22})$. Its ring of integers is $\mathbb Z[\sqrt{-22}]$, its discriminant is $-88$, and

$$
\frac{4\sqrt{22}}{\pi}<6.
$$

Every class therefore has an integral representative of norm at most five. The polynomial $X^2+22$ is irreducible modulo three and modulo five, so both primes are inert and there are no ideals of norm three or five. At two it reduces to $X^2$, and the [splitting of rational primes in a quadratic field](../../../../../splitting-of-rational-primes-in-a-quadratic-field.md) gives

$$
(2)=\mathfrak p_2^2,
\qquad
\mathfrak p_2=(2,\sqrt{-22}),
\qquad
N(\mathfrak p_2)=2.
$$

An ideal of norm four is $\mathfrak p_2^2=(2)$ and is principal. The ideal $\mathfrak p_2$ is not principal, since a generator would have norm two, whereas

$$
a^2+22b^2=2
$$

has no integer solution. Consequently the [Ideal class group of Q of square root of minus twenty-two](../../../../../ideal-class-group-of-q-of-square-root-of-minus-twenty-two.md) is

$$
\boxed{\operatorname{Cl}(\mathbb Q(\sqrt{-22}))\cong C_2}.
$$

Suppose finally that $y^3=x^2+22$. If $x$ were even, the right-hand side would be $2$ modulo four, which is not a cube modulo four. Hence $x$ and $y$ are odd. In $\mathcal O_K$,

$$
(x+\sqrt{-22})(x-\sqrt{-22})=(y)^3.
$$

The two ideals on the left are coprime. Indeed, a common prime ideal would divide both $2x$ and $2\sqrt{-22}$. It cannot lie above two because their norms are odd. It would therefore lie above eleven and force $11\mid x$; but then $x^2+22$ has $11$-adic valuation exactly one, impossible for the cube $y^3$.

By [unique factorization of ideals in a number field](../../../../../unique-factorization-of-ideals-in-a-number-field.md), coprimality implies

$$
(x+\sqrt{-22})=\mathfrak a^3
$$

for some ideal $\mathfrak a$. The class group has order two, so it has no element of order three; $[\mathfrak a]^3=1$ therefore forces $\mathfrak a$ to be principal. The only units are $\pm1$, both of which can be absorbed into a cube, and hence

$$
x+\sqrt{-22}=(a+b\sqrt{-22})^3
$$

for integers $a,b$. Comparing the coefficient of $\sqrt{-22}$ gives

$$
b(3a^2-22b^2)=1.
$$

Thus $b=\pm1$. For $b=1$ this requires $3a^2=23$, and for $b=-1$ it requires $3a^2=21$; neither is possible. Therefore the result on [no integral solutions to y cubed equals x squared plus twenty-two](../../../../../no-integral-solutions-to-y-cubed-equals-x-squared-plus-twenty-two.md) is

$$
\boxed{y^3=x^2+22\text{ has no integer solutions}}.
$$

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
