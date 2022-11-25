---
{"dg-publish":true,"permalink":"/atomic-ideas/managing-complexity/"}
---

# managing complexity

In software literature there are many references from the "great masters" talking about how important it is to **manage complexity**.


## Problems caused by complexity

From [[notes/books/O Mitico Homem-Mes\|O Mitico Homem-Mes]] (Mythical Man Month).

- Complexity causes:
    - harder communication between team members, which leads to deficiencies in the product, **increased costs**, and **delayed schedule**.
    - difficulty in list and understand all possible states of a program, which causes lack of confidence.
    - difficulty to evolve the software without creating side effects.
    - unnoticed states, which leads to security vulnerabilities


## Software's Primary Technical Imperative: Managing Complexity

From [[notes/books/code-complete/Code Complete\|Code Complete]].

> When projects fail for reasons that are primarily technical, the reason is often uncontrolled complexity. The software is allowed to grow so complex that no one really knows what it does. When a project reaches the point at which no one completely understands the impact that code changes in one area will have on other areas, progress grinds to a halt.


## The Lehman's Law of Increasing Complexity

> As a system evolves, it's complexity increases **unless work is done to reduce it**.

We can't have software teams as blind feature factories, piling more and more features on to software in the hope it will survive in the long run.

We **must** keep managing the complexity of the system as the knowledge of our domain changes.


## references

- [[notes/books/O Mitico Homem-Mes\|O Mitico Homem-Mes]]
- [[notes/books/code-complete/Code Complete\|Code Complete]]
- [Lehman's laws of software evolution](https://en.wikipedia.org/wiki/Lehman%27s_laws_of_software_evolution)
- Learn Go with tests - [Why unit tests and how to make them work for you](https://quii.gitbook.io/learn-go-with-tests/meta/why)