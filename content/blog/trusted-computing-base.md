+++
title = "Trusted Computing Base - Mindmap"
date = "2024-09-03T10:00:25-08:00"

description = "A Trusted Computing Base (TCB) is the totality of the protection mechanisms within a system or architecture that work together to enforce a security policy."

tags = ["blue-teaming","compliance","cybersecurity","policy"]
+++

A ***Trusted Computing Base (TCB)*** is the **totality** of the **protection** **mechanisms** within a **system** or architecture that work together to **enforce** a **security policy**.

### Definition Simplified
    
***Totality***: ALL

***Protection Mechanisms***:

- Hardware (TPM)
- Firmware (Code signing)
- Software (Anti-virus)

![*Figure: Mindmap for TCB*](https://auti.dev/images/blog/trusted-computing-base/mindmap.png)

*Figure: Mindmap for TCB*

A ***Trusted Computing Base*** comprises all of the protection mechanisms: 

- People
- Processes
- Technology

## Reference Monitor Concept (RMC)

A ***reference monitor*** is an **access control** concept of an abstract machine that **mediates** all **accesses** **to objects by subjects**.

*Definition 20–3. [50]* 

- If we want to **control security** we have to **control what subjects are allowed to** control objects, and what specifically can **do with objects.**
- The elements in RMC
    - A ***subject*** is an active entity
    - A ***mediation*** is required to control subject’s access to an object; it makes decisions based on rules
    - Every control also has to have an ***assurance*** aspect (we need to know if the mediation is working correctly); ***Logging & Monitoring***
    - An ***object*** is a passive entity (it is been accessed by the subject)

![*Figure: Reference Monitor Concept*](https://auti.dev/images/blog/trusted-computing-base/reference-monitor-concept.png)

*Figure: Reference Monitor Concept*

## Reference Monitor Principles

1. **Tamper Proof**
    - **Isolation**: protected from unauthorized ***alteration***
    - Resists subversion and malicious software
2. **Always invoked (non by-passable)**
    - **Completeness:** every access is ***mediated***
3. Small and simple enough to **allow assurance** of its correctness
    - **Verifiability**: ***verified*** to perform its functions properly
    - Ability to implement policy with high assurance

*Defines what it means for a system to be **“secure”**. Most system vulnerabilities can be traced to violations of one or more of the RM principles*

### Security Kernel

A ***security kernel*** is a **combination** of **hardware & software** that **implements** a **reference monitor**.

- Constantly monitors and controls access to critical system components.
- Ensures that only authorized processes and users can interact with sensitive data and functionality.
- Enforces a set of predefined security policies to create a robust barrier against potential threats.
- A compact and well-defined structure that allows for thorough testing and verification.


### Resources

---

- Chapter 20 Building Systems with Assurance, Computer Security Art and Science, 2nd Edition
- [Destination Certification - Trusted Computing Base MindMap (3 of 9) | CISSP Domain 3](https://www.youtube.com/watch?v=N4bZSoV2yis)