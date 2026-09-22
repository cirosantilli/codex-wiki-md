# Paper 2

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper2.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper2.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [a](#2/ii/a)
      - [Solution](#2/ii/a/solution)
    - [b](#2/ii/b)
      - [Solution](#2/ii/b/solution)
    - [c](#2/ii/c)
      - [Solution](#2/ii/c/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
  - [v](#5/v)
    - [Solution](#5/v/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Realize the defining [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) as $\mathbb Cx\oplus\mathbb Cy$, with $H=x\partial_x-y\partial_y$, $E=x\partial_y$, $F=y\partial_x$. A [basis](../../../vector-space.md#basis) of the [symmetric power](../../../linear-algebra.md#symmetric-power) is $e_i=x^{4-i}y^i$ for $0\leq i\leq4$, with $He_i=(4-2i)e_i$. Hence the [exterior square](../../../linear-algebra.md#exterior-square) [basis](../../../vector-space.md#basis) $w_{ij}=e_i\wedge e_j$, $i<j$, has [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $8-2(i+j)$.

Collecting equal [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) gives the complete [weight-space decomposition](../../../semisimple-lie-algebra.md#weight-space-decomposition):

$$
\begin{array}{c|l|c}
\text{weight}&\text{basis}&\text{multiplicity}\\ \hline
6&w_{01}&1\\
4&w_{02}&1\\
2&w_{03},w_{12}&2\\
0&w_{04},w_{13}&2\\
-2&w_{14},w_{23}&2\\
-4&w_{24}&1\\
-6&w_{34}&1
\end{array}
$$

Every one of the ten exterior [basis vectors](../../../vector-space.md#basis-vector) appears exactly once. Thus **$U=\bigoplus_{m=6,4,2,0,-2,-4,-6}U_m$**, with the displayed [bases](../../../vector-space.md#basis) and [dimensions](../../../vector-space.md#dimension-vector-space).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) has [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $6,4,2,0,-2,-4,-6$ with multiplicities $1,1,2,2,2,1,1$. An [Irreducible Lie algebra representation](../../../lie-algebra.md#irreducible-lie-algebra-representation) of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) with [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $n$ has [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $n,n-2,\ldots,-n$, all of multiplicity one. The top [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) therefore forces one $L(6)$ summand. Subtracting its [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) leaves [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $2,0,-2$, each once, which is $L(2)$. By [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem),

$$
\boxed{\Lambda^2(\operatorname{Sym}^4V)\cong L(6)\oplus L(2)
\cong\operatorname{Sym}^6V\oplus\operatorname{Sym}^2V.}
$$

Their [dimensions](../../../vector-space.md#dimension-vector-space) $7+3=10$ account for the entire module.

<a id="1/a/ii/image-the-exterior-square-weight-diagram-and-its-two-irreducible-summands-basis-labels-are-defined-in-part-iii"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sl2-weights.png)

**[Figure 1](#1/a/ii/image-the-exterior-square-weight-diagram-and-its-two-irreducible-summands-basis-labels-are-defined-in-part-iii). The exterior-square weight diagram and its two irreducible summands; basis labels are defined in part iii**.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Use the [exterior-power Lie algebra representation](../../../lie-algebra.md#exterior-power-lie-algebra-representation):

$$
F(e_i\wedge e_j)=(4-i)e_{i+1}\wedge e_j+(4-j)e_i\wedge e_{j+1},\qquad
E(e_i\wedge e_j)=i e_{i-1}\wedge e_j+j e_i\wedge e_{j-1}.
$$

Reorder wedge factors when necessary and interpret repeated factors as zero. The [explicit weight basis of the exterior square of Sym4 for sl2](../../../semisimple-lie-algebra.md#explicit-weight-basis-of-the-exterior-square-of-sym4-for-sl2) is

$$
\begin{aligned}
v_0&=w_{01},&v_1&=w_{02},&v_2&=w_{03}+2w_{12},\\
v_3&=w_{04}+8w_{13},&v_4&=w_{14}+2w_{23},&
v_5&=w_{24},\quad v_6=w_{34},
\end{aligned}
$$

for $L(6)$, and

$$
t_0=w_{03}-3w_{12},\qquad t_1=w_{04}-2w_{13},\qquad
t_2=w_{14}-3w_{23},
$$

for $L(2)$. Their [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) are $6-2j$ and $2-2j$, respectively.

Direct application of the displayed operators gives $Ev_0=Et_0=0$ and the lowering chains

$$
v_0\xrightarrow{\,F\,}3v_1,\quad
v_1\mapsto2v_2,\quad v_2\mapsto v_3,\quad
v_3\mapsto12v_4,\quad v_4\mapsto5v_5,\quad
v_5\mapsto2v_6,\quad v_6\mapsto0,
$$



$$
Ft_0=t_1,\qquad Ft_1=2t_2,\qquad Ft_2=0.
$$

The raising coefficients along the first chain are $2,5,12,1,2,3$; along the second, $Et_1=2t_0$ and $Et_2=t_1$. Thus each span is stable and is the required irreducible module. At the common [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $2,0,-2$, the $v$ and $t$ vectors are independent; the other [weight spaces](../../../semisimple-lie-algebra.md#weight-space) occur only in the first span. This proves that the ten vectors are a [basis](../../../vector-space.md#basis) of $U$ and that the two spans are complementary. The [highest-weight vectors](../../../semisimple-lie-algebra.md#highest-weight-vector) are

$$
\boxed{v_0=e_0\wedge e_1\text{ of weight }6,\qquad
t_0=e_0\wedge e_3-3e_1\wedge e_2\text{ of weight }2.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let $e_1,e_2,e_3$ be the [basis](../../../vector-space.md#basis) of the [defining representation](../../../lie-algebra.md#defining-representation-of-a-matrix-lie-algebra) and $y_1,y_2,y_3$ its dual. On a diagonal element of the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) their [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) are $L_i$ and $-L_i$, with $L_1+L_2+L_3=0$. Use the [tensor product](../../../linear-algebra.md#tensor-product) and [symmetric square](../../../linear-algebra.md#symmetric-square) [basis](../../../vector-space.md#basis)

$$
T_{i;jk}=e_i\otimes y_jy_k,\qquad 1\leq i\leq3,\quad1\leq j\leq k\leq3.
$$

Its [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) is $L_i-L_j-L_k$. For the three repeated [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) put

$$
A_j=T_{j;jj},\qquad B_{i;j}=e_i\otimes y_i y_j\quad(i\ne j).
$$

If $\{i,l\}=\{1,2,3\}\setminus\{j\}$, the complete [weight-space decomposition](../../../semisimple-lie-algebra.md#weight-space-decomposition) is

$$
\begin{array}{c|c|c}
\text{weight}&\text{basis}&\text{multiplicity}\\ \hline
L_i-2L_j\ (i\ne j)&T_{i;jj}&1\\
2L_i&T_{i;jk},\quad\{i,j,k\}=\{1,2,3\},\ j<k&1\\
-L_j&A_j,\ B_{i;j},\ B_{l;j}&3
\end{array}
$$

There are six spaces of the first type, three of the second, and three of the third. Their [dimensions](../../../vector-space.md#dimension-vector-space) sum to $6+3+9=18$. The [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) below labels every space with all of its [basis vectors](../../../vector-space.md#basis-vector).

<a id="1/b/i/image-all-weight-spaces-of-the-sl3-tensor-module-with-each-tensor-basis-vector-shown-at-its-weight"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sl3-tensor-weights.png)

**[Figure 2](#1/b/i/image-all-weight-spaces-of-the-sl3-tensor-module-with-each-tensor-basis-vector-shown-at-its-weight). All weight spaces of the sl3 tensor module, with each tensor-basis vector shown at its weight**.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Use the [contraction splitting of a defining module tensor a dual symmetric square](../../../semisimple-lie-algebra.md#contraction-splitting-of-a-defining-module-tensor-a-dual-symmetric-square). For a quadratic [polynomial](../../../polynomial.md) $p$ in the dual variables, define

$$
C(e_i\otimes p)=\partial_{y_i}p,\qquad
\iota(y_j)=Q_j:=\sum_{i=1}^3e_i\otimes y_i y_j.
$$

Both maps are [intertwiners](../../../representation-theory.md#intertwiner). The first is the natural [tensor contraction](../../../linear-algebra.md#tensor-contraction); the second uses the [invariant tensor](../../../representation-theory.md#invariant-tensor) $\sum_i e_i\otimes y_i$. Directly, $C(Q_j)=4y_j$, so $C\iota=4I$ and

$$
W=\ker C\oplus\operatorname{im}\iota,\qquad
\operatorname{im}\iota\cong V^*,\qquad \dim\ker C=18-3=15.
$$

The vector $T_{1;33}=e_1\otimes y_3^2$ lies in $\ker C$ and is killed by both positive simple-root operators $E_{12},E_{23}$. It is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $L_1-2L_3=\omega_1+2\omega_2$. By [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem), it generates the corresponding irreducible summand. The [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) for $\mathfrak{sl}_3$ gives $\dim\Gamma_{a,b}=(a+1)(b+1)(a+b+2)/2$, hence $\dim\Gamma_{1,2}=15$, exhausting the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). Therefore

$$
\boxed{V\otimes\operatorname{Sym}^2V^*\cong\Gamma_{1,2}\oplus\Gamma_{0,1},
\qquad \Gamma_{0,1}=V^*.}
$$

The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) has the nine outer [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) of multiplicity one and each inner [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $-L_j$ of multiplicity two; the dual summand has just the three [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $-L_j$, each once.

<a id="1/b/ii/image-weight-diagrams-and-basis-labels-of-the-fifteen-dimensional-kernel-and-the-dual-summand"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sl3-submodule-weights.png)

**[Figure 3](#1/b/ii/image-weight-diagrams-and-basis-labels-of-the-fifteen-dimensional-kernel-and-the-dual-summand). Weight diagrams and basis labels of the fifteen-dimensional kernel and the dual summand**.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Use the [basis](../../../vector-space.md#basis) labels in the preceding diagrams. For each $j$, write $\{i,l\}=\{1,2,3\}\setminus\{j\}$ with $i<l$, and define

$$
K_{j,1}=A_j-2B_{i;j},\qquad K_{j,2}=A_j-2B_{l;j}.
$$

The contraction satisfies $C(A_j)=2y_j$ and $C(B_{i;j})=y_j$, so both $K$ vectors lie in $\ker C$. They are independent and form a [basis](../../../vector-space.md#basis) of its [weight space](../../../semisimple-lie-algebra.md#weight-space) at $-L_j$.

Thus the [bases](../../../vector-space.md#basis) marked on the [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) of $\Gamma_{1,2}$ are

$$
\begin{array}{c|c}
\text{weight}&\text{basis in }\ker C\\ \hline
L_i-2L_j\ (i\ne j)&T_{i;jj}\\
2L_i&T_{i;jk},\quad\{i,j,k\}=\{1,2,3\},\ j<k\\
-L_j&K_{j,1},K_{j,2}
\end{array}
$$

and the diagram of $\Gamma_{0,1}$ uses the [basis](../../../vector-space.md#basis) $Q_j=A_j+B_{i;j}+B_{l;j}$ at $-L_j$. Each $Q_j$ is complementary to the two [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) vectors because its contraction is $4y_j\ne0$. All vectors shown are therefore genuine [bases](../../../vector-space.md#basis), not merely [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) counts. The [highest-weight vectors](../../../semisimple-lie-algebra.md#highest-weight-vector) are

$$
\boxed{T_{1;33}\text{ for }\Gamma_{1,2},\qquad Q_3\text{ for }\Gamma_{0,1}.}
$$

The latter is highest because $\iota$ intertwines the [dual Lie algebra representation](../../../lie-algebra.md#dual-lie-algebra-representation) and $y_3$ is its [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector).

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For $H=\operatorname{diag}(r,s,-r,-s)$, put $L_1(H)=r$, $L_2(H)=s$. Then $L_3=-L_1$, $L_4=-L_2$. The [matrix unit](../../../vector-space.md#matrix-unit) identity

$$
[H,E_{ij}]=(L_i-L_j)(H)E_{ij}
$$

reads off the [root spaces](../../../semisimple-lie-algebra.md#root-space) directly. The complete list is

$$
\begin{array}{c|c}
\alpha&\mathfrak g_\alpha\\ \hline
L_1-L_2&\mathbb C(E_{12}-E_{43})\\
L_2-L_1&\mathbb C(E_{21}-E_{34})\\
L_1+L_2&\mathbb C(E_{14}+E_{23})\\
-L_1-L_2&\mathbb C(E_{32}+E_{41})\\
2L_1&\mathbb CE_{13}\\
-2L_1&\mathbb CE_{31}\\
2L_2&\mathbb CE_{24}\\
-2L_2&\mathbb CE_{42}
\end{array}
$$

Thus the [C2 root system](../../../semisimple-lie-algebra.md#c2-root-system) is

$$
\boxed{\Phi=\{\pm2L_1,\ \pm2L_2,\ \pm(L_1+L_2),\ \pm(L_1-L_2)\}.}
$$

All eight [root spaces](../../../semisimple-lie-algebra.md#root-space) have [dimension](../../../vector-space.md#dimension-vector-space) one. The zero-weight space is the two-dimensional [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) $\mathbb C(E_{11}-E_{33})\oplus\mathbb C(E_{22}-E_{44})$; zero itself is not a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/a">a</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/ii/a)

For the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) gives the eight nonzero [weights](../../../semisimple-lie-algebra.md#weight-representation-theory)

$$
\pm2L_1,\quad\pm2L_2,\quad\pm L_1\pm L_2,
$$

each of multiplicity one, and [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) zero of multiplicity two from the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). Thus its [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) is the [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) diagram with a double zero [weight](../../../semisimple-lie-algebra.md#weight-representation-theory), and its total [dimension](../../../vector-space.md#dimension-vector-space) is $8+2=10$.

<a id="2/ii/a/image-adjoint-sp4-weights-the-eight-roots-and-the-zero-weight-of-multiplicity-two"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sp4-adjoint-weights.png)

**[Figure 4](#2/ii/a/image-adjoint-sp4-weights-the-eight-roots-and-the-zero-weight-of-multiplicity-two). Adjoint sp4 weights: the eight roots and the zero weight of multiplicity two**.

<h4 id="2/ii/b">b</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/ii/b)

In the [defining representation](../../../lie-algebra.md#defining-representation-of-a-matrix-lie-algebra), the diagonal element of the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) acts on the four standard [basis vectors](../../../vector-space.md#basis-vector) with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $r,s,-r,-s$. Therefore

$$
\boxed{\operatorname{wt}(V)=\{L_1,L_2,-L_1,-L_2\},\qquad\text{each with multiplicity one}.}
$$

Their [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) is the four-point cross below.

<a id="2/ii/b/image-the-four-defining-representation-weights-of-sp4"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sp4-defining-weights.png)

**[Figure 5](#2/ii/b/image-the-four-defining-representation-weights-of-sp4). The four defining-representation weights of sp4**.

<h4 id="2/ii/c">c</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#2/ii/c)

The [tensor-product weight diagram](../../../semisimple-lie-algebra.md#tensor-product-weight-diagram) is obtained by adding every ordered pair of defining [weights](../../../semisimple-lie-algebra.md#weight-representation-theory). Each $\pm2L_i$ occurs once, while each of the four [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\pm L_1\pm L_2$ occurs twice, from the two orders of the summands. Zero occurs four times, from the ordered pairs $(L_i,-L_i)$ and $(-L_i,L_i)$ for $i=1,2$. Hence

$$
\begin{array}{c|c}
\text{weight}&\text{multiplicity}\\ \hline
\pm2L_1,\ \pm2L_2&1\\
\pm L_1\pm L_2&2\\
0&4
\end{array}
$$

The [dimensions](../../../vector-space.md#dimension-vector-space) sum to $4+8+4=16$, as required for $V\otimes V$.

<a id="2/ii/c/image-tensor-square-sp4-weights-including-the-double-diagonal-weights-and-four-dimensional-zero-space"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sp4-tensor-weights.png)

**[Figure 6](#2/ii/c/image-tensor-square-sp4-weights-including-the-double-diagonal-weights-and-four-dimensional-zero-space). Tensor-square sp4 weights, including the double diagonal weights and four-dimensional zero space**.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The printed phrase “not reducible” is a misprint: the requested nonzero complementary submodules establish that this tensor square is reducible. The natural reason is that the flip $\tau(v\otimes w)=w\otimes v$ commutes with the [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). Its two [eigenspaces](../../../linear-operator-theory.md#eigenspace) are the [symmetric square](../../../linear-algebra.md#symmetric-square) and the [exterior square](../../../linear-algebra.md#exterior-square), giving

$$
\boxed{V\otimes V=\operatorname{Sym}^2V\oplus\Lambda^2V,\qquad
\dim\operatorname{Sym}^2V=10,\quad\dim\Lambda^2V=6.}
$$

In the [symmetric square](../../../linear-algebra.md#symmetric-square), the four [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\pm2L_i$ and four [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\pm L_1\pm L_2$ each occur once, while zero occurs twice. In the [exterior square](../../../linear-algebra.md#exterior-square), the four [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\pm L_1\pm L_2$ each occur once and zero occurs twice; the $\pm2L_i$ are absent because repeated wedge factors vanish. These are the two requested complementary [weight diagrams](../../../semisimple-lie-algebra.md#weight-diagram).

<a id="2/iii/image-the-complementary-symmetric-and-alternating-tensor-submodules-of-the-defining-sp4-representation"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2-sp4-split-weights.png)

**[Figure 7](#2/iii/image-the-complementary-symmetric-and-alternating-tensor-submodules-of-the-defining-sp4-representation). The complementary symmetric and alternating tensor submodules of the defining sp4 representation**.

More precisely, the [tensor-square decomposition of the defining symplectic representation](../../../semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-symplectic-representation) identifies $\operatorname{Sym}^2V$ with the irreducible adjoint module $L(2\omega_1)$. The identification is an [intertwiner](../../../representation-theory.md#intertwiner) sending a [symmetric tensor](../../../linear-algebra.md#symmetric-tensor) $vw$ to the element of the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) $x\mapsto\omega(v,x)w+\omega(w,x)v$. For the [exterior square](../../../linear-algebra.md#exterior-square), [symplectic contraction of an exterior square](../../../linear-algebra.md#symplectic-contraction-of-an-exterior-square) has a five-dimensional [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), the [primitive exterior square](../../../linear-algebra.md#primitive-exterior-square), and the [invariant tensor](../../../representation-theory.md#invariant-tensor) $\Omega=e_1\wedge e_3+e_2\wedge e_4$ supplies a complementary line. Thus the full irreducible decomposition is

$$
\boxed{V\otimes V=L(2\omega_1)\oplus L(\omega_2)\oplus L(0),\qquad
16=10+5+1.}
$$

Here $\omega_1=L_1$ and $\omega_2=L_1+L_2$. The two zero [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) in the [exterior square](../../../linear-algebra.md#exterior-square) split into one primitive zero [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) and the invariant line.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The ambient [group ring of a weight lattice](../../../semisimple-lie-algebra.md#group-ring-of-a-weight-lattice) is

$$
\mathbb Z[\Lambda_W]=\left\{\sum_{\lambda\in\Lambda_W}a_\lambda e(\lambda):
a_\lambda\in\mathbb Z,\text{ with finite support}\right\},
\qquad e(\lambda)e(\mu)=e(\lambda+\mu).
$$

Addition is coefficientwise, and multiplication uses addition in the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice). For a finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $V=\bigoplus_\lambda V_\lambda$, its [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) is

$$
\boxed{\operatorname{char}V=\sum_\lambda(\dim V_\lambda)e(\lambda).}
$$

The [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) records the [dimensions](../../../vector-space.md#dimension-vector-space) of all [weight spaces](../../../semisimple-lie-algebra.md#weight-space). The ambient lattice ring should be distinguished from the [representation ring of a semisimple Lie algebra](../../../lie-algebra.md#representation-ring-of-a-semisimple-lie-algebra), which identifies with its Weyl-invariant subring.

For the $\mathfrak{sl}_3$ module $\Gamma_{1,2}$, $L_1+L_2+L_3=0$ and the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) is $L_1-2L_3=\omega_1+2\omega_2$. The decomposition $V\otimes\operatorname{Sym}^2V^*=\Gamma_{1,2}\oplus V^*$ gives

$$
\operatorname{char}\Gamma_{1,2}
=\left(\sum_i e(L_i)\right)\left(\sum_{j\leq k}e(-L_j-L_k)\right)-\sum_i e(-L_i).
$$

Collecting equal [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) yields

$$
\boxed{\operatorname{char}\Gamma_{1,2}
=\sum_{i\ne j}e(L_i-2L_j)+\sum_{i=1}^3e(2L_i)+2\sum_{i=1}^3e(-L_i).}
$$

The six first [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) and three second [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) have multiplicity one; each of the three [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $-L_i$ has multiplicity two. Their total is $6+3+6=15$, as required.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $v\in V_\lambda$ and $w\in W_\mu$, the [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations) acts by

$$
H(v\otimes w)=Hv\otimes w+v\otimes Hw=(\lambda(H)+\mu(H))v\otimes w.
$$

Thus its [weight space](../../../semisimple-lie-algebra.md#weight-space) of [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\nu$ is

$$
(V\otimes W)_\nu=\bigoplus_{\lambda+\mu=\nu}V_\lambda\otimes W_\mu,
\qquad
\dim(V\otimes W)_\nu=\sum_{\lambda+\mu=\nu}(\dim V_\lambda)(\dim W_\mu).
$$

Substituting this into the [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) and using $e(\lambda+\mu)=e(\lambda)e(\mu)$ proves

$$
\boxed{\operatorname{char}(V\otimes W)
=(\operatorname{char}V)(\operatorname{char}W).}
$$

Every sum is finite for the [Lie algebra representations](../../../lie-algebra.md#lie-algebra-representation) under consideration.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) acts on the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) by its [root reflections](../../../semisimple-lie-algebra.md#root-reflection) and extends to ring automorphisms of the [group ring of a weight lattice](../../../semisimple-lie-algebra.md#group-ring-of-a-weight-lattice):

$$
w\left(\sum_\lambda a_\lambda e(\lambda)\right)=\sum_\lambda a_\lambda e(w\lambda),\qquad
s_\alpha\lambda=\lambda-\lambda(H_\alpha)\alpha.
$$

[Weights](../../../semisimple-lie-algebra.md#weight-representation-theory) and their multiplicities in a finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) of a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) are permuted by this action, so its [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) is Weyl-invariant.

Choose a set $\Phi^+$ of [positive roots](../../../semisimple-lie-algebra.md#positive-root) and put

$$
\rho=\frac12\sum_{\alpha\in\Phi^+}\alpha=\sum_i\omega_i,\qquad
A_\nu=\sum_{w\in W}\det(w)e(w\nu).
$$

Here $\omega_i$ are the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight), and $\det(w)=(-1)^{\ell(w)}$, where the [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length) $\ell(w)$ counts [positive roots](../../../semisimple-lie-algebra.md#positive-root) carried to negative ones. For a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) $\lambda$, let $L(\lambda)$ denote the finite-dimensional [Irreducible Lie algebra representation](../../../lie-algebra.md#irreducible-lie-algebra-representation) of [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$. The [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) is

$$
\boxed{\operatorname{char}L(\lambda)=\frac{A_{\lambda+\rho}}{A_\rho}
=\frac{\sum_{w\in W}\det(w)e(w(\lambda+\rho))}
{e(\rho)\prod_{\alpha\in\Phi^+}(1-e(-\alpha))}.}
$$

The second denominator expression is the [Weyl denominator formula](../../../semisimple-lie-algebra.md#weyl-denominator-formula). Both alternants change sign under each [root reflection](../../../semisimple-lie-algebra.md#root-reflection); their quotient is invariant. Although written as a fraction, the theorem asserts that it is a finite element of $\mathbb Z[\Lambda_W]$ with the nonnegative coefficients given by [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) multiplicities. The [highest-weight classification](../../../semisimple-lie-algebra.md#highest-weight-classification-of-finite-dimensional-semisimple-lie-algebra-modules) specifies which $\lambda$ label the irreducibles, while the [root system](../../../semisimple-lie-algebra.md#root-system) and choice of [positive roots](../../../semisimple-lie-algebra.md#positive-root) determine every other term.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Write $u=\sum_\lambda a_\lambda e(\lambda)$ with finite support. The [root reflection](../../../semisimple-lie-algebra.md#root-reflection) is an involution, and $s_\alpha u=-u$ implies $a_{s_\alpha\lambda}=-a_\lambda$. Any fixed [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) has coefficient zero. For each nonfixed orbit choose its representative $\lambda$ with

$$
m=\lambda(H_\alpha)>0,\qquad
s_\alpha\lambda=\lambda-m\alpha.
$$

Integrality of $m$ follows because $\lambda$ belongs to the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice); positivity is ensured by our choice of orbit representative. Pairing the orbit coefficients gives

$$
u=\sum_{\text{chosen }\lambda}a_\lambda[e(\lambda)-e(\lambda-m\alpha)].
$$

For each pair, elementary finite telescoping shows

$$
e(\lambda)-e(\lambda-m\alpha)
=(1-e(\alpha))\left[-\sum_{r=1}^me(\lambda-r\alpha)\right].
$$

There are finitely many chosen orbits, and each inner sum is finite. This proves the [root-binomial divisibility of reflection anti-invariants](../../../semisimple-lie-algebra.md#root-binomial-divisibility-of-reflection-anti-invariants):

$$
\boxed{\frac{u}{1-e(\alpha)}
=-\sum_{\text{chosen }\lambda}a_\lambda\sum_{r=1}^{\lambda(H_\alpha)}
e(\lambda-r\alpha)\in\mathbb Z[\Lambda_W].}
$$

For precision, the geometric-series expression is interpreted coefficientwise. Its coefficient at a [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\nu$ is $\sum_{n\geq0}a_{\nu-n\alpha}$, which is a finite sum because $u$ has finite support. On each coset of $\mathbb Z\alpha$, reflection pairs the coefficients with opposite signs, so their total is zero. These cumulative sums vanish both before the smallest occupied [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) and after the largest occupied [weight](../../../semisimple-lie-algebra.md#weight-representation-theory). Only finitely many cosets are occupied, hence the product of the formal series with $u$ has finite support and equals the boxed quotient.

The individual terms $e(n\alpha)u$ need not vanish for large $n$. For example, $u=e(\alpha)-e(-\alpha)$ is anti-invariant, and its quotient is $-1-e(-\alpha)$. Thus **“finite sum” means a finite result after coefficientwise cancellation**, not an actually truncated geometric series. No analytic convergence assumption is involved.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work over $\mathbb C$ with finite-dimensional [Lie algebras](../../../lie-algebra.md) and [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) spaces. The adjoint form of [Engel theorem](../../../lie-algebra.md#engel-s-theorem) is

$$
\boxed{\mathfrak g\text{ is nilpotent }\Longleftrightarrow
\operatorname{ad}x\text{ is nilpotent for every }x\in\mathfrak g.}
$$

Here a [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra) has terminating [lower central series](../../../group-theory.md#lower-central-series), $\gamma_1\mathfrak g=\mathfrak g$, $\gamma_{j+1}\mathfrak g=[\mathfrak g,\gamma_j\mathfrak g]$. We prove the stronger linear statement: if $V\ne0$, $L\subseteq\mathfrak{gl}(V)$ and every member of $L$ is a [nilpotent endomorphism](../../../linear-operator-theory.md#nilpotent-linear-map), then there is a nonzero $v\in V$ killed by all of $L$, and $L$ can be simultaneously represented by [strictly upper triangular matrices](../../../linear-algebra.md#strictly-upper-triangular-matrix).

For the [proof of Engel theorem by induction and normalizers](../../../lie-algebra.md#proof-of-engel-theorem-by-induction-and-normalizers), first establish a useful nilpotence fact. If $x^m=0$, left and right multiplication by $x$ on $\operatorname{End}(V)$ commute. Expanding their difference gives

$$
(\operatorname{ad}x)^N(T)=\sum_{j=0}^N(-1)^j\binom Njx^{N-j}Tx^j.
$$

For $N=2m-1$, every summand contains a power of $x$ at least $m$, so $(\operatorname{ad}x)^{2m-1}=0$. Restrictions and induced quotient maps remain nilpotent.

Now prove the common-kernel statement, the [Engel lemma](../../../lie-algebra.md#engel-lemma), by induction on $\dim L$. The zero algebra is immediate. Choose a maximal proper [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) $M$. Its action on $L/M$ by commutators consists of nilpotent maps by the preceding fact. Applying the lower-dimensional induction hypothesis to its image gives a nonzero coset $y+M$ with $[M,y]\subseteq M$. Hence

$$
M\subsetneq N_L(M),\qquad
N_L(M)=\{z\in L:[z,M]\subseteq M\}.
$$

The [normalizer of a Lie subalgebra](../../../lie-algebra.md#normalizer-of-a-lie-subalgebra) is a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) by the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Maximality implies $N_L(M)=L$, so $M$ is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra). Moreover $L/M$ has no proper nonzero [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra), and every one-dimensional subspace is a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra). Thus $\dim L/M=1$.

Induction also provides a nonzero common annihilator

$$
W=\{v\in V:mv=0\text{ for all }m\in M\}.
$$

It is stable under $L$: for $m\in M$, $x\in L$, $v\in W$,

$$
m(xv)=x(mv)+[m,x]v=0,
$$

because $[m,x]\in M$. Choose $x$ representing a [basis](../../../vector-space.md#basis) of $L/M$. The restriction of the [nilpotent endomorphism](../../../linear-operator-theory.md#nilpotent-linear-map) $x$ to the nonzero space $W$ has nonzero [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). A vector in this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is killed by both $M$ and $x$, hence by all of $L$. This finishes the induction. When an action is not faithful, induction is applied to its image, whose [dimension](../../../vector-space.md#dimension-vector-space) is no larger than $\dim M$; no faithfulness assumption is hidden.

Starting with the common-kernel line, apply the same statement to each successive quotient [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) space. It constructs a [complete flag](../../../vector-space.md#complete-flag) of [invariant subspaces](../../../representation-theory.md#invariant-subspace)

$$
0=V_0\subset V_1\subset\cdots\subset V_d=V,\qquad
\dim V_j=j,\qquad LV_j\subseteq V_{j-1}.
$$

An adapted [basis](../../../vector-space.md#basis) represents every member of $L$ by a [strictly upper triangular matrix](../../../linear-algebra.md#strictly-upper-triangular-matrix). Every product of $d$ such matrices is zero, so every iterated commutator with $d$ entries is zero as well.

Finally, if every $\operatorname{ad}x$ on $\mathfrak g$ is nilpotent, apply the linear statement to the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). With $d=\dim\mathfrak g$, every product of $d$ adjoint operators vanishes, so $\gamma_{d+1}\mathfrak g=0$. Conversely, if $\gamma_{c+1}\mathfrak g=0$, then $(\operatorname{ad}x)^cy=0$ for all $x,y$, proving the other implication. **This proves Engel's theorem and its simultaneous-triangularization form.** The hypothesis concerns every element of the algebra, not merely a chosen set of generators.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The [Killing form](../../../lie-algebra.md#killing-form) is the [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form)

$$
\boxed{B(A,C)=\operatorname{tr}_{\mathfrak g}(\operatorname{ad}A\,\operatorname{ad}C).}
$$

The facts needed here are its invariance, $B([A,C],D)=B(A,[C,D])$, and the [root space](../../../semisimple-lie-algebra.md#root-space) identity $[H,X]=\alpha(H)X$. Invariance follows from $[\operatorname{ad}A,\operatorname{ad}C]=\operatorname{ad}[A,C]$ and cyclicity of the [trace](../../../linear-algebra.md#matrix-trace):

$$
\operatorname{tr}([\operatorname{ad}A,\operatorname{ad}C]\operatorname{ad}D)
=\operatorname{tr}(\operatorname{ad}A[\operatorname{ad}C,\operatorname{ad}D]).
$$

Taking $A=H$, $C=X$, $D=Y$ proves

$$
\boxed{B(H,[X,Y])=B([H,X],Y)=\alpha(H)B(X,Y).}
$$

No normalization of $X,Y$ is needed for this identity. Semisimplicity gives nondegeneracy of the [Killing form](../../../lie-algebra.md#killing-form), but that fact is not needed for this particular equality.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Use the standard [coroot](../../../semisimple-lie-algebra.md#coroot) normalization $\alpha(H_\alpha)=2$. The symbols $H_\alpha$ are vectors in the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra), not the root-space vectors $X_\alpha$. The [root-string theorem](../../../semisimple-lie-algebra.md#root-string-theorem) gives $\beta(H_\alpha)\in\mathbb Z$, so every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) takes real values on

$$
\mathfrak h_{\mathbb R}=\operatorname{span}_{\mathbb R}\{H_\beta:\beta\in\Phi\}.
$$

The simple [coroots](../../../semisimple-lie-algebra.md#coroot) form a [basis](../../../vector-space.md#basis) of this real space.

In the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition), $\operatorname{ad}H$ is zero on $\mathfrak h$ and [scalar multiplication](../../../vector-space.md#scalar-multiplication) by $\beta(H)$ on the one-dimensional space $\mathfrak g_\beta$. Therefore, for $H,K\in\mathfrak h$,

$$
B(H,K)=\sum_{\beta\in\Phi}\beta(H)\beta(K).
$$

For $H,K\in\mathfrak h_{\mathbb R}$ every term is real, so the restricted form is real. Moreover,

$$
B(H,H)=\sum_{\beta\in\Phi}\beta(H)^2\geq0.
$$

If it is zero, all $\beta(H)$ vanish. Then $H$ commutes with every [root space](../../../semisimple-lie-algebra.md#root-space) and with $\mathfrak h$, hence is central in $\mathfrak g$. The [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) vanishes for a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), so $H=0$. Thus the [Euclidean subspace of a Cartan subalgebra](../../../semisimple-lie-algebra.md#euclidean-subspace-of-a-cartan-subalgebra) has

$$
\boxed{B|_{\mathfrak h_{\mathbb R}}\text{ real and positive definite}.}
$$

Equivalently, positivity follows because the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) span $\mathfrak h^*$.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Put $H_{12}=E_{11}-E_{22}=[E_{12},E_{21}]$. The six [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) of $\mathfrak{sl}_3$ take values $2,-2,1,-1,-1,1$ on $H_{12}$, so the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) gives

$$
B(H_{12},H_{12})=2^2+(-2)^2+1^2+(-1)^2+(-1)^2+1^2=12.
$$

Using the preceding invariant-form identity with $\alpha=L_1-L_2$,

$$
B(H_{12},[E_{12},E_{21}])=\alpha(H_{12})B(E_{12},E_{21})=2B(E_{12},E_{21}).
$$

Hence

$$
\boxed{B(E_{12},E_{21})=6.}
$$

This agrees with the [Killing form of the special linear Lie algebra](../../../lie-algebra.md#killing-form-of-the-special-linear-lie-algebra), $B(A,C)=2n\operatorname{tr}(AC)$, at $n=3$.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

The [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is

$$
\boxed{\Lambda_W=\{\lambda\in\mathfrak h^*:\lambda(H_\alpha)\in\mathbb Z\text{ for every root }\alpha\}
=\bigoplus_{i=1}^r\mathbb Z\omega_i,}
$$

where the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) satisfy $\omega_i(H_{\alpha_j})=\delta_{ij}$. The [coroots](../../../semisimple-lie-algebra.md#coroot) use the normalization fixed above.

The [Killing form](../../../lie-algebra.md#killing-form) defines the complex-linear map

$$
\mathcal B:\mathfrak h\longrightarrow\mathfrak h^*,\qquad
\mathcal B(H)(K)=B(H,K).
$$

By [nondegeneracy of the Killing form on a Cartan subalgebra](../../../semisimple-lie-algebra.md#nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra), this is an isomorphism. For $H\in\mathfrak h_{\mathbb R}$, expand its image in the dual fundamental-weight [basis](../../../vector-space.md#basis):

$$
\mathcal B(H)=\sum_{i=1}^rB(H,H_{\alpha_i})\omega_i.
$$

The coefficients are real by the preceding positivity calculation, and the $\omega_i$ are in $\Lambda_W$. Consequently

$$
\boxed{\mathcal B(\mathfrak h_{\mathbb R})\subseteq\mathbb R\Lambda_W.}
$$

In fact both spaces have real [dimension](../../../vector-space.md#dimension-vector-space) $r$, so this inclusion is equality.

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

Evaluate the [Killing form](../../../lie-algebra.md#killing-form) on the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition). For arbitrary $K\in\mathfrak h$,

$$
\mathcal B(H_\alpha)(K)=B(H_\alpha,K)
=\sum_{\beta\in\Phi}\beta(H_\alpha)\beta(K).
$$

Thus the [Killing dual of a coroot](../../../semisimple-lie-algebra.md#killing-dual-of-a-coroot) is the [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) expansion

$$
\boxed{\mathcal B(H_\alpha)=\sum_{\beta\in\Phi}\beta(H_\alpha)\beta
=2\sum_{\beta\in\Phi^+}\beta(H_\alpha)\beta.}
$$

The factor two in the positive-root expression occurs because the contributions of $\beta$ and $-\beta$ are equal.

For $\mathfrak{sl}_3$, let $a=L_1-L_2$, $b=L_2-L_3$; the [positive roots](../../../semisimple-lie-algebra.md#positive-root) are $a,b,a+b$. On $H_{12}$ their values are $2,-1,1$. Therefore

$$
\mathcal B(H_{12})=2[2a-b+(a+b)]=6a,
\qquad
\boxed{\mathcal B(H_{12})=6(L_1-L_2)=12\omega_1-6\omega_2.}
$$

This uses the unscaled [Killing form](../../../lie-algebra.md#killing-form) $\operatorname{tr}(\operatorname{ad}A\operatorname{ad}C)$. Changing that normalization would change the scalar six.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Work with a finite-dimensional complex [semisimple Lie algebra](../../../semisimple-lie-algebra.md). The [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is obtained from its intrinsic [root system](../../../semisimple-lie-algebra.md#root-system), with several structure theorems entering the construction.

First choose a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) $\mathfrak h$. The semisimple structure theory gives the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,\qquad
\mathfrak g_\alpha=\{X:[H,X]=\alpha(H)X\text{ for all }H\in\mathfrak h\}.
$$

The nonzero [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) span $\mathfrak h^*$, [root spaces](../../../semisimple-lie-algebra.md#root-space) have [dimension](../../../vector-space.md#dimension-vector-space) one, and every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) has its negative. The rank is $r=\dim\mathfrak h$.

Next use the [Killing form](../../../lie-algebra.md#killing-form). Its nondegeneracy on $\mathfrak h$ and its positive-definite restriction to the real [coroot](../../../semisimple-lie-algebra.md#coroot) span identify the real [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) span $E=\mathbb R\Phi$ with a Euclidean space. Explicitly, if $t_\lambda=\mathcal B^{-1}(\lambda)$, put $(\lambda,\mu)=B(t_\lambda,t_\mu)$. The [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root) supplies its normalized [coroot](../../../semisimple-lie-algebra.md#coroot) $H_\alpha$ and the integral pairing

$$
\beta(H_\alpha)=\frac{2(\beta,\alpha)}{(\alpha,\alpha)}\in\mathbb Z.
$$

The [root-string theorem](../../../semisimple-lie-algebra.md#root-string-theorem) makes the reflection $s_\alpha(\beta)=\beta-\beta(H_\alpha)\alpha$ permute $\Phi$. Together with the absence of multiples other than $\pm\alpha$, this shows that $\Phi$ is a finite [reduced root system](../../../semisimple-lie-algebra.md#reduced-root-system) and a [crystallographic root system](../../../semisimple-lie-algebra.md#crystallographic-root-system). These properties come from [semisimple Lie algebra](../../../semisimple-lie-algebra.md) theory, not from the diagram's definition.

Choose a vector in $E$ that is not perpendicular to any [root](../../../semisimple-lie-algebra.md#root-of-a-root-system). Define the [positive roots](../../../semisimple-lie-algebra.md#positive-root) by positive inner product with this vector. The [simple roots](../../../semisimple-lie-algebra.md#simple-root) are those [positive roots](../../../semisimple-lie-algebra.md#positive-root) that cannot be expressed as sums of two [positive roots](../../../semisimple-lie-algebra.md#positive-root). Root-system theory shows that they form a [basis](../../../vector-space.md#basis) $\Delta=\{\alpha_1,\ldots,\alpha_r\}$, and each [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) is an integer combination of them with coefficients all of one sign. Distinct [simple roots](../../../semisimple-lie-algebra.md#simple-root) have nonpositive inner product.

Use the standard [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) convention

$$
A_{ij}=\alpha_i(H_{\alpha_j})=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)}.
$$

There is one diagram vertex for each [simple root](../../../semisimple-lie-algebra.md#simple-root). For $i\ne j$, the integral off-diagonal entries are nonpositive and

$$
A_{ij}A_{ji}=4\cos^2\theta_{ij}\in\{0,1,2,3\}.
$$

Connect the two vertices with respectively zero, one, two or three edges. The corresponding angles are $90^\circ,120^\circ,135^\circ,150^\circ$. A multiple edge carries an arrow **toward the shorter [root](../../../semisimple-lie-algebra.md#root-of-a-root-system)**. For joined vertices, the length ratio is determined by $A_{ij}/A_{ji}=(\alpha_i,\alpha_i)/(\alpha_j,\alpha_j)$; hence the diagram records both angle and relative length.

For example, $\mathfrak{sl}_3$ has [simple roots](../../../semisimple-lie-algebra.md#simple-root) $L_1-L_2$ and $L_2-L_3$, giving two equal-length vertices joined by one edge: type $A_2$. For $\mathfrak{sp}_4$, take $\alpha_1=L_1-L_2$ and $\alpha_2=2L_2$. Then

$$
A=\begin{pmatrix}2&-1\\-2&2\end{pmatrix},
$$

so the two vertices have a double edge directed toward $\alpha_1$, the shorter [root](../../../semisimple-lie-algebra.md#root-of-a-root-system): type $C_2$.

Finally, orthogonal irreducible components of the [root system](../../../semisimple-lie-algebra.md#root-system) correspond to the simple [ideals of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) in the [semisimple Lie algebra](../../../semisimple-lie-algebra.md), so its diagram is the disjoint union of their connected diagrams. Conjugacy of [Cartan subalgebras](../../../semisimple-lie-algebra.md#cartan-subalgebra) and the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) action on choices of [positive roots](../../../semisimple-lie-algebra.md#positive-root) make the resulting diagram independent of these choices up to isomorphism. **Thus the vertices, edge multiplicities, arrows and connected components encode the simple-root geometry and the simple-ideal decomposition.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
