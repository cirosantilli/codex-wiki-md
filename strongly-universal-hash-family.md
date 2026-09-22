# Strongly universal hash family

↑ **Parent:** [Universal hash family](universal-hash-family.md)

A [strongly universal hash family](strongly-universal-hash-family.md) makes every [ordered pair](ordered-pair.md) of [outputs](output-computing.md) equally likely: for distinct [inputs](input-computer-science.md) $x,y$ and arbitrary specified [outputs](output-computing.md) $u,v$,

$$
\Pr_h[h(x)=u,h(y)=v]=\frac1{q^2}.
$$

Thus the two [outputs](output-computing.md) are [independent random variables](independent-random-variables.md), each with the [uniform distribution on a finite set](discrete-uniform-distribution.md). Adding the $q$ equal [ordered pairs](ordered-pair.md) gives collision [probability](probability.md) $q/q^2=1/q$, so the family is also a [universal hash family](universal-hash-family.md).

Here is a completely enumerable example. In the [finite field](finite-field.md) $\mathbb F_5$, take the [affine functions](affine-function.md) $h_{a,b}(x)=ax+b$, using [modular arithmetic](modular-arithmetic-split.md) modulo $5$. Choose $a$ and $b$ as [independent random variables](independent-random-variables.md), each with the [uniform distribution on a finite set](discrete-uniform-distribution.md) of all five [finite field](finite-field.md) elements $0,1,2,3,4$, including $a=0$. There are $25$ equally likely [hash functions](hash-function.md). For $x=0,y=1$, the [ordered pair](ordered-pair.md) is $(b,a+b)$. For instance $(a,b)=(2,3)$ gives $(h(0),h(1))=(3,0)$; $(0,3)$ gives $(3,3)$. Every prescribed $(u,v)$ occurs exactly once, at $b=u,a=v-u$.

<a id="image-enumerating-all-affine-hash-functions-over-the-finite-field-with-five-elements"></a>
![](affine-hash-pair-grid.png)

**[Figure 20](#image-enumerating-all-affine-hash-functions-over-the-finite-field-with-five-elements). Enumerating all affine hash functions over the finite field with five elements**. Each cell shows the unique coefficient pair (a,b) producing the displayed outputs at 0 and 1. Removing a = 0 deletes the diagonal and leaves dependent outputs despite uniform individual values.

Each row contains five choices, so each individual [output](output-computing.md) has [probability](probability.md) $5/25=1/5$. Each cell has [probability](probability.md) $1/25$, and the five diagonal cells give collision [probability](probability.md) $5/25=1/5$. For any distinct $x,y$, the same conclusion follows from $a=(v-u)/(y-x)$ and $b=u-ax$: a nonzero [finite field](finite-field.md) element has a unique inverse. This is the beauty of the construction: two small random coefficients provide exact pair balance without choosing five unrelated values.

The example uses equal-sized [input](input-computer-science.md) and [output](output-computing.md) [sets](set-split.md) to make every choice visible; it illustrates the family definitions rather than compression. In a larger [input](input-computer-science.md) [set](set-split.md), a [hash function](hash-function.md) cannot avoid all collisions into five buckets. What a [universal hash family](universal-hash-family.md) controls is the fraction of its members that collide on each fixed pair, rather than the existence of any collision anywhere.

Restricting to $a\ne0$ leaves $20$ [permutations](permutation.md) with zero collision [probability](probability.md) for distinct [inputs](input-computer-science.md). Individual [outputs](output-computing.md) remain uniform, but given $h(0)=u$, the four values other than $u$ each have [conditional probability](conditional-probability.md) $1/4$ and $u$ has zero. Hence these [outputs](output-computing.md) are not [independent random variables](independent-random-variables.md): this is a [universal hash family](universal-hash-family.md) but not a [strongly universal hash family](strongly-universal-hash-family.md). Finally, the full $25$-member example contains five constant [functions](function-split.md), with immediately visible collisions. Its pair guarantee concerns a random choice of [hash function](hash-function.md), and makes no claim of cryptographic [collision resistance](collision-resistance.md).

## ↑ Ancestors (4)

1. [Universal hash family](universal-hash-family.md)
2. [Hash function](hash-function.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Almost strongly universal hash family](almost-strongly-universal-hash-family.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/3/solution.md)
- [Strongly universal hash family](strongly-universal-hash-family.md)
- [Universal hash family](universal-hash-family.md)
