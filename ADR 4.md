# ADR 4: Permissions

## Title: Permissions for Native Mobile App

**Status:** Proposed

**Context:**
Our Native mobile app offers a wide range of features, including offline browsing, push notifications, and integration with various payment gateways. To ensure these functions work seamlessly, the app requires access to specific resources on the user's device, such as internet network status, notification settings, payment information, and more. However, it's crucial to manage permissions effectively and transparently, ensuring that user privacy is respected and excessive information isn't collected, as this can erode trust and lead to legal consequences. On the other hand, insufficient permissions can hinder the app's usability.

**Decision: Permissions Model**

We are building an app for a retail company with a multitude of features. To enable these features, the app will adopt a permissions model where users are asked for permissions before or during the app installation or usage. For example, we will request permission to use storage so users can view products even when offline. We will also ask for permission to send notifications about new items or order status. The app will require internet access to update data and facilitate shopping. Additionally, we may request location permission to show nearby stores but will always provide clear explanations for why we're requesting specific permissions and only ask for what is genuinely necessary. By following this approach, we aim to earn the trust of our users and provide them with an enjoyable experience.

**Consequences:**

**Positive Consequences:**

1. **User Experience & Trust:** By requesting only essential permissions and transparently explaining the reasons for these requests, users will trust us more and enjoy the app's features, including offline browsing, timely updates, push notifications about exclusive offers, and secure payment gateways.

2. **Safety from Fraud:** Requesting specific permissions ensures that users are not exposed to unnecessary risks. We are taking steps to protect their data from misuse, making the app fun, safe, and trustworthy for everyone.

**Negative Consequences:**

1. **Permission Denials:** Not all users may be comfortable granting certain permissions. For example, some users might decline location permissions due to privacy concerns, resulting in the loss of location-related features. Similarly, if users deny storage permissions, their offline browsing experience may be compromised.

2. **Balance Between App and Users:** As the app evolves with new features, the permissions it requires may change. For example, if we introduce a customer service support feature in the future, we'll need to request additional permissions. This can be a sensitive task for users, and we must ensure that we only ask for permissions that are absolutely essential and communicate the benefits clearly to maintain their trust.

