# Best Practices: README

>Before using [Template: README](./template_readme.md), read this for best practices about how to research, write, and maintain this type of content.

## How to plan and research your project's README file

The README file is the first file that displays in the main folder of a project's repository, making it the first file users encounter. Whether it's for an open-source project or commercial project, users should be able to read your README file to:

* **Identify the project:** Readers should be able to figure out your project's name and find key information like a link to the project's website and the owner of the project (either the business, organization, or author).
* **Evaluate the project:** Readers should be able to explain what the project does, its core function, and what problem it solves. They should also be able to identify the project's terms of use without legal jargon.
* **Use the project:** Readers should be able to install and run the program for the first time. After installation, they should have an idea on how to test the program to see if it's working correctly and to get a sense of how to use it for its core purpose. For example, it might provide a simple "hello world" experience to try the project's core functionality.
* **Engage with the project:** Some readers need to know how to engage with the project (either as a contributor or to submit bug reports or feature requests as a user). They need to know how to contact the project owners, interact with the community or how to propose their ideas.

While working on these goals, consider using the following strategies as you plan and do research your project's README file:

* **Identifying details for the project:** Including the project's official name, its website (if applicable), and the project owners.
* **The core purpose of the project:** You should come up with a simple, straightforward description of the project that's written in clear, plain language.
* **How to install and run the program for the first time:** Try running a fresh install of the program and recording every step you need in order to prepare your environment and get the application running. Note any dependencies you need to install and how you can verify that the installation was successful. If the install process is overly complex and difficult to describe, consider opening up an issue against the project to simplify the process.
* **Design a "hello world" experience for the program:** A "hello world" experience is a small piece of code that you can run to get a simple demonstration of the basic usage of the software. If there isn't a simple "hello world" experience, consider opening up an issue to create this program for your software.
* **Determine how you want others to contribute to the project:** Spend some time thinking about how you want people to interact with your project. If your project is open source, do you want people to join a community forum, open issues, or attend user group meetings? If your project is commercial or closed source, think about how you would onboard a teammate and what steps they would have to take in order to get access to the repository and begin contributing.

## How to write the README

Now that you have gathered information, it's time to start writing the README file. The following list includes some strategies for writing effective README content:

* Consider explaining why users want to interact with your project, in addition to what it can do. Doing this creates a more compelling story about your project that not only piques their interest but also motivates them to explore and further engage with your project.
* Describe the problems that your project solves and how users who are facing them can benefit from using your project. Think of it as an advertisement on TV or a YouTube video. This creates a stronger connection with your project's audience.
* Provide hyperlinks to the technology that's used to build your project. This can help users gain a better understanding of how they can contribute to it.
* Use screenshots that convey the steps of using your project and clickable code snippets. This can save time and effort in writing the installation process.
* Explain and provide hyperlinks to the places where users/contributors can share their feedback on the project. This would make it easier for users to directly report issues.
* Mention and provide a few examples of contributions that you encourage (design, documentation, and code). This not only gives users an idea on how to contribute to the project but also reassures them that your project embraces many ways to contribute, which in turn brings a diverse audience.

## How to maintain a README file

A README file is one of your project's founding documents. So, your README file grows and matures along with your project. When your project first starts out, it might be a simple stub or placeholder document. As your project builds momentum and attracts users or additional contributors, your README adapts to those changes.

At first, your README file usually doesn't contain much information because your project is new. However, it should contain at least these core items:

* Project name and project owners
* The goal or core purpose of the project
* A list of dependencies and the current steps to install and run the program
* Terms of use (license)

As your project grows and becomes more complex, update its README file to correspond with these changes. However, maintaining the accuracy and relevance of a README file over time can be difficult.

When your README starts to be long or overly complex, that's a signal that it's time to move some of the information out of the README and into other important documents:

| Document | Information |
| :---- | :---- |
| CONTRIBUTING | Create a CONTRIBUTING guide to tell users how they can contribute to your open source project and join the community. |
| Troubleshooting | As your project expands, its users may encounter recurring issues. As that content gets more lengthy over time, you could move it to a troubleshooting guide |
| Our Team | Create a list of your project's core maintainers to communicate who belongs to your open source project or organization and how contributors can contact or work with them. |

Breaking your README out into other documents helps maintain a clear and concise README while providing necessary guidance for potential contributors. This separation fosters a consistent and welcoming environment for the community. Remember to interlink between your README file and these additional documents.

### Additional maintenance strategies

Maintaining your README over time requires ongoing attention, but several strategies can make this process more manageable and effective.

The most efficient approach is to update your README alongside code changes. When dependencies or installation processes change, include README updates in the same pull request or merge request. This prevents documentation from becoming outdated and ensures changes are captured while fresh in developers' minds.

As your project grows, your README may become lengthy and harder to navigate. Adding a table of contents improves organization and helps readers find specific information quickly. Many projects benefit from restructuring content into logical sections that follow users' typical workflows.

Build README review into your release process by including it as a checklist item. This ensures content accuracy and freshness with each release, preventing the accumulation of outdated information that can frustrate users.

For larger projects, plan a maintenance roadmap using your project's issue tracker (GitHub, GitLab, Jira). Create dedicated tasks and categorize them with labels like "Planned," "In Progress," and "Reviewed" to organize and prioritize updates. Teams can assign members to planned tasks to ensure consistent progress.

Automation can significantly reduce maintenance burden. Implement CI/CD pipelines (GitHub Actions) to automatically update information like project dependencies. Use linters like markdownlint and Vale to check and fix formatting and styling issues automatically, saving time and effort for your team.

Open source projects can leverage community involvement in maintenance. Encourage users to share suggestions for improving README clarity, content, or organization through your issue tracker. Consider inviting first-time users or contributors to create friction logs documenting places where they became confused or struggled during installation. These logs, submitted as bug reports or issues, not only reduce your maintenance burden but foster collaboration and make the README more comprehensive and user-friendly.
