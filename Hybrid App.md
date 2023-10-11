Table of Contents:
* [Architectural Decision Record (ADR)](#architectural-decision-record-adr)
  * [Hybrid App](#hybrid-app)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

# Architectural Decision Record (ADR)
## Hybrid App

### Context:

- We are tasked with creating a mobile application for a retail company, aimed at providing a variety of features to the customers. This application is expected to include features such as product browsing, order history, loyalty programs, and offline functionality. One of our key architectural decisions is choosing whether the mobile application should be a native, web, or hybrid app.

<br/>

### Decision:

- We have opted to develop a hybrid mobile app instead of a native or web-based one.

<br/>

### Rationale:

- Simplicity: By design, starting with a hybrid app allows us to work with a single codebase that is deployable on both iOS and Android. This simplifies our development and ensures code reusability, as well as ensuring a consistent user experience no matter the device they are on.

- Cost-Efficiency: By deciding on a hybrid app, we can potentially save some costs in having to learn native specific languages or apps. This could be beneficial where budget constraints are concerned, and lets us focus on making sure our features work.

- Web Technologies: Hybrid apps let us use various languages such as HTML, CSS and Javascript. For our team who already have some firsthand experience with these, this vastly reduces our learning curve and allows us to get a head start, as opposed to having to learn brand new languages for our app.

- Rapid Iteration: Hybrid apps benefit from faster development cycles and updates due to their shared codebase. This not only allows us to work on updates quicker, but also ensures that our updates are consistent cross-platform.

<br/>

 ### Consequences:

- Performance: While we do not consider it a large problem for our app, Hybrid apps in general are not as efficient as native apps when it comes to performance.

- Platform-Specific Features: If we need to add or work around platform specific features, this will require additional development and knowledge from our team, increasing the time required to create this app.

- App Size: The app's binary size may be larger compared to fully native apps due to the inclusion of the hybrid framework.

Because of the advantages in starting with a hybrid app, We feel that this decision is worth any potential consequences, and therefore seems to be the most optimal choice moving forward.
