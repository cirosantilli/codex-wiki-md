<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

Let $f:(C,d)\to(C',d')$ be a [chain map](../../../../../chain-map.md), so

$$
d'_if_i=f_{i-1}d_i.
$$

If $x\in C_i$ is a cycle, then $d'f_i(x)=f_{i-1}d(x)=0$, so $f_i(x)$ is a cycle. If $x=d_{i+1}y$ is a boundary, then

$$
f_i(x)=f_id_{i+1}y=d'_{i+1}f_{i+1}y
$$

is a boundary. Hence

$$
f_*:H_i(C)\longrightarrow H_i(C'),
\qquad [x]\longmapsto[f_i(x)]
$$

is a well-defined [induced map on homology](../../../../../induced-map-on-homology.md).

The maps $f$ and $g$ are [chain homotopic](../../../../../chain-homotopy.md) if there are homomorphisms

$$
h_i:C_i\longrightarrow C'_{i+1}
$$

such that

$$
f_i-g_i=d'_{i+1}h_i+h_{i-1}d_i.
$$

For a cycle $x$, this gives

$$
f_i(x)-g_i(x)=d'_{i+1}h_i(x),
$$

which is a boundary. Thus $f_*[x]=g_*[x]$ and $f_*=g_*$ on [homology](../../../../../homology-split.md).

Now consider the proposed [mapping cone](../../../../../mapping-cone-homological-algebra.md) $M(f)$. Applying its differential twice gives

$$
(d_f)_{i-1}(d_f)_i
=
\begin{pmatrix}
d_{i-2}d_{i-1}&0\\
(-1)^{i-1}f_{i-2}d_{i-1}+(-1)^id'_{i-1}f_{i-1}
&d'_{i-1}d'_i
\end{pmatrix}.
$$

The diagonal entries vanish because $C$ and $C'$ are [chain complexes](../../../../../chain-complex.md), and the lower-left entry is

$$
(-1)^{i-1}(f_{i-2}d_{i-1}-d'_{i-1}f_{i-1})=0
$$

by the chain-map identity. Therefore $d_f^2=0$ and $M(f)$ is a chain complex.

There is a [short exact sequence of chain complexes](../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow C'
\xrightarrow{\ j\ }M(f)
\xrightarrow{\ p\ }C[-1]
\longrightarrow0,
$$

where

$$
j_i(y)=(0,y),
\qquad p_i(x,y)=x,
\qquad C[-1]_i=C_{i-1}.
$$

Its [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) is

$$
\cdots\longrightarrow H_i(C')
\longrightarrow H_i(M(f))
\longrightarrow H_{i-1}(C)
\xrightarrow{\ \delta_i\ }H_{i-1}(C')
\longrightarrow\cdots.
$$

To identify the connecting map, represent a class in $H_{i-1}(C)$ by a cycle $x$ and lift it to $(x,0)\in M(f)_i$. Then

$$
(d_f)_i(x,0)
=(0,(-1)^if_{i-1}x),
$$

so

$$
\delta_i=(-1)^if_*.
$$

At the preceding occurrence the degree is $i+1$, giving $(-1)^{i+1}f_*$. Hence the sequence is exactly

$$
\cdots\longrightarrow H_i(C)
\xrightarrow{(-1)^{i+1}f_*}H_i(C')
\longrightarrow H_i(M(f))
\longrightarrow H_{i-1}(C)
\xrightarrow{(-1)^if_*}H_{i-1}(C')
\longrightarrow\cdots.
$$

Finally suppose $f-g=d'h+hd$. Define

$$
\Phi_i:M(f)_i\longrightarrow M(g)_i,
\qquad
\Phi_i(x,y)=\bigl(x,y+(-1)^ih_{i-1}x\bigr).
$$

A direct calculation gives

$$
\begin{aligned}
(d_g)_i\Phi_i(x,y)
&=\left(d x,(-1)^igx+d'y+(-1)^id'hx\right),\\
\Phi_{i-1}(d_f)_i(x,y)
&=\left(d x,(-1)^ifx+d'y+(-1)^{i-1}hdx\right).
\end{aligned}
$$

These are equal precisely because $f-g=d'h+hd$. Thus $\Phi$ is a chain map. Replacing the plus sign in its definition by a minus sign gives its inverse, so $M(f)$ and $M(g)$ are isomorphic as chain complexes.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
