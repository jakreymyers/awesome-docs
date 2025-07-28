# Writing Guide: API Getting Started

>This writing guide provides extra tips describing how to fill in each of the sections within [Template: Getting Started with the {Product} API](./template_api-getting-started.md).

## Introduction

A getting started guide is a document that walks the user through how to create a minimum working example with your API. You can also think of a getting started guide as a "Hello World" tutorial that includes a complete series of steps or actions that show the user how to use your API.

|   | Getting started guide | Tutorial guide |
| :---- | :---- | :---- |
| Target audience | Domain experts who know the problem space and want a quick setup or overview of your product | Beginners who are new to the problem space and require in-depth and comprehensive guidance |
| Content | Basic steps and essential information | In-depth analysis and broader explanation of concepts |
| Purpose | Help users get started  | Provide a comprehensive understanding of the problem space or product |
| Scope | Immediate actions | Immediate actions and comprehensive explanations |

## Why do I need an API getting started guide?

API getting started guides are helpful for the following reasons:

* **Faster integration**: Getting started guides provide the user with a streamlined path to get started with an API without having to read through lengthy documentation to understand key steps to interact with your API, such as setting up an account, getting API keys and authenticating requests for specific endpoints, etc. They typically offer step-by-step instructions, code samples, and ready-to-use templates that help users quickly understand the API's core concepts and functionalities. By following the guide, users can accelerate the integration process and start using the API in their applications faster.

* **Reduced learning curve**: APIs can have complex documentation with various endpoints, parameters, authentication methods, and data formats. Getting started guides distill this information into a concise and simplified format, focusing on the most common and essential use cases.

* **Practical examples**: Getting started guides often include code snippets or sample projects that demonstrate how to interact with the API in real-world scenarios. These examples help users understand the API's capabilities and see how they can integrate it into their own applications. By showcasing practical use cases, the guides provide inspiration and guidance for users to start building with the API quickly.

* **Intended use**: API getting started guides allow for the correct and intended use of the API. Getting started guides also help prevent errors, increase efficiency, and streamline performance.

## Best practices

1. The key goal of a getting started guide is to achieve a basic core working function of the product or feature. Focus on getting users to success quickly by keeping content short and focused on the most important aspects of the API.

2. Provide a common use case with sample code that demonstrates real-world usage. Number the steps clearly and use descriptive headings for different procedures. Start headings with action verbs like "Make your first request" or "Choose an endpoint for your request" to create clear, task-oriented guidance.

3. Include examples of sample return data so users can verify they successfully completed each task. Each step should contain only one action to avoid confusion and ensure users can complete tasks systematically.

4. Error handling deserves special attention in getting started guides. Include guidance on common error scenarios and provide examples of typical error messages users might encounter. This prevents frustration when things don't work as expected.

5. Link to additional resources throughout the guide so users can learn more about specific API features without overwhelming the getting started experience.

## Content of the API getting started template

### About the "Introduction" section

In this section, give a brief introduction or explanation of the API and define the intended audience the guide targets. You should also describe what the user accomplishes or learns by using the getting started guide. For example, to integrate the API into their own app, to build an app with the API or to test the API.

### About the "Prerequisites" section

In this section, include all the necessary tools or information the user needs to accomplish the objectives of the getting started guide. Examples include:

* List of hardware requirements.
* List of any software dependencies.
* How to download (provide the web address), install, and configure the API.
* If your API requires detailed software setup instructions for dependencies, refer the user to the Getting Started Guide or Setup Guide for the API.
* How to get the required access keys or authentication credentials, if required.
* If your API requires detailed authentication information, refer the user to that document.

### About the "Authentication" section

This section is optional since not all APIs require authentication to use. Use this section to explain the requirement to get access to the API, which may include signing up for the API, setting up authentication, following the steps to get API keys or access tokens.

### About the "Base URL" section

The base URL is the root address of the API, which all API endpoints will be appended to. Provide a base URL at the top of the document to ensure all relative links are consistently referenced, and to simplify the process of updating URLs if the domain or root address changes.

### About the "Make your first API request" section

In this section, guide users through making their first CRUD request to the API. Provide clear, step-by-step instructions along with example API responses to help them understand the process.

To improve usability, consider the following:

* Code samples: Provide code snippets in relevant programming languages the user can run. The template contains placeholders for your code snippets.
* Comments and explanations: Include in-line comments within the code or provide supporting explanations after each snippet.
* "Hello, World" example: Create a "Hello, World" example that shows how to use at least one of the API endpoints.
* Common error messages: Highlight potential errors users might encounter, along with troubleshooting tips.
* Provide annotated screenshots with arrows, boxes, etc. Bear in mind that screenshots may be difficult to translate so ensure you use them only when relevant.

### About the "Next steps" section

In this section, refer the user to other documentation and features available in the API that can help improve the user's understanding and usage of your product. Provide links to:

* Additional tutorials or articles about the API.
* The API glossary or any additional core concepts.
* Relevant resources, like blogs, troubleshooting guides, reference documents, videos, and how-tos.

---
