# HealthTrack: Personal Health Monitoring Dashboard

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/LangChain-F19141?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain" />
</p>

An advanced, full-stack personal health monitoring dashboard with AI-powered insights and real-time data tracking.

This project provides a comprehensive platform to track vital signs, log daily activities, and analyze medical records. It leverages a modern tech stack, including Next.js for the frontend and FastAPI for the Python backend, and integrates AI capabilities via Langchain to offer personalized health insights.

## 📸 Screenshots

**(IMPORTANT: Add your own screenshots here!)**

*Drag and drop your project screenshots into this section. Here are some ideas for what to include:*

| Dashboard | AI Health Assistant |
| :---: | :---: |
|  |  |

| Mobile View | Medical Records |
| :---: | :---: |
|  |  |


## ✨ Key Features

* **🤖 AI-Powered Health Assistant:** Chat with an AI (powered by Langchain and OpenAI) to get personalized health insights and answers to your medical questions.
* **📈 Real-time Health Monitoring:** Designed to integrate with IoT sensors (like Arduino/ESP8266) to display live vital signs.
* **📂 Medical Record Analysis:** Securely upload and store medical records (like PDFs) and use the AI to extract and analyze key information.
* **🏃 Activity & Nutrition Tracking:** Log your daily activities, exercise routines, and nutritional intake.
* **📊 Comprehensive Dashboard:** A clean, responsive UI to visualize all your health metrics, trends, and progress in one place.
* **🔒 Secure Authentication:** Built with Supabase for secure user registration, login, and database management.

## 🛠️ Tech Stack

This project is a monorepo containing a separate frontend and backend.

### Frontend
* **Framework:** [Next.js](https://nextjs.org/)
* **Language:** [TypeScript](https://www.typescriptlang.org/)
* **Styling:** [TailwindCSS](https://tailwindcss.com/)
* **UI:** [Shadcn-UI](https://ui.shadcn.com/) / [Radix UI](https://www.radix-ui.com/)

### Backend
* **Framework:** [FastAPI (Python)](https://fastapi.tiangolo.com/)
* **Server:** [Uvicorn](https://www.uvicorn.org/)

### AI & Machine Learning
* **Orchestration:** [Langchain](https://www.langchain.com/)
* **Models:** [OpenAI](https://openai.com/), [Cohere](https://cohere.com/)

### Database & Auth
* **Platform:** [Supabase](https://supabase.com/)
* **Database:** [PostgreSQL](https://www.postgresql.org/)

## 🚀 Getting Started

Follow these instructions to get a local copy up and running.

### Prerequisites

* **Node.js & npm:** [Download Here](https://nodejs.org/en)
* **Python 3.10+ & pip:** [Download Here](https://www.python.org/)
* **Git:** [Download Here](https://git-scm.com/)
* **API Keys:**
    * Supabase (Project URL & Anon Key)
    * OpenAI API Key
    * Cohere API Key

### 1. Clone the Repository

Clone your forked repository to your local machine:
```bash
git clone [https://github.com/Gauravmangate27/HealthTrack-Personal-Health-Monitoring-Dashboard.git](https://github.com/Gauravmangate27/HealthTrack-Personal-Health-Monitoring-Dashboard.git)
cd HealthTrack-Personal-Health-Monitoring-Dashboard
```

### 2. Backend Setup (FastAPI)

1.  **Navigate to the backend directory** (assuming it's in a folder like `backend` or `api`):
    ```bash
    cd path/to/your/backend
    ```

2.  **Create and activate a Python virtual environment:**
    ```bash
    # Create venv
    python -m venv venv

    # Activate on Windows
    .\venv\Scripts\activate
    
    # Activate on macOS/Linux
    source venv/bin/activate
    ```

3.  **Install Python dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Create a `.env` file** in the backend directory and add your secret keys:
    ```.env
    SUPABASE_URL="YOUR_SUPABASE_PROJECT_URL"
    SUPABASE_KEY="YOUR_SUPABASE_SERVICE_ROLE_KEY"
    OPENAI_API_KEY="YOUR_OPENAI_KEY"
    COHERE_API_KEY="YOUR_COHERE_KEY"
    TAVILY_API_KEY="YOUR_TAVILY_KEY"
    ```

5.  **Run the backend server:**
    ```bash
    uvicorn main:app --reload
    ```
    The backend will be running at `http://127.0.0.1:8000`.

### 3. Frontend Setup (Next.js)

1.  **Open a new terminal** and navigate to the frontend directory:
    ```bash
    cd path/to/your/frontend 
    ```

2.  **Install npm dependencies:**
    ```bash
    npm install
    ```

3.  **Create a `.env.local` file** in the frontend directory and add your public keys:
    ```.env.local
    NEXT_PUBLIC_SUPABASE_URL="YOUR_SUPABASE_PROJECT_URL"
    NEXT_PUBLIC_SUPABASE_ANON_KEY="YOUR_SUPABASE_ANON_KEY"
    
    # The URL of your local backend server
    NEXT_PUBLIC_API_URL="[http://127.0.0.1:8000](http://127.0.0.1:8000)"
    ```

4.  **Run the frontend development server:**
    ```bash
    npm run dev
    ```

### 4. You're All Set!

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application live.

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improving the project, please fork the repo and create a pull request, or open an issue.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 🙏 Acknowledgments

* This project is based on the [health-monitor-next](https://github.com/CubeStar1/health-monitor-next) repository by **[CubeStar1](https://github.com/CubeStar1)**.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
