<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a signature, adding a fresh constant if it otherwise has no ground terms. Its [Herbrand universe](../../../../../herbrand-universe.md) $U$ is the set of all ground terms, and its [Herbrand base](../../../../../herbrand-base.md) $B$ is the set of all [ground atoms](../../../../../ground-atom.md) over $U$. A [Herbrand interpretation](../../../../../herbrand-structure.md) is identified with a subset $I\subseteq B$: precisely its members are true. Function symbols and constants have their term interpretations.

A [least Herbrand model](../../../../../least-herbrand-model.md) of a [knowledge base](../../../../../knowledge-base.md) $\mathcal K$ is a [Herbrand model](../../../../../herbrand-model.md) $M$ satisfying

$$
\boxed{M\models\mathcal K\quad\text{and}\quad M\subseteq J\text{ for every Herbrand model }J\models\mathcal K.}
$$

If it exists, it is unique. This is stronger than being minimal: a minimal model merely has no strictly smaller model contained in it.

For a positive definite [Datalog](../../../../../datalog.md) program with facts, let $T$ add every fact and the head of every ground rule whose body is already true. Starting from the empty set and repeatedly adding consequences yields

$$
\boxed{M=\bigcup_{n\ge0}T^n(\varnothing)=\bigcap\{J:J\text{ is a Herbrand model of }\mathcal K\},}
$$

where $T$ is taken inflationary, so it also retains its input. Every added [ground atom](../../../../../ground-atom.md) belongs to every model, and the union is closed under every finite rule body. These two facts establish that it is the [least Herbrand model](../../../../../least-herbrand-model.md). The intersection assertion is guaranteed here by the definite Horn form, not for arbitrary [knowledge bases](../../../../../knowledge-base.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
