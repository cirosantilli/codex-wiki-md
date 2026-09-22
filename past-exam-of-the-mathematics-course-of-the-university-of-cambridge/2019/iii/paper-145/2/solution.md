<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a separated filtered group define

$$
G_\lambda=\{g:\omega(g)\geq\lambda\},
\qquad
G_{\lambda+}=\{g:\omega(g)>\lambda\}.
$$

The [associated graded Lie algebra of a filtered group](../../../../../associated-graded-lie-algebra-of-a-filtered-group.md) is

$$
\operatorname{gr}G=\bigoplus_\lambda G_\lambda/G_{\lambda+}.
$$

Each quotient is abelian because $[G_\lambda,G_\lambda]\subseteq G_{2\lambda}\subseteq G_{\lambda+}$. If $x\in G_\lambda$ and $y\in G_\mu$, set

$$
[\operatorname{gr}_\lambda x,\operatorname{gr}_\mu y]
=\operatorname{gr}_{\lambda+\mu}[x,y].
$$

The standard commutator identities $[xy,z]=[x,z]^y[y,z]$ and $[x,yz]=[x,z][x,y]^z$ prove well-defined bilinearity, while the Hall-Witt identity gives the [Jacobi identity](../../../../../jacobi-identity.md). If $\omega([x,y])=\omega(x)+\omega(y)$, this bracket has nonzero initial form, so the graded Lie algebra is nonabelian.

For a [p-valuation](../../../../../p-valuation.md), define

$$
t\operatorname{gr}_\lambda(g)=\operatorname{gr}_{\lambda+1}(g^p).
$$

The p-power axiom and the [Hall-Petrescu formula](../../../../../hall-petrescu-formula.md) make this well defined and turn each homogeneous component into part of a graded $\mathbb F_p[t]$-module. The leading-term congruence $[x^p,y]\equiv[x,y]^p$ modulo terms of valuation greater than $\omega(x)+\omega(y)+1$ makes the bracket $\mathbb F_p[t]$-bilinear.

For the given upper-triangular group, write an element of degree $n$ to leading order as

$$
1+p^n\begin{pmatrix}\alpha&\beta\\0&0\end{pmatrix},
\qquad \alpha,\beta\in\mathbb F_p.
$$

Let $X_n,Y_n$ denote the classes with $(\alpha,\beta)=(1,0),(0,1)$. Matrix commutators give

$$
[\alpha X_n+\beta Y_n,\gamma X_m+\delta Y_m]
=(\alpha\delta-\gamma\beta)Y_{n+m},
$$

and pth powers give $tX_n=X_{n+1}$ and $tY_n=Y_{n+1}$. Thus

$$
\boxed{\operatorname{gr}G=\mathbb F_p[t]X_1\oplus\mathbb F_p[t]Y_1,
\qquad [X_1,Y_1]=tY_1.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 145](../../paper-145-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
