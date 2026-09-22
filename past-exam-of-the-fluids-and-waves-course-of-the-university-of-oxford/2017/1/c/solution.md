<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $f(z)=\cosh(\pi z/a)$. The [hyperbolic cosine](../../../../hyperbolic-cosine.md) addition formula gives

$$
f(x+iy)=\cosh\frac{\pi x}a\cos\frac{\pi y}a+i\sinh\frac{\pi x}a\sin\frac{\pi y}a.
$$

For $x>0$ and $0<y<a$, both factors in the imaginary part are positive. Thus the image lies in the [upper half-plane](../../../../upper-half-plane-complex-analysis.md). The three walls map onto the entire [real axis](../../../../real-axis.md):

$$
\begin{aligned}
y=0&:\quad f\in[1,\infty),\\
x=0&:\quad f\in[-1,1],\\
y=a&:\quad f\in(-\infty,-1].
\end{aligned}
$$

Also $f'(z)=(\pi/a)\sinh(\pi z/a)\ne0$ in the interior.

To verify that this is a one-to-one [conformal map](../../../../conformal-map.md) onto the whole [upper half-plane](../../../../upper-half-plane-complex-analysis.md), factor it through $s=e^{\pi z/a}$. This first map is one-to-one onto $|s|>1$, $\operatorname{Im}s>0$, and $f(z)=(s+s^{-1})/2$. Given any $\operatorname{Im}\zeta>0$, the roots of $s^2-2\zeta s+1=0$ have product one. Neither lies on $|s|=1$, since that would make $\zeta$ real. Exactly one root therefore has $|s|>1$, and

$$
\operatorname{Im}\zeta=\tfrac12(1-|s|^{-2})\operatorname{Im}s
$$

forces that root into the upper half of the exterior disk. It has a unique preimage $z=(a/\pi)(\log|s|+i\arg s)$ with $0<\arg s<\pi$. This proves both surjectivity and injectivity. The construction is the [hyperbolic-cosine map of a half-strip](../../../../hyperbolic-cosine-map-of-a-half-strip.md).

The source location $c$ is complex, with $\operatorname{Re}c>0$ and $0<\operatorname{Im}c<a$. Put $C=f(c)$, so $\operatorname{Im}C>0$. The [method of images](../../../../method-of-images.md) places an equal [line source](../../../../line-source.md) at $\bar C$ below the [real axis](../../../../real-axis.md):

$$
W(\zeta)=\frac Q{2\pi}\left[\log(\zeta-C)+\log(\zeta-\bar C)\right].
$$

For real $\zeta$, the product of the two logarithm arguments is $|\zeta-C|^2>0$. Hence the [streamfunction](../../../../stream-function.md) is constant along the wall, on locally consistent branches of the [complex logarithm](../../../../complex-logarithm.md), and there is no normal [velocity](../../../../velocity.md). Pulling back gives the requested [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md):

$$
\boxed{w(z)=\frac Q{2\pi}\left[\log\!\left(\cosh\frac{\pi z}a-\cosh\frac{\pi c}a\right)+\log\!\left(\cosh\frac{\pi z}a-\cosh\frac{\pi\bar c}a\right)\right].}
$$

This is the [line source in a closed-end semi-infinite strip](../../../../line-source-in-a-closed-end-semi-infinite-strip.md), with no extra imposed flow. Since $f'(c)\ne0$, near the physical source $f(z)-f(c)=f'(c)(z-c)+O((z-c)^2)$. Thus $w=(Q/(2\pi))\log(z-c)+$ a regular term, verifying that the source strength remains $Q$ under the [conformal map](../../../../conformal-map.md). The image source has no preimage inside the physical strip. Finally, as $x\to\infty$, $w(z)\sim Qz/a+$ a constant, so the far-field [velocity](../../../../velocity.md) is $(Q/a,0)$ and the channel carries exactly the injected [volume flux](../../../../volumetric-flow-rate.md) $Q$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
