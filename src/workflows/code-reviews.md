# Code Reviews Guide

Code reviews are critical for producing high-quality, maintainable code, especially in large-scale or collaborative projects. Adopting consistent coding standards—like those in Google's style guides—ensures uniformity across teams and makes code easier to understand. This section introduces key code review strategies and highlights the role of pull request reviews in modern development workflows.

## Google style guides
Every major open-source project includes a style guide, which is a set of norms for writing code for that project. When all the code in a huge codebase is written in the same manner, it is considerably simpler to understand.
You can find the project and style guide for Google code [here](https://google.github.io/styleguide/).

## Code review
Code review, also referred to as peer code review, is the deliberate and methodical gathering of other programmers to examine each other's code for errors. Code review can speed up and simplify the software development process, unlike other techniques. Peer reviews also save time and money, especially by catching the kinds of defects that could sneak through testing, production, and into the laptops of end users.

### Common code review strategies
- **Pair programming**: Engineers work side-by-side on the same code. Useful for mentoring, but less objective and more resource-intensive.
- **The email thread**: Code is sent via email for review. Flexible but can lead to disorganized feedback.
- **Over the shoulder**: A developer walks a peer through their code directly. Informal and effective for quick feedback.
- **Tool assisted**: Using browser- or IDE-integrated tools to asynchronously review and track code feedback, enabling efficient, non-local review processes.

## Pull request reviews
A pull request (PR) is a way to review new code before merging it into a main branch on GitHub. Contributors can comment on, approve, or request changes to proposed updates. Repository admins can require approval before merging.
Anyone with read access can review and suggest inline changes. Learn more about reviewing PRs [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews).

### Five tips for pull request reviews
1.	**Be selective with reviewers**: Add only a reasonable number of reviewers to avoid inefficiency.
2.	**Timely reviews**: Ideally complete within two hours to reduce context switching and delays.
3.	**Constructive feedback**: Feedback should be specific, helpful, and respectful.
4.	**Detailed pull request description**: Include a comprehensive summary of changes, usage, design, and additional reviewer notes.
5.	**Interactive rebasings**: Keep commit history clean by editing commits before merge.

> **Key takeaways**
>
> - Consistent coding standards improve readability and maintenance.
> - Code reviews catch defects early and improve quality through collaboration.
> - Review strategies should match project context—pair programming, async tools, email, or over-the-shoulder.
> - Pull request reviews enable structured collaboration and code validation before merging.
