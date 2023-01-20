---
{"dg-publish":true,"permalink":"/atomic-ideas/managing-complexity/"}
---

# managing complexity

In software literature there are many references from the "great masters" talking about how important it is to **manage complexity**.


## Problems caused by complexity

From [[notes/books/O Mitico Homem-Mes\|O Mitico Homem-Mes]] (The Mythical Man Month).

- Complexity causes:
    - harder communication between team members, which leads to deficiencies in the product, **increased costs**, and **delayed schedule**.
    - difficulty in list and understand all possible states of a program, which causes lack of confidence.
    - difficulty to evolve the software without creating side effects.
    - unnoticed states, which leads to security vulnerabilities


## Software's Primary Technical Imperative: Managing Complexity

From [[notes/books/code-complete/Code Complete\|Code Complete]].


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/notes/books/code-complete/code-complete-5-2-sotfware-s-primary-technical-imperative-managing-complexity/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




### Code Complete - 5.2. Sotfware's Primary Technical Imperative: Managing Complexity

> Once you understand that all other technical goals in software are secondary to managing complexity, many design considerations become straightforward.

I noticed how this thought influenced me when I check commit diffs. If the code is not simpler, I'm not satisfied.

> You might think of this as mental juggling - the more mental balls the program requires you to keep in the air at once, the more likely you'll drop one of the balls, leading to a design or coding error.
> 
> (...) If your design doesn't let you safely ignore most other parts of the program when you're immersed in one specific part, the design isn't doing its job.

Complexity is one of the reasons for project failure:

> When projects fail for reasons that are primarily technical, the reason is often uncontrolled complexity. The software is allowed to grow so complex that no one really knows what it does. When a project reaches the point at which no one completely understands the impact that code changes in one area will have on other areas, progress grinds to a halt.


</div></div>



## Lehman's Law of Increasing Complexity

> As a system evolves, it's complexity increases **unless work is done to reduce it**.

We can't have software teams as blind feature factories, piling more and more features on to software in the hope it will survive in the long run.

We **must** keep managing the complexity of the system as the knowledge of our domain changes.


## Tesler's Law of Conservation of Complexity

> Every application has an inherent amount of complexity that cannot be removed or hidden. Instead, it must be dealt with, either in product development or in user interaction.

We should never use this 👆 as an excuse to tolerate "artificial" complexity.

This law refers to the "minimal amount of complexity" in a system. Such complexity cannot be reduced, but "shifted" from a step in the value stream to another. Despite this law, you must always keep your eyes open and avoid increasing the "artificial" complexity (the complexity caused by bad design, bad coding practices, etc.).


## references

- [[notes/books/O Mitico Homem-Mes\|O Mitico Homem-Mes]]
- [[notes/books/code-complete/Code Complete\|Code Complete]]
- [Lehman's laws of software evolution](https://en.wikipedia.org/wiki/Lehman%27s_laws_of_software_evolution)
- Learn Go with tests - [Why unit tests and how to make them work for you](https://quii.gitbook.io/learn-go-with-tests/meta/why)