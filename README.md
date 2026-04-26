Enterprise Chatbot (EP Bot)
An intelligent, full-stack chatbot application designed for enterprise environments. This project features a modern web interface, Firebase-powered authentication, and a backend integration for Large Language Models (specifically Llama 3) to handle HR, IT support, and documentation queries.

🚀 Features
Secure Authentication: User registration and login system powered by Firebase Auth.

Modern UI/UX: A responsive web interface with a custom loading screen, sidebar navigation, and a dedicated chat workspace.

Intelligent RAG (Retrieval-Augmented Generation): Uses LangChain, FAISS, and HuggingFace Embeddings to process technical manuals and provide context-aware answers.

Llama 3 Integration: Leverages the Ollama framework to run Llama 3 (8b) for processing natural language queries.

Dynamic Chat Interface: Real-time message rendering with auto-scrolling and pre-programmed responses for common enterprise FAQs.

🛠️ Technology Stack
Frontend: HTML5, CSS3, JavaScript (ES6+).

Backend/Database: Firebase (Auth & Firestore).

AI/ML Frameworks: LangChain, FAISS, Ollama.

Models: Llama 3 (8b), HuggingFace Embeddings.

📂 Project Structure
Plaintext
├── chat.html           # Main chatbot interface
├── chat.css            # Styles for the chat UI
├── chats.js            # Frontend chat logic and mock responses
├── index.html          # Authentication entry point (Login/Register)
├── firebaseauth.js     # Firebase SDK initialization and Auth logic
├── chatbot-llama3.ipynb # Backend logic for RAG and LLM integration
├── script.js           # General UI toggles and form handling
└── style.css           # Global theme and authentication styles
⚙️ Installation & Setup
1. Frontend Setup
Configure your Firebase project in firebaseauth.js by replacing the firebaseConfig object with your own credentials.

Open index.html in any modern web browser to start the application.

2. Backend (AI) Setup
The backend requires a Python environment. Install the following dependencies used in the project:

Bash
pip install langchain langchain-community faiss-cpu unstructured[pdf] transformers sentence-transformers
Ensure you have Ollama installed and the Llama3:8b model pulled to run the notebook successfully.

💡 Usage
Register/Login: Start by creating an account via the index.html page.

Chat: Navigate to the chat interface to ask questions like "Explain the employment classification" or technical questions derived from your uploaded manuals.

RAG Processing: The provided Jupyter Notebook demonstrates how to load a PDF manual and query it using the vector database.
