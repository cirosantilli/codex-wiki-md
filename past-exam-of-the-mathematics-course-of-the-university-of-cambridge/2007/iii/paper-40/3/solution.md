<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

If the center $z$ violates a constraint, choose a row $a^T$ with $a^Tz<b_i$. Under the assumption of nonempty $P$, this row cannot have $a=0$. Every $x\in P$ satisfies $a^Tx\geq b_i>a^Tz$. Thus the central [half-space](../../../../../half-space.md)

$$
H=\{x:a^T(x-z)\geq0\}
$$

contains $P$, and the given outer bound yields $P\subseteq E(z,D)\cap H$. Checking the rows of $A$ therefore supplies a [separation oracle](../../../../../separation-oracle.md). If a violated row has zero normal, it instead certifies that $P$ is empty.

Whiten the [ellipsoid](../../../../../ellipsoid.md) by $x=z+D^{1/2}y$ and rotate the cut normal to $e_1$. The normalized current [ellipsoid](../../../../../ellipsoid.md) is the unit ball centered at zero. In the stated covering [ellipsoid](../../../../../ellipsoid.md), for $n\geq2$, the shape matrix has eigenvalue $n^2/(n+1)^2$ in the $e_1$ direction and $n^2/(n^2-1)$ in each of the other $n-1$ directions. The center does not affect volume, so

$$
R:=\frac{\operatorname{vol}(E')}{\operatorname{vol}(E)}
=\frac n{n+1}\left(\frac{n^2}{n^2-1}\right)^{(n-1)/2}.
$$

Using $\log(1-a)<-a$ for $0<a<1$ and $\log(1+b)<b$ for $b>0$ gives

$$
\begin{aligned}
\log R
&=\log\left(1-\frac1{n+1}\right)+\frac{n-1}{2}\log\left(1+\frac1{n^2-1}\right)\\
&<-\frac1{n+1}+\frac{n-1}{2(n^2-1)}
=-\frac1{2(n+1)}.
\end{aligned}
$$

Therefore

$$
\boxed{\operatorname{vol}(E')<e^{-1/(2(n+1))}\operatorname{vol}(E).}
$$

This is the [central-cut ellipsoid volume bound](../../../../../central-cut-ellipsoid-volume-bound.md). Affine transformations preserve the ratio. The displayed matrix formula is undefined when $n=1$; in that case interval bisection gives the stronger ratio $1/2$.

Undoing the normalization gives the general central-cut update

$$
\begin{aligned}
z'&=z+\frac{Da}{(n+1)\sqrt{a^TDa}},\\
D'&=\frac{n^2}{n^2-1}\left(D-\frac{2}{n+1}\frac{Daa^TD}{a^TDa}\right).
\end{aligned}
$$

It preserves containment of the feasible region while reducing volume geometrically. After $k$ cuts the volume is less than $V_0e^{-k/(2(n+1))}$. If a feasible region has a known positive-volume lower bound $V_{\min}$, more than $2(n+1)\log(V_0/V_{\min})$ unsuccessful cuts would be impossible. For rational inputs, outer-radius and positive-volume bounds of exponential size in a polynomial of the bit length therefore translate into a polynomial iteration count.

For a full [ellipsoid method](../../../../../ellipsoid-method.md) proof, two qualifications matter. A nonempty rational polyhedron may be lower-dimensional and have zero volume, so shrinking below a volume threshold alone cannot certify its emptiness. One uses a bounded-feasibility reduction and a sufficiently small rational relaxation or an affine-hull treatment, with input-dependent rational separation bounds. Also [ellipsoid](../../../../../ellipsoid.md) updates involve square roots, so a bit-complexity proof rounds with controlled outward error to preserve containment and a fixed volume decrease. With these precision bounds, and the polynomial-time row separation oracle here, the method establishes polynomial-time [linear programming](../../../../../linear-programming.md). The volume calculation is its essential geometric step, not by itself the entire complexity proof.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
