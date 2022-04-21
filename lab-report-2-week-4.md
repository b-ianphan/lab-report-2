# CSE15L Lab report 2 | Week 4
```
Written and Submitted by: Billy Phan
```
---

```Code Change 1```

> First Code Diff: 

![CodeChange1](cse15l-lab-report-2-ss1.png)

*See why we needed to make this change here:*
[Failure Inducing Symptom](https://github.com/b-ianphan/markdown-parser/blob/main/breakingTest.md)

> Output of Symptom:

![Symptom1Output](cse15l-lab-report-2-ss2.png)

> Explanation: 

Our code prior to fixing was essentially reading the index of `Closing Parenthesis: ")"` as "-1" it couldn
't be found), so when our program would take note of a link using `.add` there would be an `indexOutOfBoundsException` (Our symptom). This output only occurs when we pass to it a file where we have a open paranthesis withouted a paired closing one `Ex: [...](...`.

---

> 