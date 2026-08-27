

🎯 Quiz Application

A Java-based desktop Quiz Application developed as a group project using Java Swing, JDBC, and MySQL. The application provides an interactive graphical interface for creating quiz questions, managing categories, and attempting quizzes.

📌 About the Project

The Quiz Application is designed to make the process of creating and taking quizzes simple and interactive.

The application uses Java Swing to create the graphical user interface and MySQL to store quiz-related information. JDBC is used to connect the Java application with the MySQL database.

Users can create questions, add multiple answer options, select the correct answer, and attempt quizzes through the application.

✨ Features

- 📝 Create quiz questions
- 📚 Create and manage quiz categories
- ❓ Add multiple answer options
- ✅ Select the correct answer
- 🎯 Attempt quizzes
- 🔀 Randomize questions
- 🔀 Randomize answer options
- 💾 Store quiz data in MySQL
- 🖥️ Java Swing graphical interface
- 🔗 JDBC database connectivity

🛠️ Technologies Used

- Java
- Java Swing
- JDBC
- MySQL
- MySQL Connector/J
- IntelliJ IDEA

📂 Project Structure

QuizApplication/
│
├── src/
│   ├── constants/
│   │   └── CommonConstants.java
│   │
│   ├── database/
│   │   ├── Answer.java
│   │   ├── Category.java
│   │   ├── JDBC.java
│   │   └── Question.java
│   │
│   ├── screens/
│   │   ├── CreateQuestionScreenGui.java
│   │   ├── QuizScreenGui.java
│   │   └── TitleScreenGui.java
│   │
│   └── App.java
│
├── lib/
│   └── mysql-connector-j-8.3.0.jar
│
├── Javareport.pdf
├── QuizGuiDatabase.iml
└── README.md

🗄️ Database

The application uses MySQL to store quiz information.

The database manages:

- Quiz categories
- Questions
- Answer options
- Correct answers

The application communicates with the database using JDBC.

Database Configuration

Database: quiz_gui_db
Host: 127.0.0.1
Port: 3306
Username: root

«Note: Update the MySQL username and password in the JDBC configuration according to your local system.»

🚀 Installation & Setup

Prerequisites

Make sure the following are installed:

- Java JDK
- MySQL Server
- IntelliJ IDEA
- MySQL Connector/J

1. Clone the Repository

git clone https://github.com/lohithkumar8763/QuizApplication.git

2. Open the Project

Open the cloned project in IntelliJ IDEA.

3. Set Up MySQL

Create a database named:

CREATE DATABASE quiz_gui_db;

Create the required tables for categories, questions, and answers.

4. Configure JDBC

Open:

src/database/JDBC.java

Update the database credentials according to your MySQL setup.

private static final String DB_URL =
        "jdbc:mysql://127.0.0.1:3306/quiz_gui_db";

private static final String DB_USERNAME = "root";

private static final String DB_PASSWORD = "your_password";

5. Add MySQL Connector

Make sure the MySQL Connector/J ".jar" file is added to the project dependencies.

6. Run the Application

Run:

src/App.java

The Quiz Application will start.

🎮 How to Use

1. Start the Application

Run "App.java" to launch the application.

2. Create Questions

The question creation screen allows users to:

1. Enter a question.
2. Select a category.
3. Enter answer options.
4. Select the correct answer.
5. Save the question.

The question and answers are stored in the MySQL database.

3. Take the Quiz

Users can start the quiz and answer the displayed questions.

Questions and answer options can be displayed in random order.

4. Database

JDBC is used to retrieve and store quiz information from the MySQL database.

🧩 Main Components

"App.java"

The main entry point of the application.

"TitleScreenGui.java"

Displays the initial screen of the Quiz Application.

"CreateQuestionScreenGui.java"

Provides the interface for creating and storing quiz questions.

"QuizScreenGui.java"

Provides the interface for attempting the quiz.

"JDBC.java"

Handles the connection between the Java application and MySQL database.

"Question.java"

Represents quiz question data.

"Answer.java"

Represents answer information and correct-answer details.

"Category.java"

Represents quiz category information.

🔄 Application Flow

                 ┌─────────────────┐
                 │   Start App     │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │  Title Screen   │
                 └────────┬────────┘
                          │
              ┌───────────┴───────────┐
              │                       │
              ▼                       ▼
     ┌─────────────────┐     ┌─────────────────┐
     │ Create Question │     │    Take Quiz    │
     └────────┬────────┘     └────────┬────────┘
              │                       │
              └───────────┬───────────┘
                          ▼
                 ┌─────────────────┐
                 │ MySQL Database  │
                 └─────────────────┘

🎓 Learning Outcomes

This project helped the team gain practical experience in:

- Java programming
- Object-Oriented Programming
- Java Swing
- GUI development
- JDBC
- MySQL
- SQL queries
- Database connectivity
- CRUD operations
- Event-driven programming
- Team collaboration

🔮 Future Improvements

The project can be further improved by adding:

- 👤 User registration and login
- ⏱️ Quiz timer
- 🏆 Leaderboard
- 📊 Score history
- 🎚️ Difficulty levels
- 📝 More question types
- 👨‍💼 Admin dashboard
- 🔐 Secure database credential management
- 🎨 Improved user interface

👥 Team Members

This project was developed as a group project.

1. Lohith Kumar — "GitHub" (https://github.com/lohithkumar8763)
2. Arya Bhaskar — "GitHub" (https://github.com/aryamadathil2005)
3. Nihal — "GitHub" (https://github.com/nihal4170)
4. Pooja P Bhaskar — "GitHub" (https://github.com/PoojaPBhaskar)

🌐 Repository

"QuizApplication – GitHub" (https://github.com/lohithkumar8763/QuizApplication)

📄 License

This project was developed as an academic group project for educational purposes.