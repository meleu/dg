---
{"dg-publish":true,"permalink":"/notes/books/code-complete/code-complete-checklist-requirements/"}
---

# Code Complete - Checklist - Requirements



## Specific Functional Requirements

- Are all the tasks the user wants to perform specified?
- Is the data used in each task and the data resulting from each task specified?
- Are all thee inputs to the system specified?
    - including their source, accuracy, range of values, and frequency?
- Are all the outputs from the system specified?
    - including their destination, accuracy, range of values, frequency and format?
- Are all output formats specified for Web pages, reports and so on?

- Are all the external hardware and software interfaces specified?
- Are all the external communication interfaces specified?
    - including handshaking, error-checking, and communication protocols?

## Specific Nonfunctional (Quality) Requirements

- Is the expected response time, from the user's point of view, specified for all necessary operations?
- Are other timing considerations specified?
    - such as processing time, datatransfer rate, and system throughput?
- Is the level of security specified?
- Is the reliability specified?
    - consequences of software failure
    - the vital information that needs to be protected from failure
    - the strategy for error detection and recovery
- Are minimum machine memory, CPU and free disk space specified?
- Is the maintainability of the system specified?
    - including its ability to adapt to changes in specific functionality, changes in the operating environment, and changes in its interfaces with other software
- Is the definition of success Included? Of failure?


## Requirements Quality

- Are the requirements written in the user's language?
    - Do the users think so?
- Does each requirement avoid conflicts with other requirements?
- Are acceptable tradeoffs between competing attributes specified?
    - example: between robustness and correctness
- Do the requirements at a fairly consistent level of detail?
    - Should any requirement be specified in more detail?
    - Should any requirement be specified in less detail?
- Are the requirements clear enough to be turned over to an independent group for construction and still be understood?
    - Do the developers think so?
- Is each item relevant to the problem and its solution?
    - Can each item be traced to its origin in the problem environment?
- Is each requirement testable?
    - Will it be possible for independent testing to determine whether each requirement has been satisfied?
- Are all possible changes to the requirements specified, including the likelihood of each change?

## Requirements Completeness

- Where information isn't available before development begins?
    - are the areas of incompleteness specified?
- Are the requirements complete in the sense that if the product satisfies every requirement, it will be acceptable?
- Are you comfortable with all the requirements?
    - Have you eliminated requirements that are impossible to implement and included just to appease your customer or your boss?

