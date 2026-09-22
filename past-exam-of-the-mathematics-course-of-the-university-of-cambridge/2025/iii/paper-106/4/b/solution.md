<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The seminorms in $\mathcal R$ have inverse images of intervals that constrain one coordinate at a time. Finite intersections of these sets are exactly the standard basic neighbourhoods for the product topology, so $(X\times Y,\mathcal R)$ is the [product of locally convex spaces](../../../../../../product-of-locally-convex-spaces.md). If $F\in(X\times Y)^*$, then

$$
f(x)=F(x,0),
\qquad
g(y)=F(0,y)
$$

belong to $X^*$ and $Y^*$ and $F(x,y)=f(x)+g(y)$. Conversely every such pair defines a continuous functional, so $(X\times Y)^*=X^*\oplus Y^*$.

For the open convex sets $K_1,\ldots,K_n$, consider

$$
C=\{(x_1-x_n,\ldots,x_{n-1}-x_n):x_i\in K_i\}\subseteq X^{n-1}.
$$

This set is open and convex, and $0\notin C$ because the $K_i$ have empty intersection. Separate $0$ from $C$ by a continuous linear functional on the product. By the dual description just proved, it has the form

$$
L(z_1,\ldots,z_{n-1})=\sum_{j=1}^{n-1}f_j(z_j)
$$

for $f_j\in X^*$, and $L$ is nonzero with one strict sign on $C$. Define

$$
T:X\to\mathbb R^{n-1},
\qquad
T(x)=(f_1(x),\ldots,f_{n-1}(x)).
$$

If some vector belonged to every $T(K_i)$, choose $x_i\in K_i$ with the same image. Then every $f_j(x_j-x_n)=0$, making $L(x_1-x_n,\ldots,x_{n-1}-x_n)=0$, a contradiction. Hence $\bigcap_iT(K_i)=\varnothing$, proving [finite-dimensional separation of open convex sets](../../../../../../finite-dimensional-separation-of-open-convex-sets.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
