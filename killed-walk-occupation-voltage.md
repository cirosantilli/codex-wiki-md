# Killed-walk occupation voltage

↑ **Parent:** [Expected occupation count before absorption](expected-occupation-count-before-absorption.md)

For [simple random walk](simple-random-walk.md) on a finite connected loopless unweighted [graph](graph-split.md), start at $a\ne z$ and stop on first hitting $z$. If

$$
g_{az}(u)=\mathbb E_a\sum_{t<T_z}\mathbf1_{\{X_t=u\}},\qquad v_{az}(u)=\frac{g_{az}(u)}{\deg(u)},
$$

then $v_{az}(z)=0$ and $Lv_{az}=\delta_a-\delta_z$ for the [Graph Laplacian](laplacian-matrix.md) $L$. The incoming-visit balance equation is $g_{az}(u)=\mathbf1_{\{u=a\}}+\sum_{w\sim u}g_{az}(w)/\deg(w)$ for $u\ne z$; at $z$ the Laplacian value is $-1$ because all its coordinates sum to zero. Thus $v_{az}$ is the [voltage](voltage.md) for unit current from $a$ to $z$, and $v_{az}(a)=R_{\mathrm{eff}}(a,z)$. In particular, the expected number of directed transitions $u\to w$ before $T_z$ is $v_{az}(u)$.

## ↑ Ancestors (8)

1. [Expected occupation count before absorption](expected-occupation-count-before-absorption.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Directed edge occupation in a random-walk commute](directed-edge-occupation-in-a-random-walk-commute.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/b/solution.md)
