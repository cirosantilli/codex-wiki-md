<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For each complex coordinate, exchanging the factors of a [wedge product of differential forms](../../../../wedge-product-of-differential-forms.md) reverses its sign, giving

$$
 dz_k\wedge d\bar z_k
=(dx_k+i\,dx_{k+3})\wedge(dx_k-i\,dx_{k+3})
=-2i\,dx_k\wedge dx_{k+3}.
$$

Consequently the [Kähler form](../../../../kahler-form.md) is $\omega=dx_{14}+dx_{25}+dx_{36}$, and $\omega\wedge dx_7=dx_{147}+dx_{257}+dx_{367}$. Expanding the [holomorphic volume form](../../../../holomorphic-volume-form.md) gives

$$
\begin{aligned}
\operatorname{Re}\bigl((dx_1+i\,dx_4)\wedge(dx_2+i\,dx_5)\wedge(dx_3+i\,dx_6)\bigr)
&=dx_{123}-dx_{156}-dx_{426}-dx_{453}\\
&=dx_{123}-dx_{156}+dx_{246}-dx_{345}.
\end{aligned}
$$

The sign of $dx_{426}$ changes on exchanging $4,2$, while reordering $4,5,3$ to $3,4,5$ requires two exchanges. This verifies every sign in

$$
\boxed{\phi=\omega\wedge dy+\operatorname{Re}\Omega,\qquad y=x_7.}
$$

Under $z\mapsto Uz$, [unitarity](../../../../unitary-operator.md) preserves $\omega$:

$$
\omega' =\frac i2\sum_{a,b}\left(\sum_kU_{ka}\bar U_{kb}\right)dz_a\wedge d\bar z_b
=\omega.
$$

The [determinant](../../../../determinant.md) is the factor by which a transformation acts on a top [exterior power](../../../../exterior-power.md), so $\Omega'=(\det U)\Omega=\Omega$ for $U\in SU(3)$. Extend the real embedding by fixing $y$. It preserves $\omega$, $dy$ and $\Omega$, and therefore $\phi$. Thus

$$
\boxed{U\longmapsto\operatorname{diag}(\rho(U),1)
\quad\text{embeds }SU(3)\text{ into }G_2.}
$$

The induced seven-dimensional [representation](../../../../group-representation.md) is exactly the restriction already computed in [c](../c.md). In the conventional complex notation its [branching rule](../../../../branching-rule.md) is

$$
\boxed{\mathbf7_{G_2}\downarrow SU(3)=\mathbf3\oplus\bar{\mathbf3}\oplus\mathbf1.}
$$

Over the [real numbers](../../../../real-number.md), the six-dimensional summand is the underlying real space of the complex [fundamental representation](../../../../fundamental-representation.md), and the last real line is the fixed $y$ axis.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
