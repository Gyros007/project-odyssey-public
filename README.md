# project-odyssey-public

**This repository serves as a workspace to showcase the development progress, architecture, and features of my PRIVATE repository 'Project Odyssey', covering the entire lifecycle from planning and implementation to testing and deployment. **

Independently developing a cross-platform application designed for Web, Android, and iOS, leveraging Firebase and Google Cloud Platform (GCP) for robust functionality, authentication, data analytics, machine learning, and DevOps. Built with Ionic to ensure a seamless and mobile-friendly user experience across all platforms.

Project Odyssey focuses on trip creation, allowing users to build trips either using AI with the help of Gemini through Firebase Genkit or manually with ReactFlow, connecting places in a structured and intuitive way.

# 🔧 Tech Stack
<p align="left">
  <a href="https://reactjs.org/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/>
  </a>
  <a href="https://nextjs.org/" target="_blank" rel="noreferrer">
    <img src="https://cdn.brandfetch.io/id2alue-rx/theme/dark/idqNI71Hra.svg?c=1dxbfHSJFAPEGdCLU4o5B" alt="nextjs" width="40" height="40"/>
  </a>
  <a href="https://ionicframework.com" target="_blank" rel="noreferrer">
    <img src="https://upload.wikimedia.org/wikipedia/commons/d/d1/Ionic_Logo.svg" alt="ionic" width="40" height="40"/>
  </a>
  <a href="https://firebase.google.com/" target="_blank" rel="noreferrer">
    <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/>
  </a>
  <a href="https://cloud.google.com" target="_blank" rel="noreferrer">
    <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/>
  </a>
</p>

# Images

![Screenshot 2025-03-06 022756](https://github.com/user-attachments/assets/e2337dcf-b93d-4b88-a0ca-d3c6a6efc35e)
![Screenshot 2025-03-06 022430](https://github.com/user-attachments/assets/ec6cca91-3839-4a00-84c5-b4ec169fe163)

## Update 1: Migration from Firestore to Firebase Data Connect

This project is currently undergoing a migration from Google Cloud Firestore to Firebase Data Connect. This decision was driven by several factors:

*   **Data Connect is now Generally Available:** With Firebase Data Connect recently exiting its public preview on April 9, 2025, it's become a production-ready solution.
*   **Query Flexibility:** Firestore's query limitations were becoming a significant constraint. Data Connect, leveraging PostgreSQL, offers much greater flexibility in querying and manipulating data.
*   **Simplified Data Management:** Maintaining denormalized data in Firestore was increasingly complex and time-consuming. Data Connect's relational structure promises to simplify data management and reduce redundancy.
*   **Future-Proofing with Industry Standards:** While Firestore is a proprietary NoSQL database, Data Connect is built on open standards like PostgreSQL and GraphQL. This significantly lowers the barrier to migrating to other database providers in the future if needed.
*   **Vendor Lock-in Mitigation:** Although Firebase Data Connect's GraphQL implementation includes custom directives from the Firebase team, the underlying data structure remains PostgreSQL. This means that even with Firebase's abstractions, a future migration *away* from Data Connect is still a viable option, unlike the complete vendor lock-in that comes with Firestore's NoSQL structure.

By embracing Data Connect, this project aims to benefit from increased query power, simplified data maintenance, and the assurance of greater portability in the long run.
