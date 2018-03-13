**Motivation:** There is a need to identify requirements of a software project. Earlier attempts in this area have been to use source code to generate software requirements. Considering the huge amount of information contained in other artifacts associated with software like issues, commits, authors, pull requests, etc. we plan to use these artifacts over source code to identify or generate software requirements.

**Recent Work:**

We found a Research paper that appeared in *ICSEA 2012 : The Seventh International Conference on Software Engineering Advances* titled **Tracing requirements and source code changes during software development.**

[Link to paper]()

The paper defines a model for Tracing links between a given set of requirements and artifacts associated with a software project. This model named Traceability integration model (TIM) is built over the standard model in software Engineering called Management-based Unified Software Engineering (MUSE).

With their work on traceability, they answer 5 most important questions asked by developers w.r.t software requirements. These are as follows:

1. Which code is involved in the implementation of this feature?
2. To move this feature into this code, what else needs to be moved?
3. What is the program supposed to do?
4. Why was this code implemented this way?
5. What have my co-workers been doing?
6. What will be the impact of this change?

**Our tool:**
- We believe that these questions can be answered by extracting information from the above mentioned artifacts associated with the software project. For ex. We can answer "what have my coworkers been doing?" by looking at the commits made by the coworker and files modified or added by the coworker.
- Huge information contained in the commit messages can be extracted to identify keywords that may relate to functional requirements of the project.
- Bug fixes are indicative of fixed features while feature additions directly indicate the functional requirements.

Considering all these, we propose a tool that can **Identify functional requirements given the artifacts associated with the software project.**
