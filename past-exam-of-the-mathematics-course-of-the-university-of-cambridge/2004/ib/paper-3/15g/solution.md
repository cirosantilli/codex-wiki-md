<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

Work on the unit sphere, so side lengths are central angles. Place the right-angle vertex at the north pole and choose perpendicular meridians through it. The other vertices can then be written

$$
B=(\sin a,0,\cos a),\qquad C=(0,\sin b,\cos b).
$$

Their dot product is the cosine of the central angle between them, namely the hypotenuse length $c$. Hence the spherical Pythagorean relation is

$$
\boxed{\cos c=B\cdot C=\cos a\cos b.}
$$

For the small triangle let its hypotenuse be $c_\lambda$. The same formula gives $\cos c_\lambda=\cos(\lambda a)\cos(\lambda b)$, so $c_\lambda\to0$. Expanding each cosine about zero yields

$$
1-\frac12c_\lambda^2+O(c_\lambda^4)
=1-\frac12\lambda^2(a^2+b^2)+O(\lambda^4).
$$

In particular $c_\lambda=O(\lambda)$, and thus $c_\lambda^2=\lambda^2(a^2+b^2)+O(\lambda^4)$. Consequently **$(c_\lambda/\lambda)^2\to a^2+b^2$**, the ordinary Pythagorean theorem in the locally flat limit.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
