<h1 id="18g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a depressed quartic

$$
f(x)=x^4+px^2+qx+r_0
$$

with roots summing to zero, set

$$
\beta_1=\alpha_1\alpha_2+\alpha_3\alpha_4,
\quad
\beta_2=\alpha_1\alpha_3+\alpha_2\alpha_4,
\quad
\beta_3=\alpha_1\alpha_4+\alpha_2\alpha_3.
$$

The [cubic resolvent of a quartic](../../../../../../cubic-resolvent-of-a-quartic.md) is

$$
g(y)=\prod_{i=1}^3(y-\beta_i)
=y^3-py^2-4r_0y+(4pr_0-q^2).
$$

The symmetric group $S_4$ acts on the three partitions of four roots into two unordered pairs. The resulting homomorphism $S_4\to S_3$ has kernel the [Klein four-group](../../../../../../klein-four-group.md) $V_4$. If $\Delta(f)$ is a square and the characteristic is not two, the [discriminant criterion for an alternating Galois group](../../../../../../discriminant-criterion-for-an-alternating-galois-group.md) gives $G=\operatorname{Gal}(f)\leq A_4$, and its image on the three resolvent roots lies in $A_4/V_4\cong C_3$.

For an irreducible quartic, $G$ is transitive on four roots, and its only possibilities inside $A_4$ are $V_4$ and $A_4$. The resolvent is irreducible exactly when the image acts transitively on its three roots, equivalently when that image is $C_3$. Thus

$$
g\text{ irreducible}\iff G=A_4,
\qquad
g\text{ reducible}\iff G=V_4.
$$

The printed statement omits the needed irreducibility hypothesis on $f$. Literally it is false: $f=x(x^3-3x-1)$ has square discriminant and Galois group $C_3$, and its resolvent is irreducible. Without quartic irreducibility, a reducible resolvent only implies $G\leq V_4$, allowing the trivial group, $C_2$, or $V_4$.

For the specified polynomial $x^4+8x+12$,

$$
\Delta=256\cdot12^3-27\cdot8^4=331776=576^2.
$$

Its resolvent is $g(y)=y^3-48y-64$. Modulo $5$ this is $y^3+2y+1$, which has no root in $\mathbb F_5$ and is therefore an [irreducible](../../../../../../irreducible-polynomial.md) cubic. The quartic is given to be irreducible, so the preceding criterion yields

$$
\boxed{\operatorname{Gal}(x^4+8x+12)=A_4}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18G](../../18g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
