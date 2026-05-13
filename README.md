# AI-Powered Expense Tracker

A full-stack web application built with Spring Boot and Thymeleaf 
that uses Claude AI API to analyze spending patterns and generate 
personalized budget insights.

## Tech Stack
- **Backend:** Spring Boot, Spring Data JPA
- **Frontend:** Thymeleaf, HTML, CSS
- **Database:** MySQL
- **AI:** Claude API (Anthropic)

## Features
- Add, Edit, Delete expenses
- Category-wise expense tracking
- Monthly summary reports
- AI-powered personalized budget insights

## Setup Instructions

### Prerequisites
- Java 17+
- MySQL
- Maven

### Steps
1. Clone the repository
   git clone https://github.com/yourusername/ai-expense-tracker.git

2. Configure MySQL in application.properties
   spring.datasource.url=jdbc:mysql://localhost:3306/expense_tracker
   spring.datasource.username=your_username
   spring.datasource.password=your_password

3. Add Claude API Key in application.properties
   claude.api.key=your_api_key_here

4. Run the application
   mvn spring-boot:run

5. Open browser
   http://localhost:8080

## Project Structure
src/
├── controller/
│   ├── ExpenseController.java
│   └── AIInsightController.java
├── service/
│   ├── ExpenseService.java
│   └── ClaudeAIService.java
├── model/
│   └── Expense.java
├── repository/
│   └── ExpenseRepository.java
└── templates/
    ├── index.html
    ├── add-expense.html
    └── insights.html
