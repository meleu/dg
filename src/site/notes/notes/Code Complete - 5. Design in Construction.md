---
{"dg-publish":true,"permalink":"/notes/code-complete-5-design-in-construction/"}
---

## Chapter 5 - Design in Construction


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


### Desirable Characteristics of a Design

- Minimal complexity
- Ease of maintenance
- Loose coupling
- Extensibility
- Reusability
- High fan-in
    - meaning: high number of "clients" using a given class.
- Low-to-medium fan-out
    - meaning: a given class use a low-to-medium number of other classes
    - high fan-out (more than about seven) indicates that a class may be overly complex.
- Portability
- Leanness
    - no extra parts, nothing more to be removed
    - code is liability
- Stratification
    - design the system so that you can view it at one level without dipping into other levels
    - example: if you have to use a lot of older, poorly designed code, write a layer on top of it offering a simplified interface.
- Standard techniques
    - Have a coding style, a standard tooling, etc.


