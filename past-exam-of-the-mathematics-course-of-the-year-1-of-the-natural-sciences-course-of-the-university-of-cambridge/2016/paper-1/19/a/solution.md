<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [multivariable chain rule](../../../../../multivariable-chain-rule.md) to an arbitrary differentiable scalar [function](../../../../../function-split.md) of $x,y,z$. With the subscripts indicating the coordinates held fixed, the first operator is

$$
\boxed{(\partial_W)_{\theta,\phi}
=\tan\theta\cos\phi\,(\partial_x)_{y,z}
+\tan\theta\sin\phi\,(\partial_y)_{x,z}
+(\partial_z)_{x,y}.}
$$

Holding $W,\phi$ fixed when differentiating with respect to $\theta$ gives

$$
\boxed{(\partial_\theta)_{W,\phi}
=W\sec^2\theta\cos\phi\,(\partial_x)_{y,z}
+W\sec^2\theta\sin\phi\,(\partial_y)_{x,z}.}
$$

Finally, holding $W,\theta$ fixed gives

$$
\boxed{(\partial_\phi)_{W,\theta}
=-W\tan\theta\sin\phi\,(\partial_x)_{y,z}
+W\tan\theta\cos\phi\,(\partial_y)_{x,z}.}
$$

For example, the coefficient of $\partial_x$ in $\partial_\theta$ is precisely $(\partial x/\partial\theta)_{W,\phi}$; all coefficients follow by differentiating the given coordinate [functions](../../../../../function-split.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
