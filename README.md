# 📊 NEET Rank Predictor

A Java-based application that analyzes quiz performance by fetching and processing quiz data from APIs. It identifies weak areas, detects trends, and predicts future performance.

## 🚀 Features
- 📌 **Fetches Quiz Data** from APIs
- 📈 **Performance Analysis** based on past quizzes
- 🔎 **Identifies Weak Areas** with low accuracy
- 🔮 **Predicts Future Performance** using moving averages
- 🏆 **Topic-wise & Overall Score Evaluation**

## 🛠️ Tech Stack
- **Programming Language:** Java
- **Libraries Used:**
  - `Jackson` (for JSON parsing)
  - `HttpClient` (for API requests)
  - `Stream API` (for data processing)
- **Build Tool:** Maven (optional for dependency management)

## 📂 Project Structure
```
📦 TestlineR1
 ┣ 📜 src
 ┃ ┣ 📜 main
 ┃ ┃ ┗ 📜 java/org/example/ApiFetcher.java
 ┃ ┣ 📜 models (QuizData, QuizSubmissionData, PastQuizData)
 ┣ 📜 pom.xml (If using Maven)
 ┣ 📜 README.md
```

## 🔧 Setup Instructions
### Prerequisites
- Install **Java 11+**
- IDE: **VS Code / IntelliJ / Eclipse**
- (Optional) **Maven** for dependency management

### Installation Steps
1. **Clone the repository**
   ```sh
   git clone https://github.com/your-username/quiz-performance-analysis.git
   cd quiz-performance-analysis
   ```
2. **Compile and Run the Application**
   ```sh
   javac -d out src/org/example/ApiFetcher.java
   java -cp out org.example.ApiFetcher
   ```
   *(If using Maven, simply run `mvn compile exec:java`)*

## 📜 Approach
### 1️⃣ **Data Fetching**
- Uses `HttpClient` to retrieve data from APIs.
- Parses JSON responses using `Jackson`.

### 2️⃣ **Performance Analysis**
- Groups quiz responses **by topic**.
- Calculates **average accuracy & score**.
- Flags topics with accuracy **below 70%** as weak areas.

### 3️⃣ **Future Prediction**
- Uses a **moving average** (last 3 quizzes) to estimate future accuracy.
- Warns if predicted accuracy is **below 70%**.

## 🏆 Future Improvements
- ✅ Add difficulty-level-based analysis
- ✅ Enhance visualization (Charts, Graphs)
- ✅ Implement a web dashboard

## 📜 License
This project is licensed under **MIT License**.

---
Made with ❤️ by **Anmol Pandya**

