<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Define the [exterior square](../../../../../exterior-square.md) over the arbitrary field $k$ by $\bigwedge^2V=(V\otimes V)/\operatorname{span}\{v\otimes v:v\in V\}$. Write the image of $u\otimes v$ as $u\wedge v$. Then $v\wedge v=0$ and $u\wedge v=-v\wedge u$; the basis is $v_i\wedge v_j$ with $i<j$, in [characteristic two](../../../../../characteristic-two.md) as well. The [exterior-power Lie algebra representation](../../../../../exterior-power-lie-algebra-representation.md) is

$$
\boxed{x\cdot(u\wedge v)=(xu)\wedge v+u\wedge(xv).}
$$

The [tensor product of Lie algebra representations](../../../../../tensor-product-of-lie-algebra-representations.md) descends to this quotient: $x\cdot(v\otimes v)=xv\otimes v+v\otimes xv$ is a linear combination of square tensors, namely $(v+xv)\otimes(v+xv)-v\otimes v-xv\otimes xv$. On the wedge basis its coefficients follow directly from the original representing matrices. Expanding both actions shows $[\rho_{\wedge^2}(x),\rho_{\wedge^2}(y)]=\rho_{\wedge^2}([x,y])$.

The inclusions of $V$ and $W$ into their [direct sum](../../../../../direct-sum.md) define the map

$$
\bigwedge^2V\oplus\bigwedge^2W\oplus(V\otimes W)\longrightarrow\bigwedge^2(V\oplus W),\qquad(a,b,v\otimes w)\longmapsto a+b+(v,0)\wedge(0,w).
$$

A combined [basis](../../../../../basis.md) shows that this sends a basis to the pure-$V$, pure-$W$ and mixed wedge basis vectors, with no overlap and no omission. The defining action on each wedge proves equivariance. Hence the [exterior square of a direct sum](../../../../../exterior-square-of-a-direct-sum.md) gives

$$
\boxed{\bigwedge^2(V\oplus W)\cong\bigwedge^2V\oplus\bigwedge^2W\oplus(V\otimes W).}
$$

No division by $2$ is involved, so the proof remains valid in [characteristic two](../../../../../characteristic-two.md).

For the complex [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_3$, write $\Gamma_{a,b}$ for the irreducible [highest-weight representation](../../../../../highest-weight-representation.md) with [Dynkin labels](../../../../../dynkin-label.md) $(a,b)$, and $V=\Gamma_{1,0}$. First the [sl3 decomposition of the symmetric-square dual tensor product](../../../../../sl3-decomposition-of-the-symmetric-square-dual-tensor-product.md) is

$$
A:=(S^2V)\otimes V^*\cong\Gamma_{2,1}\oplus\Gamma_{1,0}.
$$

Indeed contraction $c((uv)\otimes f)=f(u)v+f(v)u$ is a surjective [Lie algebra representation homomorphism](../../../../../lie-algebra-representation-homomorphism.md) onto $V$. Its 15-dimensional [kernel](../../../../../kernel-of-a-linear-map.md) contains the [highest-weight vector](../../../../../highest-weight-vector.md) $e_1^2\otimes e_3^*$ of weight $(2,1)$. The [Weyl dimension formula](../../../../../weyl-dimension-formula.md) gives $\dim\Gamma_{2,1}=15$, and the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) identifies the kernel and splits the map. With $B=\Gamma_{2,1}$, the direct-sum identity reduces the requested calculation to $\bigwedge^2B$, $B\otimes V$ and $\bigwedge^2V$.

For completeness, these decompositions can be checked entirely by [formal characters](../../../../../formal-character-of-a-weight-module.md). Let $x_1x_2x_3=1$, $h_1=x_1+x_2+x_3$, $h_1^*=x_1^{-1}+x_2^{-1}+x_3^{-1}$ and $h_2=\sum_i x_i^2+\sum_{i<j}x_ix_j$. Then $\chi_B=h_2h_1^*-h_1$. The [Weyl character formula](../../../../../weyl-character-formula.md) takes the determinant form

$$
\chi_{a,b}(x)=\frac{\det\!\begin{pmatrix}x_1^{a+b+2}&x_1^{b+1}&1\\x_2^{a+b+2}&x_2^{b+1}&1\\x_3^{a+b+2}&x_3^{b+1}&1\end{pmatrix}}{\det\!\begin{pmatrix}x_1^2&x_1&1\\x_2^2&x_2&1\\x_3^2&x_3&1\end{pmatrix}}.
$$

Substitute $\chi_B$ into $\chi_{\wedge^2B}(x)=\tfrac12(\chi_B(x)^2-\chi_B(x_1^2,x_2^2,x_3^2))$ and collect the determinant characters. This gives the [exterior square of the sl3 representation of highest weight (2,1)](../../../../../exterior-square-of-the-sl3-representation-of-highest-weight-2-1.md) and the [sl3 highest-weight tensor rule](../../../../../sl3-highest-weight-tensor-rule.md):

$$
\begin{aligned}
\bigwedge^2B&\cong\Gamma_{5,0}\oplus\Gamma_{2,3}\oplus\Gamma_{3,1}\oplus\Gamma_{1,2}\oplus\Gamma_{0,1},\\
B\otimes V&\cong\Gamma_{3,1}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0},\qquad\bigwedge^2V\cong\Gamma_{0,1}.
\end{aligned}
$$

The first line has dimensions $21+42+24+15+3=105=\binom{15}{2}$; the tensor product has dimension $24+15+6=45$. Equivalently, enumerate weights with the [sl3 interlacing character formula](../../../../../sl3-interlacing-character-formula.md) and subtract characters from the highest weight downwards. Finally

$$
\boxed{\bigwedge^2\!\bigl((S^2V)\otimes V^*\bigr)\cong\Gamma_{5,0}\oplus\Gamma_{2,3}\oplus2\Gamma_{3,1}\oplus2\Gamma_{1,2}\oplus\Gamma_{2,0}\oplus2\Gamma_{0,1}.}
$$

Its dimension is $21+42+48+30+6+6=153=\binom{18}{2}$. The exterior square here is taken of the entire 18-dimensional tensor product; taking it only of $S^2V$ would be a different representation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
