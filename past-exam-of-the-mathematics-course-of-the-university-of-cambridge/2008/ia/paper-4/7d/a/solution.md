<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $x^2+y^2=0$ in the [field](../../../../../../field.md) $F$. If $y\ne0$, division by $y^2$ gives $(x/y)^2=-1$, contrary to the hypothesis. Hence $y=0$ and then $x^2=0$; the absence of nonzero [zero divisors](../../../../../../zero-divisor.md) in a [field](../../../../../../field.md) gives $x=0$. Therefore

$$
\boxed{x^2+y^2=0\Longrightarrow x=y=0.}
$$

For the stated operations on $F^2$, addition is an [abelian group](../../../../../../abelian-group.md) operation: [associativity](../../../../../../associative-property.md) and [commutativity](../../../../../../commutativity.md) hold componentwise, its identity is $(0,0)$, and the negative of $(x,y)$ is $(-x,-y)$.

To check multiplication without omitting associativity, associate to each pair the [matrix](../../../../../../matrix.md)

$$
M(x,y)=\begin{pmatrix}x&-y\\y&x\end{pmatrix}.
$$

This is an [injection](../../../../../../injective-function.md) into the two-by-two [matrices](../../../../../../matrix.md) over $F$, and direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives

$$
M(x,y)M(z,w)=M(xz-yw,xw+yz).
$$

It also preserves addition. The [associativity](../../../../../../associative-property.md) and distributivity of [matrix multiplication](../../../../../../matrix-multiplication.md) therefore imply the same laws for the pair multiplication. Its formula is symmetric in the pairs, so it is commutative. Its identity is $(1,0)$, which is different from $(0,0)$.

For a nonzero pair, the first result shows that $x^2+y^2\ne0$. Its multiplicative inverse is

$$
\boxed{(x,y)^{-1}=\left(\frac{x}{x^2+y^2},\frac{-y}{x^2+y^2}\right),}
$$

since multiplying $(x,y)$ by $(x,-y)$ gives $(x^2+y^2,0)$. This verifies every [field](../../../../../../field.md) axiom, so **the given operations make $F^2$ a [field](../../../../../../field.md)**. The embedded copy of $F$ is $\{(x,0):x\in F\}$; the element $(0,1)$ has square $(-1,0)$, describing a [quadratic extension](../../../../../../quadratic-extension.md) of $F$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
