# DSApractice
## 🚀 Overview
Welcome to DSApractice - your ultimate companion for mastering Data Structures and Algorithms (DSA)! This Spring Boot and MongoDB-based web application is designed to help you stay on top of your DSA practice by sending timely reminders and revision questions directly to your phone via WhatsApp, powered by Twilio.
## 📦 Features
- Automated Reminders: Receive daily reminders to keep your practice consistent.
- Randomized Questions: Get a random DSA question every day to challenge yourself.
- Twilio Integration: Seamlessly integrated with Twilio to send messages over WhatsApp.
- MongoDB Backend: Manage and store your practice questions and other data efficiently.
## 🔧 Getting Started
### Prerequisites
Before you begin, ensure you have the following:
- [Java 17+](https://adoptopenjdk.net/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Twilio Account](https://www.twilio.com/try-twilio)
### Installation
1. Clone the Repository:

```
  git clone https://github.com/your-username/DSApractice.git
   cd DSApractice
```




## Configuration File

Create a file named `application.properties` with the following content:

properties

# MongoDB Configuration

```
spring.data.mongodb.uri=mongodb://localhost:27017/your-database
```

 # Twilio Configuration
```
twilio.account.sid=your_account_sid
twilio.auth.token=your_auth_token
twilio.whatsapp.from=whatsapp:+1415523888
# application.properties
spring.data.mongodb.uri=mongodb://localhost:27017/your-database
twilio.account.sid=your_account_sid
twilio.auth.token=your_auth_token
twilio.whatsapp.from=whatsapp:+14155238886
```

**📦Usage**
### Schedule Messages
The application is configured to send a random DSA question daily at 9 AM. You can adjust the schedule in the MessageScheduler class.
### Check Logs
Monitor your Twilio dashboard to see message logs and statuses.
### API Endpoints
- **Search by Name**: GET /api/questions/searchByName?name={name}
- **Search by Tags**: GET /api/questions/searchByTags?tags={tag1}&tags={tag2}
## 📄 How It Works
1. **Twilio Integration**: The application uses Twilio's API to send WhatsApp messages. It sends a random DSA question daily to a specified phone number.
2. **Spring Boot**: Manages scheduling, message handling, and API endpoints.
3. **MongoDB**: Stores questions and user data, ensuring efficient data retrieval and management.
## 🔧 Customization
- **Change the Schedule**: Modify the cron expression in MessageScheduler to adjust when messages are sent.
- **Update Questions**: Add or modify questions in the questions array within the MessageScheduler` class.
## 🧪 Testing
Ensure that the application is running and your Twilio account is properly set up. Use the provided API endpoints to test searching functionality. Verify that reminders and questions are sent as expected.
## 📚 Resources
- [Spring Boot Documentation](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)
- [Twilio API Documentation](https://www.twilio.com/docs/whatsapp)
- [MongoDB Documentation](https://docs.mongodb.com/)
📧 ContactClaude currently cannot access the internet or reference links
For any issues or suggestions, feel free to reach out: This is a .md file make it look better without changing content.I mean add motivation etc and images which will make standout for a job
Email: meghanadh777@gmail.com
GitHub Issues: DSApractice Issues

