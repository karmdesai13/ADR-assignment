# ADR 5: Data Storage

## Title: Selection of Data Storage for Retail Mobile App

**Status:** Proposed

**Context:**
The retail company is developing a mobile app with features like offline browsing, order tracking, push notifications, payment processing, user behavior insights, and image handling. A robust data storage system is vital to support these functionalities. The system should be accessible to users even when offline, scale with the company's growth, and adhere to global data protection standards, especially considering international expansion plans.

**Decision:**

**Local Storage:** For offline support, essential data like recently viewed products and a brief order history will be stored locally on the user's device. This ensures users can access critical functionalities even without an internet connection. Storing data locally enhances user satisfaction and attracts new users in the future.

**Cloud Storage:** Less critical data, including information about products, categories, images, and other non-essential data, will be stored in Google Cloud Storage. Google Cloud Storage enables easy data synchronization and updates to their database.

**Database:** User information such as customer names, email addresses, phone numbers, and transaction records will be stored in a PL/SQL database. This choice is ideal for business applications and data storage. The database will sync with local storage when the user's device connects to the internet, ensuring that all data remains up-to-date.

**Consequences:**

**Positive Consequences:**

1. **Seamless User Experience:** Storing essential data locally allows users to browse products and view their order history offline, ensuring a reliable app experience at all times.

2. **Scalability:** Combining cloud storage and a scalable database enables the app to handle increasing numbers of products and users without compromising performance.

**Negative Consequences:**

1. **Data Syncing:** Regular syncing between local and cloud storage is essential, and any issues in this process could lead to data discrepancies.

2. **Security Concerns:** Storing data, especially user transaction details, introduces security concerns. Investment in high-quality security measures will be necessary to ensure data accuracy and maintain user trust.
