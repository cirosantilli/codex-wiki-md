<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We first prove the algebraic extension step needed for [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md). Suppose $p$ is a finite [sublinear functional](../../../../../sublinear-function.md) on a real [vector space](../../../../../vector-space-split.md) and $g$ is a [linear functional](../../../../../linear-functional.md) on a [vector subspace](../../../../../vector-subspace.md) $W$, with $g\leq p$ there. For $v\notin W$, choose a real number $c$ between

$$
\sup_{w\in W}\{g(w)-p(w-v)\}
\quad\hbox{and}\quad
\inf_{w\in W}\{p(w+v)-g(w)\}.
$$

This interval is nonempty: for any $w,z\in W$,

$$
g(w)+g(z)=g(w+z)\leq p(w+z)\leq p(w-v)+p(z+v).
$$

Taking $w=0$ or $z=0$ also bounds the endpoints by finite numbers. Define $\widetilde g(w+tv)=g(w)+tc$. For $t>0$, the upper bound for $c$, applied to $w/t$, proves $\widetilde g(w+tv)\leq p(w+tv)$. For $t<0$, writing $t=-s$ and using the lower bound at $w/s$ proves the same inequality. The case $t=0$ is the original domination. Thus a dominated [linear functional](../../../../../linear-functional.md) extends over one further direction. Order all dominated extensions by extension of their domains. A chain has its union as an upper bound, so [Zorn's lemma](../../../../../zorn-s-lemma.md) supplies a maximal extension. The one-direction argument shows its domain is the whole [vector space](../../../../../vector-space-split.md). This proves the required algebraic [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md), rather than assuming the separation result.

Choose $a\in A$, and put $C=A-a$. This is a [radially open convex set](../../../../../radially-open-convex-set.md) containing zero. It is absorbing: along each line through zero, sufficiently small multiples of any vector lie in $C$. Its [Minkowski functional](../../../../../minkowski-functional.md)

$$
p(x)=\inf\{t>0:x\in tC\}
$$

is finite and nonnegative. Positive homogeneity follows by rescaling $t$. If $x\in sC$ and $y\in tC$, convexity gives $x+y\in(s+t)C$, proving [subadditivity](../../../../../subadditive-sequence.md) by taking infima. Moreover,

$$
C=\{x:p(x)<1\}.
$$

Indeed, $p(x)<1$ gives $x\in sC$ for some $s<1$, hence $x\in C$ by convexity and $0\in C$. Conversely, radial openness at $x\in C$ permits $(1+\epsilon)x\in C$ for some $\epsilon>0$, giving $p(x)<1$.

Since $A\cap U=\varnothing$, $a\notin U$ and $u-a\notin C$ for every $u\in U$. Define a [linear functional](../../../../../linear-functional.md) on $U+\mathbb Ra$ by

$$
g(u+ta)=-t.
$$

It is well defined because $a\notin U$. For $t<0$, write $s=-t$; then $p(u+ta)=s\,p(u/s-a)\geq s=g(u+ta)$. For $t\geq0$, domination follows from $g(u+ta)\leq0\leq p(u+ta)$. The extension step therefore gives $L:V\to\mathbb R$ with $L\leq p$, $L|_U=0$ and $L(a)=-1$. If $x\in A$, then

$$
L(x)+1=L(x-a)\leq p(x-a)<1,
$$

so $L(x)<0$. Consequently

$$
\boxed{H=\ker L\supseteq U,\qquad H\cap A=\varnothing.}
$$

Because $L(a)\ne0$, this [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) has codimension one and is a [hyperplane](../../../../../hyperplane.md). This establishes the [geometric Hahn-Banach theorem for radially open sets](../../../../../geometric-hahn-banach-theorem-for-radially-open-sets.md) without assuming a norm or a topology on $V$.

For the [convex function](../../../../../convex-function.md), use its strict [epigraph](../../../../../epigraph.md) in $V\times\mathbb R$. It is nonempty and convex, and does not contain $(0,0)$. It is also radially open: on every affine line, a finite [convex function](../../../../../convex-function.md) is continuous. To justify this last fact, convexity orders secant slopes; on a smaller interval the slopes are bounded above and below by slopes to two fixed exterior endpoints, giving a local Lipschitz bound. Thus $t\mapsto f(x+ty)-\beta-ts$ is continuous, and a strict negative value persists near $t=0$.

Apply the separation theorem with the zero subspace. A nonzero separating [linear functional](../../../../../linear-functional.md) has form $L(x,\beta)=g(x)+c\beta$. Its values on the convex [epigraph](../../../../../epigraph.md) cannot have both signs, since a line segment would then meet its kernel. Choose the sign so that $L>0$ on the [epigraph](../../../../../epigraph.md). At $x=0$ and $\beta>0$ this gives $c>0$. Letting $\beta$ decrease to $f(x)$ yields $g(x)+cf(x)\geq0$. Therefore

$$
\boxed{l(x)=-g(x)/c\leq f(x)\quad\hbox{for every }x\in V.}
$$

The resulting [linear functional](../../../../../linear-functional.md) need not be nonzero: for example, the zero functional is the only linear minorant of $f(x)=x^2$ on $\mathbb R$.

Now suppose the norm and continuity hypotheses hold. Domination at $x$ and $-x$ gives

$$
-f(-x)\leq l(x)\leq f(x).
$$

If $x_n\in\ker l$ and $x_n\to x$ in norm, apply this inequality to $x-x_n$. Since $l(x-x_n)=l(x)$ and both bounding values tend to $f(0)=0$, we obtain $l(x)=0$. The [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) is therefore closed.

Finally, a [linear functional with closed kernel](../../../../../linear-functional-with-closed-kernel.md) on a [normed vector space](../../../../../normed-vector-space.md) is continuous. If $l=0$, this is immediate. Otherwise choose $v$ with $l(v)=1$ and put $M=\ker l$. Closedness gives $d=\operatorname{dist}(v,M)>0$. For $l(x)\ne0$, $x/l(x)-v\in M$, so $d\leq\|x\|/|l(x)|$. The same resulting bound holds when $l(x)=0$:

$$
\boxed{|l(x)|\leq d^{-1}\|x\|.}
$$

This proves continuity and explains exactly how closedness of the kernel is used.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
