<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Starting with $y_1=0$, choose $y_j\in A+A$ for as long as

$$
\left|(X+y_j)\mathbin{\backslash}\bigcup_{i<j}(X+y_i)\right|\geq\frac12|X|.
$$

The union of these translates lies in $X+2A$, whose size is at most $K^2|X|$ by part a. The first translate contributes $|X|$, and every later translate contributes at least $|X|/2$, so

$$
|X|+(m-1)\frac{|X|}{2}\leq K^2|X|,
\qquad m\leq2K^2-1.
$$

Let $Y=\{y_1,\ldots,y_m\}$. Maximality says that, for each $z\in A+A$, more than half of the elements $x\in X$ satisfy

$$
x+z\in X+y_i
$$

for some $y_i\in Y$. Given $z,z'\in A+A$, the two corresponding subsets of $X$ each have more than $|X|/2$ elements, so they intersect. For an $x$ in their intersection there are $x_i,x_j\in X$ and $y_i,y_j\in Y$ such that

$$
x+z=x_i+y_i,
\qquad x+z'=x_j+y_j.
$$

Subtracting gives

$$
z-z'=x_i-x_j+y_i-y_j\in A-A+Y-Y.
$$

As every element of $A+A-A-A$ is some $z-z'$, this proves

$$
\boxed{A+A-A-A\subseteq A-A+Y-Y.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
