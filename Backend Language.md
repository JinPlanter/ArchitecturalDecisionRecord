Table of Contents:
* [Architectural Decision Record (ADR)](#architectural-decision-record-adr)
  * [Backend Language](#backend-language)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

# Architectural Decision Record (ADR)
## Backend Language

### Context

- We are tasked with creating a mobile application for a retail company, aimed at providing a variety of features to the customers. This application is expected to include features such as product browsing, order history, loyalty programs, and offline functionality. One critical decision is choosing the appropriate backend programming language for the app's server-side development.

<br/>

### Decision

- We have decided to use Node.js as the backend programming language for the retail app.

<br/>

### Rationale

- JavaScript Expertise: Node.js is based on JavaScript, a language familiar to many developers. As with our decision with React Native, our knowledge with Javascript gives us a solid base to work off of, and speeds up our initial stages of development.

- Non-blocking I/O: Node.js is known for its non-blocking I/O model, which is well-suited for handling a large number of concurrent connections and real-time features such as push notifications and live updates. Given the nature of our app, push notifications and being able to handle a large number of customers shopping at the same time is important.

- Vibrant Ecosystem: Node.js has a vibrant ecosystem with a vast collection of open-source libraries and packages available through npm (Node Package Manager). This allows us to leverage existing solutions for common tasks and integrate third-party services effectively.

- Scalability: Node.js's scalability and performance have been proven in various high-traffic applications, making it suitable for accommodating the growth of this app.

<br/>

### Consequences

- Single-Threaded: Node.js uses a single-threaded event loop, which means long-running tasks can block the event loop and affect responsiveness. We will have to employ careful coding and possibly the use of worker threads in order to mitigate this if it becomes a problem.

- Dependency Management: Managing dependencies via npm is convenient but may introduce versioning conflicts if not carefully managed.

Considering the need for real-time features, a vibrant ecosystem, and the potential for scalability, Node.js is a suitable choice for the backend language for this retail app. It aligns well with the project's goals and requirements.
