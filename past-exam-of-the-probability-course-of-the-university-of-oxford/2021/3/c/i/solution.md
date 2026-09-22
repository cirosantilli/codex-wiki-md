<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define

$$
L=\{-c-b,\ldots,-c-1\},\quad U=\{c+1,\ldots,c+a\},\quad
C=L\cup I\cup U=\{-c-b,\ldots,c+a\}.
$$

An interior jump cannot go below $-c-b$ or above $c+a$, and every exterior reset lands in $I$. Thus $C$ is closed.

To prove that it is one [communicating class](../../../../../communicating-class.md), start anywhere in $C$. From $L$ or $U$, a reset can reach $I$ with positive [probability](../../../../../probability.md). From any state of $I$, repeated $+a$ steps reach some state of $U$, after staying in $I$ up to the last step. A reset from this state can reach every point of the consecutive block

$$
B=\{c-b+1,\ldots,c\}.
$$

Every [integer](../../../../../integer-split.md) $j\in\{-c-b,\ldots,c\}$ has the form $t-kb$ for some $t\in B$ and an [integer](../../../../../integer-split.md) $k\geq0$. Repeated $-b$ steps from $t$ reach $j$, with all departure states in $I$ until a possible last step into $L$. This gives access to all of $I\cup L$. Finally, each $j\in U$ can be reached from $j-a\in I$. Every path described has strictly positive [probability](../../../../../probability.md). Therefore every state in $C$ reaches every other state in $C$.

Each state outside $C$ can only stay put or reset into $I$, and no transition from $C$ returns to it. Different states outside $C$ cannot reach one another. Hence the complete list of [communicating classes](../../../../../communicating-class.md) is

$$
\boxed{C=\{-c-b,\ldots,c+a\}\text{, and }\{i\}\text{ for each }i\notin C.}
$$

The finite class $C$ is the unique [closed communicating class](../../../../../closed-communicating-class.md). The exterior singleton classes are [transient communicating classes](../../../../../transient-communicating-class.md), since their self-transition [probabilities](../../../../../probability.md) are strictly less than one. Notice that this reachability proof does not require $a,b$ to be [coprime](../../../../../coprime-integers.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
