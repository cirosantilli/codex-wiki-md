<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

For $a\in U$, the [function](../../../../../function-split.md) $f:U\to\mathbb R^n$ is [differentiable](../../../../../differentiable-function.md) at $a$ if there is a [linear map](../../../../../linear-map.md) $A:\mathbb R^m\to\mathbb R^n$ such that

$$
f(a+h)=f(a)+Ah+r(h),
\qquad
\frac{\lVert r(h)\rVert}{\lVert h\rVert}\longrightarrow0
\quad\hbox{as }h\longrightarrow0.
$$

The [linear map](../../../../../linear-map.md) is unique and is the [Fréchet derivative](../../../../../frechet-derivative.md) $Df_a=A$. The [function](../../../../../function-split.md) is [continuously differentiable](../../../../../continuously-differentiable-function.md) at $a$ if it is [differentiable](../../../../../differentiable-function.md) on a [neighbourhood](../../../../../neighbourhood-mathematics.md) of $a$ and the map $x\mapsto Df_x$, with values in the space of [linear maps](../../../../../linear-map.md) equipped with the [operator norm](../../../../../operator-norm.md), is [continuous](../../../../../continuous-function.md) at $a$.

If $T:\mathbb R^m\to\mathbb R^n$ is linear, then

$$
T(a+h)-T(a)-T(h)=0.
$$

Consequently $DT_a=T$ at every $a$. The [derivative](../../../../../derivative.md) is a [constant function](../../../../../constant-function.md) of $a$, hence is continuous, so every [linear map](../../../../../linear-map.md) is continuously [differentiable](../../../../../differentiable-function.md) everywhere.

The [mean value inequality](../../../../../mean-value-inequality.md) says that if the [line segment](../../../../../line-segment.md) $[x,y]$ lies in $U$ and

$$
\lVert Df_z\rVert\leq M\qquad(z\in[x,y]),
$$

then

$$
\lVert f(y)-f(x)\rVert\leq M\lVert y-x\rVert.
$$

To prove it, put $v=f(y)-f(x)$. The claim is immediate if $v=0$. Otherwise set $e=v/\lVert v\rVert$ and apply the one-dimensional [mean value theorem](../../../../../mean-value-theorem.md) to the [real-valued function](../../../../../real-valued-function.md)

$$
\phi(t)=e\mathbin{\cdot}f\bigl(x+t(y-x)),
\qquad 0\leq t\leq1.
$$

For some $c\in(0,1)$, the [chain rule](../../../../../chain-rule.md) gives

$$
\begin{aligned}
\lVert f(y)-f(x)\rVert
&=\phi(1)-\phi(0)\\
&=e\mathbin{\cdot}Df_{x+c(y-x)}(y-x)\\
&\leq \lVert Df_{x+c(y-x)}\rVert\lVert y-x\rVert
\leq M\lVert y-x\rVert,
\end{aligned}
$$

as required.

Now suppose that $U$ is [open](../../../../../open-set.md) and [connected](../../../../../connected-space.md) and that $Df_a=0$ for every $a\in U$. Every point has an [open ball](../../../../../open-ball.md) contained in $U$. The mean value inequality with $M=0$ shows that $f$ is constant on each such ball, so $f$ is [locally constant](../../../../../locally-constant-function.md). Fix $a_0\in U$. The [level set](../../../../../level-set.md)

$$
E=\{x\in U:f(x)=f(a_0)\}
$$

is nonempty and open in $U$; its complement is also open because $f$ is locally constant. Since $U$ is connected, $E=U$. This proves the [zero derivative on a connected open set](../../../../../zero-derivative-on-a-connected-open-set.md) result: $f$ is constant.

The [inverse function theorem](../../../../../inverse-function-theorem.md) states that if $f:U\to\mathbb R^m$ is continuously [differentiable](../../../../../differentiable-function.md), $a\in U$, and $Df_a$ is an [invertible linear map](../../../../../invertible-linear-map.md), then there are open neighbourhoods $V$ of $a$ and $W$ of $f(a)$ such that $f|_V:V\to W$ is a [bijection](../../../../../bijection.md) whose inverse is continuously [differentiable](../../../../../differentiable-function.md).

For the curve in the question, define the continuously [differentiable function](../../../../../differentiable-function.md)

$$
F(x,y)=x^2+y+\cos(xy)-1.
$$

Then

$$
F(0,0)=0,
\qquad
\frac{\partial F}{\partial y}(x,y)=1-x\sin(xy),
\qquad
\frac{\partial F}{\partial y}(0,0)=1\neq0.
$$

The [implicit function theorem](../../../../../implicit-function-theorem.md), which follows from the [inverse function theorem](../../../../../inverse-function-theorem.md) applied to $(x,y)\mapsto(x,F(x,y))$, therefore gives an [open interval](../../../../../open-interval.md) $I$ containing $0$, an open [neighbourhood](../../../../../neighbourhood-mathematics.md) $U_0$ of $(0,0)$, and a [continuously differentiable](../../../../../continuously-differentiable-function.md), hence [continuous](../../../../../continuous-function.md), [function](../../../../../function-split.md) $g:I\to\mathbb R$ such that

$$
\boxed{U_0\cap C
=\{(x,y)\in\mathbb R^2:x\in I,\ y=g(x)\}.}
$$

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
