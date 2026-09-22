<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

For a [divisor](../../../../../divisor.md) $D$ on a [smooth projective curve](../../../../../smooth-projective-curve.md), let $L(D)=\{f\in k(X):\operatorname{div}(f)+D\ge0\}\cup\{0\}$, and write $\ell(D)=\dim_kL(D)$. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) states

$$
\boxed{\ell(D)-\ell(K_X-D)=\deg D+1-g,}
$$

where $g$ is the [genus](../../../../../genus-of-a-surface.md), $K_X$ is a [canonical divisor](../../../../../canonical-divisor.md) given by a nonzero rational differential, and the degree of a [divisor](../../../../../divisor.md) is the sum of its coefficients since $k$ is algebraically closed.

For [genus](../../../../../genus-of-a-surface.md) one, a nonzero regular differential has a nonnegative [divisor](../../../../../divisor.md) of degree $2g-2=0$, hence no zeros; therefore $K_X\sim0$. Negative-degree [divisors](../../../../../divisor.md) have no nonzero sections. Thus $\ell(nP_\infty)=n$ for $n>0$, $\ell(0)=1$, and $L(nP_\infty)=0$ for $n<0$.

Choose $x\in L(2P_\infty)\setminus L(P_\infty)$ and $y\in L(3P_\infty)\setminus L(2P_\infty)$. Their unique poles have orders two and three respectively. Distinct pole orders prove linear independence in the following complete list:

$$
\boxed{\begin{aligned}
L(0)&=L(P_\infty)=\langle1\rangle,\\
L(2P_\infty)&=\langle1,x\rangle,\\
L(3P_\infty)&=\langle1,x,y\rangle,\\
L(4P_\infty)&=\langle1,x,y,x^2\rangle,\\
L(5P_\infty)&=\langle1,x,y,x^2,xy\rangle,\\
L(6P_\infty)&=\langle1,x,y,x^2,xy,x^3\rangle.
\end{aligned}}
$$

Since $y^2$ also lies in the last six-dimensional space, it satisfies

$$
y^2=ax^3+bxy+cx^2+dy+ex+f,\qquad a\ne0.
$$

The coefficient $a$ cannot vanish because only $x^3$ among the displayed basis has a sixth-order pole available to cancel the leading pole of $y^2$. Homogenizing gives a plane cubic relation, valid also in characteristics two and three without completing squares or dividing by three.

It remains to prove that the map actually embeds the curve. For $D=3P_\infty$, Riemann-Roch gives $\ell(D)=3$, $\ell(D-Q)=2$ for every point $Q$, and $\ell(D-Q-R)=1$, including $R=Q$. The first equality makes the [linear system](../../../../../system-of-linear-equations.md) base-point-free; the second separates distinct points, and the double-point case separates tangent directions. Therefore $D$ is very ample and $\phi_D$ is a [closed immersion](../../../../../closed-immersion.md) into $\mathbb P^2$. Its pullback of a line has degree three, so its image has degree three. The displayed cubic equation consequently defines the image, which is smooth because it is isomorphic to $X$. **Thus $\boxed{\phi_{3P_\infty}:X\cong\text{a smooth plane cubic}}$**. The affine expression $(1:x:y)$ extends across $P_\infty$ to $(0:0:1)$ by the pole orders.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
