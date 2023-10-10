# ADR 3: Backend Language

## Title: Choice of Backend Language

**Status:** Proposed

**Context:**
The development team faces the decision of selecting a backend language for the retail company's app, which needs to support features like browsing and purchasing products, push notifications, and order tracking. After considering the app's requirements, the team has chosen Node.js as the backend language.

**Decision: Node.js as Backend Language**

After assessing the app's requirements, the team has decided to proceed with Node.js as the backend language. The reasons for choosing Node.js are as follows:

**Real-time Notifications:** Node.js is well-suited for pushing real-time notifications. This capability will be valuable for sending order tracking updates, daily deal notifications, and other real-time notifications to users.

**Non-blocking I/O:** Node.js offers non-blocking I/O, a critical feature for supporting a multi-user platform with various activities such as product searching, ordering, and data and image loading. Non-blocking I/O ensures that user interactions do not get blocked, enhancing the app's responsiveness.

**Consequences:**

**Positive Consequences:**

1. **Scalability:** Node.js can easily accommodate an increase in traffic and users in the future. It is well-suited for handling growing activities and user numbers.

2. **JavaScript Ecosystem:** Node.js integrates seamlessly with the JavaScript ecosystem, making it a natural fit when using React Native as the framework. This integration simplifies development and maintenance.

**Negative Consequences:**

1. **Error Handling:** Node.js may sometimes crash if errors occur and aren't handled in a controlled manner. Ensuring robust error handling and exception management is crucial to prevent unexpected crashes.

2. **Learning Challenges:** Some developers may not be familiar with Node.js or may not have worked with all of its functions or packages, which could result in a learning curve for the development team.
