# Login and Auth

## Review, Research, and Discussion

- Why is the Context API useful?

  Because it can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props.

- Can a component outside of a provider get its context?

  No, it needs to be wrapped by the provider Tags.

- What are some common use cases for using the Context API?

  Useful for sharing data that can be considered global, such as currently authenticated user, or theme settings for the application.

- Describe “Context Hell”

  Context API has virtually no boilerplate in comparison to Redux, adding Context Providers makes for messy and unreadable code.

## Document the following Vocabulary Terms

- **global state** is keeping a state at the top level of an application and providing access methods to all child levels without the need to pass props. Global state should only keep states that concern the entire app, such as theme, language, or other app-wide settings.

- **global context** provides a way to share values and data between components without having to explicity pass a prop through every level of the tree. Designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- **provider** accepts a value that will be passed to its children. All children components will re-render when the value changes.

- **consumer** is component that subscribes to context changes in value of the Provider.

## Preparation Materials

### What is role based access control?

  Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

  Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.

  As a result, lower-level employees usually do not have access to sensitive data if they do not need it to fulfill their responsibilities. This is especially helpful if you have many employees and use third-parties and contractors that make it difficult to closely monitor network access. Using RBAC will help in securing your company’s sensitive data and important applications.

  **BENEFITS OF RBAC**

  Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization. Other advantages include:

  1- **Reducing administrative work and IT support**. With RBAC, you can reduce the need for paperwork and password changes when an employee is hired or changes their role. Instead, you can use RBAC to add and switch roles quickly and implement them globally across operating systems, platforms and applications. It also reduces the potential for error when assigning user permissions. This reduction in time spent on administrative tasks is just one of several economic benefits of RBAC. RBAC also helps to more easily integrate third-party users into your network by giving them pre-defined roles.

  2- **Maximizing operational efficiency**. RBAC offers a streamlined approach that is logical in definition. Instead of trying to administer lower-level access control, all the roles can be aligned with the organizational structure of the business and users can do their jobs more efficiently and autonomously.

  3- **Improving compliance**. All organizations are subject to federal, state and local regulations. With an RBAC system in place, companies can more easily meet statutory and regulatory requirements for privacy and confidentiality as IT departments and executives have the ability to manage how data is being accessed and used. This is especially significant for health care and financial institutions, which manage lots of sensitive data such as PHI and PCI data.

### React Cookies

- “Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them”.

- To set or remove the cookies, we are using a third-party dependency of react-cookie

- Install : npm i react-cookies

- “To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie”.
