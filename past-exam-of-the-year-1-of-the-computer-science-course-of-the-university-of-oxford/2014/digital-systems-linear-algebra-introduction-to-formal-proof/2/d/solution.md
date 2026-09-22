<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An [access control list](../../../../../access-control-list.md) is attached to an object, such as a [file](../../../../../computer-file.md), and lists which subjects or groups may perform which operations. Access requires checking the requesting identity against that object's list. A [security capability](../../../../../capability-computer-security.md) is an unforgeable reference to an object carrying specified rights; possessing valid authority is what permits access. Protected storage or another integrity mechanism must prevent users manufacturing stronger [security capabilities](../../../../../capability-computer-security.md).

The traditional [Unix](../../../../../unix.md) owner/group/other read-write-execute permissions are a compact, restricted [access control list](../../../../../access-control-list.md): the [inode](../../../../../inode.md) records the owner, group and permission [bits](../../../../../bit.md), and the [operating system](../../../../../operating-system-split.md) compares these against the caller's credentials.

$$
\boxed{\text{Traditional Unix file protection is closest to access control lists}.}
$$

An already-open [file descriptor](../../../../../file-descriptor.md) can behave like a limited handle carrying rights, but that does not change the identity-based nature of the initial pathname permission check.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
