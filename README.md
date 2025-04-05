❄️ coldemail-with-genai
An AI-powered tool that scrapes job postings, matches them with your portfolio, and generates personalized cold emails — all in one click.

Built with LangChain, ChromaDB, and Streamlit.

📁 Project Structure
graphql
Copy
Edit
coldemail-with-genai/
├── chains.py              # AI-based job extraction and email generation
├── main.py                # Streamlit app entry point
├── portfolio.py           # Portfolio management and vector database queries
├── utils.py               # Utility functions (e.g., text cleaning)
├── Pipfile                # Dependency management
├── sample_portfolio.csv   # Sample portfolio data
├── vectorstore2/          # Persistent ChromaDB vector store
├── testing/               # Jupyter notebooks for testing and experimentation
└── README.md              # Project documentation


cd coldemail-with-genai
2. Install Dependencies
Make sure Pipenv is installed:

bash
Copy
Edit
pipenv install
3. Activate the Virtual Environment
bash
Copy
Edit
pipenv shell
4. Launch the Streamlit App
bash
Copy
Edit
streamlit run main.py
🧠 How It Works
Paste a job posting URL into the Streamlit app.

The app:

Scrapes the job posting text.

Extracts key responsibilities and requirements.

Matches those with relevant portfolio projects.

Generates a cold email tailored to the job.

Copy and send the email to pitch yourself to clients or hiring managers!

🧩 Core Components
File	Description
chains.py	Uses LangChain's ChatGroq to extract job details and generate emails
portfolio.py	Manages portfolio data using ChromaDB
utils.py	Cleans and preprocesses scraped text
main.py	Streamlit front-end integrating all components
📊 Data & Storage
Portfolio CSV: sample_portfolio.csv with skills and project links.

Vector Store: ChromaDB stores embeddings for portfolio matching.

📦 Dependencies
Python 3.11+

LangChain

ChromaDB

Streamlit

JupyterLab


