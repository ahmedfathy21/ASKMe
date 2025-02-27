# AskMe System

## Overview
The AskMe System is a C++ application that allows users to ask and answer questions anonymously or publicly. Users can interact with each other by asking questions, answering them, and managing their questions. The system supports threading, allowing users to follow up on questions with additional related questions.

## Features
1. **User Authentication**:
   - **Login**: Existing users can log in using their username and password.
   - **Sign Up**: New users can create an account by providing a username, password, name, email, and preference for anonymous questions.

2. **Question Management**:
   - **Ask Questions**: Users can ask questions to other users. Questions can be anonymous or public, depending on the recipient's preferences.
   - **Answer Questions**: Users can answer questions directed to them.
   - **Delete Questions**: Users can delete their own questions.
   - **Threaded Questions**: Users can ask follow-up questions in a thread, creating a conversation around the original question.

3. **Question Display**:
   - **Questions To Me**: Users can view all questions directed to them.
   - **Questions From Me**: Users can view all questions they have asked to others.
   - **Feed**: Users can view a feed of all answered questions in the system.

4. **User Management**:
   - **List Users**: Users can view a list of all system users with their IDs and names.

5. **Data Persistence**:
   - **File Storage**: User and question data are stored in text files (`users.txt` and `questions.txt`), ensuring data persistence across sessions.

## Code Structure
The project is structured into several key components:

1. **Helper Methods**:
   - **File Handling**: Methods to read from and write to text files.
   - **String Manipulation**: Methods to split strings and convert strings to integers.
   - **Input Validation**: Methods to ensure user input is within a specified range.

2. **Question Class**:
   - Represents a question with attributes such as question ID, parent question ID, user IDs, anonymity status, question text, and answer text.
   - Methods to print questions in different formats (to user, from user, and feed).

3. **User Class**:
   - Represents a user with attributes such as user ID, username, password, name, email, and preference for anonymous questions.
   - Methods to print user details and manage user-related questions.

4. **QuestionsManager Class**:
   - Manages all questions in the system.
   - Handles loading and updating the question database.
   - Provides methods to ask, answer, delete, and list questions.

5. **UsersManager Class**:
   - Manages all users in the system.
   - Handles user authentication (login and sign-up).
   - Provides methods to list users and update user data.

6. **AskMeSystem Class**:
   - The main system class that integrates user and question management.
   - Provides a menu-driven interface for users to interact with the system.

## How to Use
1. **Compile and Run**:
   - Compile the C++ code using a C++ compiler (e.g., `g++`).
   - Run the executable to start the AskMe System.

2. **Login or Sign Up**:
   - Existing users can log in using their credentials.
   - New users can sign up by providing the required information.

3. **Interact with the System**:
   - Use the menu options to ask questions, answer questions, delete questions, and view questions.
   - Explore the feed to see answered questions from other users.

## File Structure
- **users.txt**: Stores user data in a comma-separated format.
- **questions.txt**: Stores question data in a comma-separated format.

## Example Data Format
- **User Data**: