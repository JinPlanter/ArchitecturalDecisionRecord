Table of Contents:
* [Architectural Decision Record (ADR)](#architectural-decision-record-adr)
  * [Data Storage](#data-storage)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

# Architectural Decision Record (ADR)
## Data Storage

### Context

- We are tasked with creating a mobile application for a retail company, aimed at providing a variety of features to the customers. This application is expected to include features such as product browsing, order history, loyalty programs, and offline functionality. One important decision is how to manage and store data efficiently and securely.

### Decision

- We have decided to use a combination of local device storage and cloud-based storage for managing app data.

<br/>

### Rationale

- Offline Mode: To support the retail company's requirement for offline mode, local device storage is essential. It allows users to access their order history and other relevant data even when they are not connected to the internet.

- Real-time Updates: Cloud-based storage is necessary for real-time updates, including product availability, order status, and loyalty program points. Cloud storage ensures that users always have access to the latest information.

- Scalability: Cloud-based storage provides scalability to handle large amounts of data and user interactions, accommodating potential future growth of the app.

- Data Security: Sensitive data, such as payment information and user profiles, will be securely stored in the cloud, implementing industry-standard security measures and encryption.

- Data Synchronization: A synchronization mechanism will be implemented to ensure data consistency between the local storage and the cloud. This mechanism will sync data when the app is online, adhering to the requirement for data syncing.

<br/>

### Consequences

- Development Complexity: Managing both local and cloud storage introduces complexity into the development process, requiring us to learn how to implement synchronization and error handling.

- Data Sync Logic: Implementing data synchronization logic can be challenging, as it needs to handle conflicts, errors, and network fluctuations gracefully.

- Data Privacy and Compliance: Storing user data in the cloud requires strict adherence to data privacy regulations and compliance standards which we will have to research further into.

Considering the need to support offline mode, real-time updates, scalability, and data security, a combination of local device storage and cloud-based storage is the appropriate decision for this retail app. It allows us to provide a seamless user experience while ensuring data availability and security.

Despite the various difficulties in implementing both local and cloud-based storage, we feel that using both is a requirement in order to meet our clients requirements for this application.
