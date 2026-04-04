# How to Give and Receive Effective Code Reviews

> **TL;DR:** Code reviews improve quality and prevent knowledge silos, but only when done well. Be constructive, not critical. Focus feedback on substance, not preference. Keep reviews fast (24-48 hours). The goal is to help the author improve, not to prove you're smarter.

## Purpose

Code reviews maintain quality and prevent knowledge silos. Every change requires at least one review before merging to main.

---

## For Reviewers

### Your Role as a Reviewer

As a reviewer, your job is to ensure that code being merged meets our quality standards while being respectful and constructive toward the author.

### What to Look For

- **Design & Complexity**: Well-architected and understandable?
- **Functionality & Tests**: Works correctly? Tests comprehensive?
- **Naming & Style**: Clear names and conventions followed?
- **Documentation**: Updated if needed?

### Who Should Review

Best reviewers know the code well. Assign to CODEOWNERS. For complex changes, get multiple reviewers.

### Review Etiquette

- Review code, not character
- Ask questions to encourage reflection
- Be specific—point to exact lines
- Respond within 24 hours
- Flag blocking issues separately

### Feedback Levels

- **MUST FIX**: Bugs, security issues, architectural problems
- **SHOULD FIX**: Performance, readability, maintainability improvements
- **NICE TO HAVE**: Learning suggestions
- **APPROVED**: Ready to merge

---

## For Authors

### Before Requesting Review

- Keep PRs small (reviewable in 30 minutes)
- Write clear PR description
- Self-review first
- Tests pass locally

### Responding to Feedback

- Ask for clarification if needed
- Explain your reasoning if you disagree
- Address feedback quickly
- Thank reviewers

### Handling Disagreements

Focus on facts. Reference style guides or architecture decisions. If stuck, involve a tech lead.

---

## Best Practices & Common Mistakes

### Key Principles

- Review code, not character
- Target 24-hour turnaround
- Be specific and constructive
- Use positive tone

### What to Avoid

**Reviewers**: Dismissiveness, style focus, blocking on preferences

**Authors**: Large PRs, defensive responses, merging with unresolved comments

---

## Common Themes Across Sources

- **Tone matters more than process.** Reviews fail when feedback feels personal. Developers become defensive and stop listening.
- **Speed beats perfection.** A 24-hour review teaches more than a perfect review a week later. Momentum matters.
- **Be specific.** "Too complex" creates defensiveness. "Extract this logic into a helper" creates agreement.
- **Culture beats tooling.** Teams struggle from lack of psychological safety, not templates. Consistency prevents endless debates.

---

## References

1. [Code Review: Do's and Don'ts for Developers and Reviewers](https://www.michaelagreiler.com/code-review-best-practices-and-when-to-avoid-code-reviews/) by Michaela Greiler
   - Personal experience from leading code review culture changes at large tech companies

2. [Code Review in the Era of Continuous Integration](https://engineeringblog.yelp.com/2017/11/code-review-in-the-era-of-continuous-integration.html) by Yelp Engineering
   - Practitioner insights from scaling code reviews at a fast-growing company

3. [OWASP Code Review Guide](https://www.owasp.org/index.php/Code_Review_Guide) by OWASP Foundation
   - Evidence-based guide on code review effectiveness and psychological safety

4. [Peer Code Review: Lessons Learned at Scale](https://engineering.meta.com/) by Meta Engineering
   - Real experiences scaling code review practices across thousands of engineers

5. [The Morning Paper: Code Review Research](https://www.adriancolyer.org/) by Adrian Colyer
   - Synthesis of peer-reviewed research on code review effectiveness and impact
