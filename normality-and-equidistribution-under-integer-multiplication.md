# Normality and equidistribution under integer multiplication

↑ **Parent:** [Normal number](normal-number.md)

A [real number](real-number.md) $x$ is a [normal number](normal-number.md) in base $K$ exactly when its iterates under the [integer multiplication map on the circle](integer-multiplication-map-on-the-circle.md), $T_K(x)=\{Kx\}$, form an [equidistributed sequence](equidistributed-sequence.md). Braces denote the [fractional part](fractional-part.md). Multiplication by $K$ shifts the [positional notation](positional-notation.md) one digit to the left:

$$
T_K^n(x)=\{K^nx\}=0.d_{n+1}d_{n+2}\ldots\quad\text{in base }K.
$$

A length-$r$ [word](string.md) with base-$K$ [integer](integer.md) value $a$ specifies the half-open [interval](interval-mathematics.md) $[a/K^r,(a+1)/K^r)$, whose length is $K^{-r}$. Visiting that [interval](interval-mathematics.md) is exactly encountering that [word](string.md) at the next digit position. These digit [intervals](interval-mathematics.md) form arbitrarily fine grids, so their correct limiting visiting frequencies imply [equidistribution](equidistributed-sequence.md) on every [interval](interval-mathematics.md). This converts a question about digits into one about a [dynamical system](dynamical-system.md). Bailey and Crandall develop this connection using [equidistribution](equidistributed-sequence.md) of the [fractional parts](fractional-part.md) of $K^nx$. [David H. Bailey and Richard E. Crandall, Random Generators and Normal Numbers, 2003 author manuscript, Section 2](https://www.davidhbailey.com/dhbpapers/bcnormal.pdf)

In base ten the [word](string.md) $12$ corresponds to $[0.12,0.13)$. For [Champernowne constant](champernowne-constant.md), counting the visits $T_{10}^n(x)$ for $0\leq n\leq99998$ gives precisely the $2088$ occurrences of $12$ in its first $100000$ digits. For $x=1/3$, the base-two [integer multiplication map on the circle](integer-multiplication-map-on-the-circle.md) instead alternates between $1/3$ and $2/3$; it never visits $[0,1/4)$, the [interval](interval-mathematics.md) for $00$. This two-point [orbit](orbit-dynamical-system.md) is not an [equidistributed sequence](equidistributed-sequence.md).

## ↑ Ancestors (5)

1. [Normal number](normal-number.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fractional part](fractional-part.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/4/solution.md)
