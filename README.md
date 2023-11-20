# CorporationX
Project: Startup Platform Development <br>
I had the privilege of contributing to the development of a groundbreaking startup platform with the goal of empowering entrepreneurs and innovators in their startup journey.
Each team has its own master branch in the shared repository. There is a branch for my Cerberus-master command, which contains all the stable code for that command in a specific service.

---
#### List with my tasks:
1. Obtaining the 'Writer' achievement
    - Description: Condition for receiving the achievement: publish 100 posts.
    - [implementation](https://github.com/CorporationX/achievement_service/blob/cerberus-master/src/main/java/faang/school/achievement/service/AchievementService.java)
2. Notification of receipt of comment
    - Description: The notification_service should be designed to send a notification when another user leaves a comment under the post authored by the original post's author.
    - [implementation](https://github.com/CorporationX/notification_service/blob/cerberus-master/src/main/java/faang/school/notificationservice/listener/event/CommentEventListener.java)
3. Generating unique account numbers
    - Description: It is necessary to implement the automatic generation of unique account numbers. Additionally, introduces the capability to incorporate a pre-generated account number into the account opening process.
    - [implementation](https://github.com/CorporationX/account_service/blob/cerberus-master/src/test/java/faang/school/accountservice/service/FreeAccountNumbersServiceTest.java)
4. Exchange rate
    - Description: The payment_service could periodically interact with an external service to fetch current exchange rates and store them locally throughout the day. This way, it avoids the need to contact the external service with each payment. This functionality can be implemented using a scheduled job and by accessing the external service through its Web API.
    - [implementation](https://github.com/CorporationX/payment_service/commit/4928e0a5504f0c6d78caa1f076f6b18c5122d483#diff-3057833b57b40119fa7656e6a7bbc8bae8e595049ed39257eb027db3504402a1)
5. Writing a recommendation
     - Description: Implement the functionality for users to leave recommendations for each other, with validation for the presence of text. Allow users to make a recommendation only if they haven't provided the same user with another recommendation within the last 6 months
     - [implementation](https://github.com/CorporationX/user_service/blob/cerberus-master/src/main/java/school/faang/user_service/service/RecommendationService.java)
6. Deactivating users
     - Description: It should be possible to deactivate a user account before final deletion. When a user requests to delete their account, it is initially deactivated for three months. Prior to deactivation, all planned profile activities associated with the user must be halted
     - [implementation](https://github.com/CorporationX/user_service/pull/631/files)
7. Album visibility system
     - Description: In the application, users can create albums of posts. It is essential to include a visibility setting for each album. This means that an album created by a specific user can be accessed by: All users, Only their subscribers, Only users selected by the author, Only the author. 
     - [implementation](https://github.com/CorporationX/post_service/pull/274/files)
8. Comment system
     - Description: As your application allows users to create posts, there is a need to develop a comment system that enables users to leave comments under these posts.
     - [implementation](https://github.com/CorporationX/post_service/pull/59/files)
9. Mentorship request analysis
     - Description: The analytics service is required to gather information about mentoring requests sent from one user to another
     - [implementation](https://github.com/CorporationX/analytics_service/pull/20/files)
10. Creating an original link
     - Description: The UrlController must include a GET /{hash} endpoint that redirects the user to the original link associated with the hash in the databas
     - [implementation](https://github.com/CorporationX/url_shortener_service/pull/52/files)
11. Jacoco connection
     - Description: Connect and configure Jacoco in project_service
     - [implementation](https://github.com/CorporationX/project_service/pull/176/files)

# How to install a database and other tools locally?
Follow the instructions in the README in the `infra` section. This is a separate repository that contains all infrastructure components (DB, Redis, Docker Compose, etc.)
