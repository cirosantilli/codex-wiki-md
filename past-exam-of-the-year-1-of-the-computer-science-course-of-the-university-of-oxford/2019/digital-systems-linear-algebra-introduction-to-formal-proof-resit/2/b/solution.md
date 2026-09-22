<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Provide a blocking [request-reply sensor conversion](../../../../../request-reply-sensor-conversion.md) operation, using [synchronous send-and-receive](../../../../../synchronous-send-and-receive.md) when the system supplies it:

```
get_temp():
    token := a new token for this process's call
    reply := request-and-wait(
        destination = temperature_driver,
        message = REQUEST(self, token),
        expected_reply = RESULT(token, value))
    return reply.value
```

Here `request-and-wait` means sending the request and remaining ready to accept its matching response; it denotes a protocol action, not a claimed library symbol. Separate blocking send and receive operations are also adequate if they preserve the sender identity and the reply cannot be lost between them. With a synchronous reply, the driver simply waits until this client's receive is ready.

The call returns only after the driver has selected this request, issued `TEMP_START`, observed completion, read the new value and replied with the matching token. **Each call therefore starts its own fresh conversion and returns its own result.** It never returns a cached sample or another caller's reply. Local request and response storage belong to the calling process and are not a shared global message buffer.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
