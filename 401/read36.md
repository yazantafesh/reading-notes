# Application State with Redux

## Review, Research, and Discussion

- What are the advantages of storing tokens in “Cookies” vs “Local Storage”

  Cookies are automatically saved, sent and removed by the browser. When doing browser level navigation, only cookies are sent. Sharing the same session across subdomains can easily be done with cookies. Cookies have a special flag called httpOnly, which means that malicious JS code cannot send the access token to the attacker.

- Explain 3rd party cookies.

  **Third party cookies** are cookies that are stored under a different domain than you are currently visiting. They are mostly used to track users between websites and display more relevant ads between websites. Another good example is a support chat functionality provided by a 3rd party service.

- How do pixel tags work?

  Tracking pixel or pixel tag (also called 1x1 pixel) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. The website operator or sender of an email adds the tracking pixel using a code in the website’s HTML code or email. This code contains an external link to the pixel server. If a user visits the destination website, the HTML code is processed by the client – usually the user’s browser. The browser follows the link and opens the (invisible) graphic. This is registered and noted in the server’s log files. In addition, various information about the user is also transmitted using this method. To some extent, combination with JavaScript is necessary in order to collect information about the operating system or browser type. The following data can be acquired and analyzed with a tracking pixel: operating system used, type of website or email used (mobile or desktop), type of client used (browser or mail program), client's screen resolution, time the email was read or website was visited, activites on the website during the session (when using multiple tracking pixels), IP address.

## Document the following Vocabulary Terms

- **cookies** are small blocks of data created by a web server while a user is browsing a website and placed on the user's computer or other device by the user’s web browser. Cookies are placed on the device used to access a website, and more than one cookie may be placed on a user’s device during a session.

- **authorization** is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular.

- **access control** is the selective restriction of access to a place or other resource, while access management describes the process. The act of accessing may mean consuming, entering, or using. Permission to access a resource is called authorization.

- **conditional rendering** is a term to describe the ability to render different user interface (UI) markup if a condition is true or false.

## Preparation Materials

### Redux

  **Redux** is an open-source JavaScript library for managing application state. It is most commonly used with libraries such as React or Angular for building user interfaces. Similar to (and inspired by) Facebook's Flux architecture, it was created by Dan Abramov and Andrew Clark.

  **Why Should I Use Redux?**

  Redux helps you manage "global" state - state that is needed across many parts of your application.

  The patterns and tools provided by Redux make it easier to understand when, where, why, and how the state in your application is being updated, and how your application logic will behave when those changes occur. Redux guides you towards writing code that is predictable and testable, which helps give you confidence that your application will work as expected.

  **When Should I Use Redux?**

  Redux helps you deal with shared state management, but like any tool, it has tradeoffs. There are more concepts to learn, and more code to write. It also adds some indirection to your code, and asks you to follow certain restrictions. It's a trade-off between short term and long term productivity.

  Redux is more useful when:

- You have large amounts of application state that are needed in many places in the app
- The app state is updated frequently over time
- The logic to update that state may be complex
- The app has a medium or large-sized codebase, and might be worked on by many people.

  