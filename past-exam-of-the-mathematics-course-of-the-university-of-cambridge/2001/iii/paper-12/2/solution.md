<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $i:M\hookrightarrow N$ be an embedded [submanifold](../../../../../submanifold.md). In the general terminology, a [vector field along a map](../../../../../vector-field-along-a-map.md) $i$ is a smooth section $X\in\Gamma(i^*TN)$, so $X_p\in T_pN$. A [local extension of a vector field along a submanifold](../../../../../local-extension-of-a-vector-field-along-a-submanifold.md) near $p$ is a [vector field](../../../../../vector-field.md) $\widetilde X$ on an open neighbourhood in $N$ with $\widetilde X|_M=X$ on that neighbourhood. Choose adapted coordinates $(x^1,\ldots,x^m,y^{m+1},\ldots,y^n)$ in which $M$ is given by $y=0$. Writing $X=X^a(x)\partial_a|_{y=0}$, extend the coefficient functions independently of $y$:

$$
\widetilde X(x,y)=\sum_aX^a(x)\partial_a.
$$

This proves local existence, including for fields with normal components.

For the [Lie bracket](../../../../../lie-bracket.md) assertion, the fields must be tangent to $M$, namely sections of $TM$ viewed inside $i^*TN$. In this case the useful criterion for a [local extension of a vector field along a submanifold](../../../../../local-extension-of-a-vector-field-along-a-submanifold.md) is

$$
\boxed{(\widetilde XF)|_M=X(F|_M)\quad\text{for every local smooth function }F\text{ on }N.}
$$

If $\widetilde X$ extends $X$, the [chain rule](../../../../../chain-rule.md) gives this identity because their tangent values agree. Conversely, applying it to the adapted coordinate functions forces the tangent components to equal those of $X$ and all normal components on $M$ to vanish, so $\widetilde X|_M=X$. The criterion also shows that functions vanishing on $M$ are differentiated to functions vanishing on $M$ by $\widetilde X$.

For tangent [vector fields](../../../../../vector-field.md) $X,Y$ and local extensions $\widetilde X,\widetilde Y$, apply the criterion twice:

$$
\begin{aligned}
([\widetilde X,\widetilde Y]F)|_M
&=X\bigl((\widetilde YF)|_M\bigr)-Y\bigl((\widetilde XF)|_M\bigr)\\
&=X\bigl(Y(F|_M)\bigr)-Y\bigl(X(F|_M)\bigr)\\
&=[X,Y](F|_M).
\end{aligned}
$$

Hence **the ambient bracket restricts to the intrinsic bracket, independently of the chosen extensions**. Tangency is essential. For example, on the $x$-axis in $\mathbb R^2$, let $X=\partial_y|_M$ and $Y=0|_M$. The two extensions $\widetilde Y=0$ and $\widetilde Y=y\partial_x$, with $\widetilde X=\partial_y$, give bracket restrictions $0$ and $\partial_x|_M$. Thus general sections with normal components do not possess the extension-independent [Lie bracket](../../../../../lie-bracket.md) asserted for tangent fields.

For the [hypersurface](../../../../../hypersurface.md) $M^n\subset\mathbb R^{n+1}$, choose a smooth unit normal $\nu$ locally. A global choice is needed only if one wants a globally signed [shape operator](../../../../../shape-operator.md); an arbitrary [hypersurface](../../../../../hypersurface.md) need not come equipped with such a choice. With $D$ the Euclidean [Levi-Civita connection](../../../../../levi-civita-connection.md), define the [shape operator](../../../../../shape-operator.md), also called the [Weingarten map](../../../../../shape-operator.md), by

$$
\boxed{S_p:T_pM\to T_pM,\qquad S_p(v)=-D_v\nu.}
$$

The derivative is defined along $M$ and is linear in $v$. Since $v\langle\nu,\nu\rangle=2\langle D_v\nu,\nu\rangle=0$, its value is tangent to $M$, so this is an endomorphism of the [tangent space](../../../../../tangent-space.md). Differentiating $\langle\nu,Y\rangle=0$ gives, for tangent [vector fields](../../../../../vector-field.md) $X,Y$,

$$
h(X,Y):=\langle SX,Y\rangle=\langle\nu,D_XY\rangle.
$$

This is the scalar [second fundamental form](../../../../../second-fundamental-form-split.md) for the chosen normal. The Euclidean [connection on a vector bundle](../../../../../connection-vector-bundle.md) has zero [torsion tensor](../../../../../torsion-tensor.md), giving $D_XY-D_YX=[X,Y]$. The bracket is tangent to $M$ by the previous argument; therefore

$$
h(X,Y)-h(Y,X)=\langle\nu,[X,Y]\rangle=0.
$$

Consequently $\boxed{\langle S_pv,w\rangle=\langle v,S_pw\rangle}$ for every $v,w\in T_pM$: the [shape operator](../../../../../shape-operator.md) is [self-adjoint](../../../../../self-adjoint-operator.md). Reversing $\nu$ reverses $S$ and $h$ but preserves this self-adjointness.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
