Table of Contents:
* [Architectural Decision Record (ADR)](#architectural-decision-record-adr)
  * [UI Framework Selection](#ui-framework-selection)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

# Architectural Decision Record (ADR)
## UI Framework Selection

### Context:

- We are tasked with creating a mobile application for a retail company, aimed at providing a variety of features to the customers. This application is expected to include features such as product browsing, order history, loyalty programs, and offline functionality. One of our choices is determining what UI Framework we will use for our application.

<br/>

### Decision:

- We have chosen to employ React Native as the cross-platform UI framework for developing the mobile application.

<br/>

### Rationale:

- Cross-Platform Compatibility: React Native is a reputable cross-platform framework that facilitates the creation of a single codebase, allowing the application to run on both iOS and Android platforms. This approach minimizes development effort, enhances code maintainability, and guarantees a uniform user experience across devices.

- JavaScript Expertise: As we already have experience with JavaScript, utilizing React Native gives us a solid foundation of knowledge to work off of.

- Access to Native Modules: React Native provides access to a broad array of native modules and components. This should potentially allow us to use platform specific features if we have need for them.

- Performance: React Native is designed to optimize application performance, offering a user experience comparable to native apps. It accomplishes this through components that bridge between JavaScript and native code, resulting in fast and responsive applications.

- Active Community and Ecosystem: React Native boasts a thriving community of developers, which gives us a rich ecosystem of libraries, plugins, and third-party tools. This community support can potentially accelerate development, simplify problem-solving, and offer a plethora of resources for our project.

<br/>

### Consequences:

- Platform-Specific Features: Although React Native allows for the integration of platform-specific features, some advanced or intricate features may require additional development effort.

- App Size: The app's binary size may be larger compared to fully native apps, primarily due to the inclusion of the React Native runtime and bridge.

Despite these few disadvantages, we believe that with our understanding and skills, React Native is the best and pragmatic choice for our Framework.
