# STRIPS

↑ **Parent:** [Artificial intelligence](artificial-intelligence-split.md)

A representation for [automated planning](automated-planning.md) in which a state $S$ is a [set](set-split.md) of true ground facts and an action has a positive [precondition](precondition.md) set $P$, add set $A$ and delete set $D$. Under the [closed-world assumption](closed-world-assumption.md), facts absent from $S$ are false. The action applies when $P\subseteq S$ and produces

$$
S'=(S\setminus D)\cup A.
$$

Negative effects are delete-list entries; they do not require negative [preconditions](precondition.md). A movement action must delete an object's old location as well as add its destination. Capacity and safety restrictions require explicit action conditions or auxiliary [planning fluents](planning-fluent.md); they do not follow automatically from an intended physical interpretation.

**Table of contents**

- [Precondition-free STRIPS planning](precondition-free-strips-planning.md)
  - [Last-achiever algorithm for precondition-free planning](last-achiever-algorithm-for-precondition-free-planning.md)
- [Action schema](action-schema.md)
  - [Ground action](ground-action.md)
    - [Action grounding](action-grounding.md)
- [Static predicate](static-predicate.md)

## ↑ Ancestors (3)

1. [Artificial intelligence](artificial-intelligence-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Automated planning](automated-planning.md)
- [Blocks world](blocks-world.md)
- [Classical planning](classical-planning.md)
- [Closed-world assumption](closed-world-assumption.md)
- [Delete-relaxation heuristic](delete-relaxation-heuristic.md)
- [Forward state-space planning](forward-state-space-planning.md)
- [Frame axiom](frame-axiom.md)
- [Ground atom](ground-atom.md)
- [Intelligent Systems examination paper by the University of Oxford (2015)](intelligent-systems-examination-paper-by-the-university-of-oxford-2015.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/2/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/2/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/3/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/3/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/3/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/g/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/h/solution.md)
- [Plan](plan.md)
- [Planning fluent](planning-fluent.md)
- [Planning safety certificate](planning-safety-certificate.md)
