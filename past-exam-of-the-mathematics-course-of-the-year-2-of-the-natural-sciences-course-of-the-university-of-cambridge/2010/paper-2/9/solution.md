<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Two elements are [conjugate group elements](../../../../conjugate-group-elements.md) if $h=xgx^{-1}$ for some $x\in G$. The [conjugacy class](../../../../conjugacy-class.md) of $g$ is $\{xgx^{-1}:x\in G\}$. Conjugacy is an [equivalence relation](../../../../equivalence-relation.md): it is reflexive using $x=e$, symmetric by replacing $x$ with $x^{-1}$, and transitive because

$$
k=yhy^{-1},\quad h=xgx^{-1}\quad\Longrightarrow\quad k=(yx)g(yx)^{-1}.
$$

Thus the classes partition the group: every element belongs to its own class, and any two classes that intersect are equal. This proves that every element belongs to exactly one class.

If $G$ is [Abelian](../../../../abelian-group.md), then $xgx^{-1}=g$, so every class is a singleton. In general the elements whose classes are singletons are precisely those commuting with every group element. Thus the [center of a group](../../../../center-of-a-group.md) is

$$
Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}.
$$

It contains $e$. If $a,b\in Z(G)$, then $ab^{-1}$ commutes with every $g$, since $b^{-1}$ does and $a$ does. The [subgroup test](../../../../subgroup-test.md) therefore proves that $Z(G)$ is a subgroup. Any two of its elements commute with each other, so it is an [abelian subgroup](../../../../abelian-subgroup.md).

For the square centred at the origin with vertices $(\pm1,\pm1)$, put

$$
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad S=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

The [dihedral group](../../../../dihedral-group.md) $D_4$ consists of $R^j$ and $R^jS$, $j=0,1,2,3$. Its eight actions and their matrices are

$$
\begin{array}{c|c|c}
\text{element}&\text{geometrical action}&\text{matrix}\\\hline
I&\text{identity}&\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
R&90^\circ\text{ counterclockwise rotation}&\begin{pmatrix}0&-1\\1&0\end{pmatrix}\\
R^2&180^\circ\text{ rotation}&\begin{pmatrix}-1&0\\0&-1\end{pmatrix}\\
R^3&270^\circ\text{ counterclockwise rotation}&\begin{pmatrix}0&1\\-1&0\end{pmatrix}\\
S&\text{reflection in }y=0&\begin{pmatrix}1&0\\0&-1\end{pmatrix}\\
RS&\text{reflection in }y=x&\begin{pmatrix}0&1\\1&0\end{pmatrix}\\
R^2S&\text{reflection in }x=0&\begin{pmatrix}-1&0\\0&1\end{pmatrix}\\
R^3S&\text{reflection in }y=-x&\begin{pmatrix}0&-1\\-1&0\end{pmatrix}
\end{array}.
$$

These exhaust the symmetries: the image of one vertex has four choices and the image of an adjacent vertex has two choices, determining the entire square. For an explicit pair of nonconjugate elements take $R^2$ and $S$. Both have order two, but their [determinants](../../../../determinant.md) are $+1$ and $-1$. A [similarity transformation](../../../../similarity-transformation.md) preserves the determinant, so **$R^2$ and $S$ are not conjugate**.

To find the centre, use $SR=R^{-1}S$. A rotation $R^j$ commutes with $S$ exactly when $R^j=R^{-j}$, so $j$ is even. No reflection $R^jS$ commutes with $R$, since $(R^jS)R=R^{j-1}S$ while $R(R^jS)=R^{j+1}S$, and $R^2\ne I$. Therefore

$$
\boxed{Z(D_4)=\{I,R^2\}.}
$$

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
