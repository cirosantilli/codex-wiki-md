<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md) assigns to $a$ in a unital complex Banach algebra and every function holomorphic near $\sigma(a)$ the element

$$
f(a)=\frac1{2\pi i}\int_\Gamma f(z)(z1-a)^{-1}\,dz,
$$

where $\Gamma$ winds once around the spectrum. It is a unital algebra homomorphism, extends polynomial evaluation, is independent of the admissible contour, and obeys the [spectral mapping theorem](../../../../../spectral-mapping-theorem.md)

$$
\sigma(f(a))=f(\sigma(a)).
$$

Let $z_K\in\mathcal R(K)$ be the coordinate function. For a character $\varphi$, put $\lambda=\varphi(z_K)$. If $\lambda\notin K$, then $(z_K-\lambda)^{-1}$ is one of the admitted rational functions, contradicting the fact that $z_K-\lambda$ lies in the kernel of $\varphi$. Thus $\lambda\in K$. For every rational function $r$ without poles on $K$,

$$
\varphi(r)=r(\lambda).
$$

Continuity of characters and uniform density extend this identity to every member of $\mathcal R(K)$. Conversely evaluation at every $\lambda\in K$ is a character. Therefore the [character space of R(K)](../../../../../character-space-of-r-k.md) is naturally $K$.

[Runge approximation theorem](../../../../../runge-s-theorem.md) says that if $K\subset\mathbb C$ is compact, $f$ is holomorphic on a neighbourhood of $K$, and one chooses one point in every bounded component of $\mathbb C\setminus K$, then $f$ can be approximated uniformly on $K$ by rational functions whose finite poles belong only to the chosen points.

To prove it, surround $K$ by finitely many small rectangles contained in the domain of $f$ and apply the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) on their oriented boundaries:

$$
f(z)=\frac1{2\pi i}\int_\Gamma\frac{f(\zeta)}{\zeta-z}\,d\zeta.
$$

Riemann sums approximate this integral uniformly on $K$ by rational functions with poles on $\Gamma$. If a pole $b$ lies in a component containing the selected point $a$, choose a polygonal path from $b$ to $a$ inside that component and subdivide it finely. The resolvent identity

$$
\frac1{z-b}-\frac1{z-c}
=\frac{b-c}{(z-b)(z-c)}
$$

allows the pole to be moved step by step along the path, with arbitrarily small uniform error on $K$. Moving every pole proves the theorem.

For an open set $U$, choose a compact exhaustion $K_1\subset K_2\subset\cdots$ such that every component of $\mathbb C\setminus K_n$ meets $\mathbb C\setminus U$. Runge's theorem approximates a holomorphic function on $K_n$ by a rational function with all poles outside $U$. A diagonal choice gives convergence uniformly on every compact subset, proving that such rational functions are dense in the [space of holomorphic functions](../../../../../space-of-holomorphic-functions.md) $\mathcal O(U)$ with its compact-open topology.

Finally, equality of the [Gelfand transforms](../../../../../gelfand-representation.md) gives

$$
\sigma_A(x_1)=\{\widehat{x_1}(\varphi):\varphi\in\Phi_A\}
=\{\widehat{x_2}(\varphi):\varphi\in\Phi_A\}
=\sigma_A(x_2).
$$

Let this common compact spectrum be $K$. The divided difference

$$
g(z,w)=
\begin{cases}
\dfrac{f(z)-f(w)}{z-w},&z\ne w,\\
f'(z),&z=w
\end{cases}
$$

is holomorphic near $K\times K$. The two-variable holomorphic functional calculus for the commuting pair $(x_1,x_2)$ gives an element $u=g(x_1,x_2)$ satisfying

$$
f(x_1)-f(x_2)=u(x_1-x_2).
$$

For every character,

$$
\widehat u(\varphi)
=g(\widehat{x_1}(\varphi),\widehat{x_2}(\varphi))
=f'(\widehat{x_1}(\varphi))\ne0.
$$

An element of a commutative unital Banach algebra is invertible exactly when its Gelfand transform has no zero. Thus $u$ is invertible, and $f(x_1)=f(x_2)$ implies $x_1=x_2$. This is [injectivity through a holomorphic functional calculus with nonvanishing derivative](../../../../../injectivity-through-a-holomorphic-functional-calculus-with-nonvanishing-derivative.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
