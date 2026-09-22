<h1 id="40a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\omega=kc_P$, and let $\psi$ be the transmission angle. Since $\hat c_P=2c_P$, tangential phase matching gives

$$
k\sin\phi=\hat k\sin\psi,
\qquad
\hat k=\frac k2,
\qquad
\boxed{\sin\psi=2\sin\phi.}
$$

The assumption of no evanescence requires $\sin\phi\leq1/2$.

With a common suppressed factor $e^{-i\omega t}$, take

$$
\begin{aligned}
\mathbf u_I&=(\sin\phi,0,\cos\phi)
e^{ik(x\sin\phi+z\cos\phi)},\\
\mathbf u_R&=R(\sin\phi,0,-\cos\phi)
e^{ik(x\sin\phi-z\cos\phi)},\\
\mathbf u_T&=T(\sin\psi,0,\cos\psi)
e^{i\hat k(x\sin\psi+z\cos\psi)}.
\end{aligned}
$$

For an inviscid liquid, continuity of normal displacement and normal stress gives

$$
\cos\phi(1-R)=T\cos\psi,
\qquad
Z(1+R)=\hat ZT,
$$

where $Z=\lambda/c_P$ and $\hat Z=\hat\lambda/\hat c_P$. Solving,

$$
\boxed{
R=\frac{\hat Z\cos\phi-Z\cos\psi}
{\hat Z\cos\phi+Z\cos\psi},
\qquad
T=\frac{2Z\cos\phi}
{\hat Z\cos\phi+Z\cos\psi}.}
$$

The condition $|R|=|T|$ gives

$$
|\hat Z\cos\phi-Z\cos\psi|=2Z\cos\phi.
$$

The sign that could instead produce $Z\cos\psi=(\hat Z+2Z)\cos\phi$ leads to $\sin^2\phi>1$ and is inadmissible. Hence

$$
Z\cos\psi=(\hat Z-2Z)\cos\phi.
$$

Using $\cos^2\psi=1-4\sin^2\phi$ and squaring gives

$$
\boxed{
\sin^2\phi
=\frac{3Z^2-4Z\hat Z+\hat Z^2}
{\hat Z(\hat Z-4Z)}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40A](../../40a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
