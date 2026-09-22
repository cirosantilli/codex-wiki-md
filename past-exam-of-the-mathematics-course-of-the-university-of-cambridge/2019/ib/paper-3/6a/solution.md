<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Since

$$
f''(x)=(a-1)x^{a-2}>0
$$

for $x>0$, the second-derivative criterion shows that $f(x)=x^a/a$ is [strictly convex](../../../../../strictly-convex-function.md). Put $b=a/(a-1)$, so $1/a+1/b=1$. For dual variable $p>0$, the stationary equation in the [Legendre transform](../../../../../convex-conjugate.md) is

$$
p=f'(x)=x^{a-1},
\qquad x=p^{1/(a-1)}.
$$

It is the unique global maximizer of $px-f(x)$, and hence

$$
\boxed{f^*(p)=\frac{p^b}{b}},
\qquad p>0.
$$

Applying the same calculation with the conjugate exponent $b$ gives

$$
\boxed{(f^*)^*(x)=\frac{x^a}{a}=f(x)},
\qquad x>0.
$$

Under the [Legendre-Fenchel transform](../../../../../convex-conjugate.md) on all real dual variables, the same supremum additionally gives $f^*(p)=0$ for $p\leq0$.

Now take $a=r$, $b=s$, and apply the [Fenchel–Young inequality](../../../../../fenchel-young-inequality.md) $f(x)+f^*(y)\geq xy$. This yields [Young's inequality for products](../../../../../young-s-inequality-for-products.md)

$$
\boxed{\frac{x^r}{r}+\frac{y^s}{s}\geq xy}
$$

for positive $x,y$ and conjugate exponents $r,s$.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
