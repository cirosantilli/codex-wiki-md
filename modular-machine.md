# Modular machine

↑ **Parent:** [Turing machine](turing-machine.md)

A modular machine of modulus $m>1$ acts on pairs in $\mathbb N^2$. Each instruction $(a,b,c,R)$ or $(a,b,c,L)$ has $0\le a,b<m$ and $0\le c<m^2$, and at most one instruction is assigned to each residue pair $(a,b)$. The two transition types are $(mu+a,mv+b)\mapsto(m^2u+c,v)$ and $(mu+a,mv+b)\mapsto(u,m^2v+c)$. These finite arithmetic operations can encode a [Turing machine](turing-machine.md); a designated terminal configuration can have a nonrecursive [halting set](halting-set.md).

**Table of contents**

- [Group encoding of a modular machine](group-encoding-of-a-modular-machine.md)
- [Halting set at a designated terminal configuration](halting-set-at-a-designated-terminal-configuration.md)

## ↑ Ancestors (4)

1. [Turing machine](turing-machine.md)
2. [Theoretical computer science](theoretical-computer-science.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Group encoding of a modular machine](group-encoding-of-a-modular-machine.md)
- [Halting set at a designated terminal configuration](halting-set-at-a-designated-terminal-configuration.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104/5/c/solution.md)
