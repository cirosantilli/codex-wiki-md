<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Write $Q(x,y)=ax^2+bxy+cy^2$ and associate the symmetric matrix $M=\begin{pmatrix}a&b/2\\b/2&c\end{pmatrix}$. Define the left [group action](../../../../../group-action.md) of $SL_2(\mathbb Z)$ by $(g\cdot Q)(v)=Q(g^{-1}v)$; using $Q(gv)$ instead describes the same equivalence classes. The transformed matrix is $g^{-T}Mg^{-1}$, so its [determinant](../../../../../determinant.md) is unchanged. Hence the [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md)

$$
D=b^2-4ac=-4\det M
$$

is invariant under [proper equivalence of binary quadratic forms](../../../../../proper-equivalence-of-binary-quadratic-forms.md).

A proper representation here means $Q(x,y)=n$ with $\gcd(x,y)=1$. Such a vector extends to the first column of an integer determinant-one matrix by [Bezout identity](../../../../../bezout-identity.md). After that change of variables the form has leading coefficient $n$, and [discriminant](../../../../../discriminant.md) $-35$, so its middle coefficient $b'$ satisfies $(b')^2\equiv-35\pmod{4n}$. Conversely, such a congruence gives the positive definite integral form

$$
[n,b',((b')^2+35)/(4n)],
$$

which represents $n$ at $(1,0)$. It is primitive: a common divisor of all three coefficients would have its square dividing the squarefree [discriminant](../../../../../discriminant.md) 35.

For clarity, enumerate all the proper equivalence classes at this [discriminant](../../../../../discriminant.md). Substitutions $(x,y)\mapsto(x+my,y)$ first arrange $|b|\le a$; if $c<a$, the determinant-one substitution $(x,y)\mapsto(-y,x)$ makes the leading coefficient smaller. Repeating terminates because this coefficient is a positive integer. Thus every class has a reduced representative with $|b|\le a\le c$. From $4ac-b^2=35$ it follows that $3a^2\le35$, giving $a\le3$. Checking $a=1,2,3$, with $b$ odd, yields

$$
[1,\pm1,9]\quad\hbox{or}\quad[3,\pm1,3].
$$

The two signs in the first pair are equivalent by replacing $x$ with $x-y$, and in the second pair by the determinant-one swap. Thus the two forms in the question exhaust the classes.

The [primitive representation criterion at discriminant minus thirty-five](../../../../../primitive-representation-criterion-at-discriminant-minus-thirty-five.md) now follows. For odd $n$ prime to 35, the congruence modulo $4n$ is solvable exactly when $-35$ is a square modulo every prime divisor of $n$. Necessity is immediate. For sufficiency, a nonzero root modulo each odd prime $q\mid n$ lifts to all required prime powers because its derivative $2b'$ is invertible; combine the lifts by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), also imposing $b'\equiv1\pmod2$. This gives the modulus-four condition since $-35\equiv1\pmod4$. We conclude

$$
\boxed{n\text{ is properly represented by one of the two forms}
\iff \left(\frac{-35}{q}\right)=1\quad\text{for every prime }q\mid n.}
$$

By [quadratic reciprocity](../../../../../quadratic-reciprocity.md), the symbol equals $(q/5)(q/7)$. In particular each prime divisor must be a quadratic residue at both 5 and 7, or a nonresidue at both. The condition is on each prime divisor, not merely on the product [Jacobi symbol](../../../../../jacobi-symbol.md) of $n$.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
