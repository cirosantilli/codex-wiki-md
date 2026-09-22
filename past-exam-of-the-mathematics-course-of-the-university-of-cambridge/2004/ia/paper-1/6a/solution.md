<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and [Einstein summation convention](../../../../../einstein-notation.md), the [scalar triple product](../../../../../scalar-triple-product.md) is

$$
S=a_i\varepsilon_{ijk}a_jb_k.
$$

Interchange the dummy indices $i,j$. Antisymmetry gives $S=-a_j\varepsilon_{ijk}a_ib_k=-S$, since $a_ia_j=a_ja_i$. Over the [real numbers](../../../../../real-number.md) this proves

$$
\boxed{a\cdot(a\times b)=0.}
$$

The normal [vector](../../../../../vector.md) to the first plane and the specified positive direction give $a=(1,1,1)$. Then $a\cdot m=3$ and $a\times m=(1,1,-2)$, so

$$
b=(3,3,-6),\qquad a+b=(4,4,-5).
$$

Next $a\times b=(-9,9,0)$. A [vector](../../../../../vector.md) perpendicular to both $a$ and $b$ is a scalar multiple of their [cross product](../../../../../cross-product.md); the required length gives the two possibilities $c=(-2,2,0)$ and $c=(2,-2,0)$. The original PDF specifies approach to the **x-axis**. From $(4,4,-5)$ the original squared distance to that axis is $4^2+(-5)^2=41$. The two candidate endpoint squared distances are $6^2+(-5)^2=61$ and $2^2+(-5)^2=29$. Hence $c=(2,-2,0)$.

Adding the given $d$ yields $(7,0,-3)$. By the proved [scalar triple product](../../../../../scalar-triple-product.md) identity, $a\cdot b=3a\cdot(a\times m)=0$, so the only [vector](../../../../../vector.md) of the specified length for $e$ is the [zero vector](../../../../../zero-vector.md). Finally set $f=s\,m=(2s,0,s)$. The last point is $(7+2s,0,-3+s)$, and its plane condition becomes $2+8s=10$. Thus $s=1$ and $f=(2,0,1)$.

All waypoints, in the given distance units, are

$$
\begin{array}{c|c}
\text{stage}&\text{position}\\\hline
\text{start}&(0,0,0)\\
 a&(1,1,1)\\
 b&(4,4,-5)\\
 c&(6,2,-5)\\
 d&(7,0,-3)\\
 e&(7,0,-3)\\
 f&(9,0,-2)
\end{array}
$$

Therefore **the final location is $(9,0,-2)$**. The converted TeX omits two [vector](../../../../../vector.md) instructions and changes the axis; the computation above follows the original PDF.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
