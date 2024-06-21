# differences between monorepo and multirepo

# Multirepo (Multiple Repositories)
Structure:

Each project or component has its own independent repository.
Example: One repository for the frontend, one for the backend, one for the database, etc.
Advantages:

Isolation: Changes in one repository do not directly affect others, making it easier to isolate problems.
Permissions: It is easier to manage specific access permissions for each repository.
History: The change history is clearer and more specific to each project.
Disadvantages:

Coordination: It can be difficult to coordinate changes between multiple repositories, especially if there are strong dependencies between them.
Maintenance: Managing multiple repositories can be tedious and require more effort in terms of configuration and administration.
Dependencies: Dependencies between projects can be difficult to manage and version correctly.

# Monorepo (Monolithic Repository)
Structure:

All projects or components are stored in a single shared repository.
Example: The frontend, backend, and other components reside in different directories within the same repository.
Advantages:

Synchronization: It's easier to make synchronized changes across multiple projects, since they're all in the same repository.
Consistency: Shared tools and libraries can be managed more consistently.
Visibility: Developers have full visibility into all code, making it easier to understand and collaborate across teams.
Disadvantages:

Scalability: As the repository grows, it can become slow and unwieldy.
Conflicts: The high amount of changes can increase the likelihood of code conflicts.
Permissions: Managing permissions can be more complex, since everyone has access to the entire repository.

# Real World Examples
Multirepo: Used by companies that prefer more separation between their components and projects, such as many organizations that follow the microservices approach.
Monorepo: Used by large technology companies such as Google, Facebook, and Microsoft, who have advanced infrastructure and tools to manage large amounts of code in a single repository.

# Decision
The choice between multirepo and monorepo depends on several factors, including:

Team size: Large teams with many dependencies may prefer a monorepo.
Infrastructure: The availability of tools and infrastructure to manage a large monorepo.
Development strategy: The architecture of the software and how dependencies and release cycles are managed.

# What are http methods (Put, Post, Pat)

Also known as HTTP verbs, they are instructions that indicate the action you want to perform on a specific resource on a web server. They are essential for communication between a client and a web server.

Common HTTP methods include GET, POST, PUT, and DELETE.
## GET: Retrieves data from a resource.
## POST: Sends data to the server for processing or storage.
## PUT: Updates an existing resource.
## DELETE: Deletes a resource.

# Additional HTTP methods:

• PATCH: Similar to PUT, but updates only a specific part of a resource
• HEAD: Similar to GET, but only retrieves the response headers, not the resource body.
• OPTIONS: Gets the HTTP request options available for a specific resource.

# NODE VERSION WE WILL USE

• We will use v20.14.0 for this project since it is the version with long-term support (lts) at the moment

# Are we going to use multirepo or monorepo?

In this case we are going to use multirepo since we have seen that changes in one repository do not directly affect others, which makes it easier to isolate problems and it is easier to manage specific access permissions for each repository.

# Problems, objectives and/or services of the project or residential units?
to see the scope of the project
Requirements from users or apartment owners or people living in the unit
- it is necessary to have a user account for each apartment
- they can request reservations for common areas
- they can send photos and/or emails with problems of damage or situations in the complex
- a link for payment of the administration bill

Requirements from the administration
- admin user
- to be able to make publications and/or notices
- to be able to send letters to certified emails of users for notifications
- to be able to create surveys on the page on different topics
- to have a section for managing the building financially.
- to approve reservations for common areas.





# differences between npm and yarn

Both NPM and Yarn are powerful tools for JavaScript package management and the choice between them depends on your project requirements and preferences. NPM, being the default package manager for Node.js, enjoys widespread adoption and compatibility. On the other hand, Yarn offers advantages like improved performance, deterministic dependency resolution, parallel installation, and better support for workspaces and monorepos.

# Definition of nvm

Node Version Manager (NVM), as the name suggests, is a tool for managing Node versions on your device. Different projects on your device may use different versions of Node. Using only one version (the one installed by npm) for these different projects may not give you accurate execution results.

Basically it is to be able to jump from node.js version and do a quick update

(page to install nvm step by step https://4geeks.com/es/how-to/como-instalar-nvm-en-windows)

# Definition of swagger

It is an application that allows us to extract information from the API that allows us to know what we can do in each http verb.

Swagger toolkit:

It is a set of open source tools that are based on the OpenAPI specification.

It includes tools for:
- Documenting APIs: Generates complete and readable documentation for humans and machines from the API definition.
- Designing APIs: Allows developers to design APIs visually and collaboratively.
- Testing APIs: Provides tools to test APIs and ensure their correct operation.
- Generate code: Can generate source code in different programming languages from the API definition.

In short, Swagger is an essential tool for the development and consumption of REST APIs.

# definition of Eslint

ESLint is a static code analysis tool for JavaScript.

Its primary function is to identify and fix bugs, style issues, and violations of coding conventions in JavaScript development projects.

ESLint helps developers write cleaner, more consistent, and maintainable code.

It is a highly versatile tool that can be configured to fit the needs of any project or development team.
