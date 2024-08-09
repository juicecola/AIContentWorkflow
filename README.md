AI Content Creation Workflow
This project provides a web-based application for managing an AI-driven content creation workflow using Streamlit. The app allows users to generate, write, and edit content based on specified topics. It leverages various AI tools to assist with content planning, writing, and editing.

Features
Content Planning: Uses AI to create a detailed content plan, including audience analysis and SEO recommendations.
Content Writing: Generates a blog post based on the content plan.
Content Editing: Proofreads and edits the blog post to ensure grammatical correctness and alignment with the organization's writing style.
Requirements
Python 3.10 or higher
Streamlit
crewai library
langchain_groq library
crewai_tools library
python-dotenv library
pandas library
IPython library
Setup Instructions
Clone the Repository:

bash
Copy code
git clone <repository_url>
cd <repository_directory>
Create and Activate a Virtual Environment:

bash
Copy code
python -m venv env
source env/bin/activate
Install Required Packages:

bash
Copy code
pip install streamlit crewai langchain_groq crewai_tools python-dotenv pandas ipython
Create a .env File:

Create a .env file in the project root directory and add your API keys:

plaintext
Copy code
GROQ_API_KEY=your_groq_api_key_here
SERPER_API_KEY=your_serper_api_key_here
Run the Application:

Start the Streamlit app with the following command:

bash
Copy code
streamlit run app.py
Access the Application:

Open your web browser and navigate to http://localhost:8501 to interact with the application.

Code Overview
The app.py file contains the main code for the application. Here's a brief overview:

Environment Variables: Loads API keys from the .env file.
AI Tools: Initializes language models and search tools using the provided API keys.
Agents: Defines different roles in the content creation workflow:
Content Planner: Plans content strategy and outlines.
Content Writer: Writes the blog post based on the plan.
Content Editor: Edits the blog post for clarity and style.
Tasks: Defines tasks for planning, writing, and editing content.
Streamlit Interface: Provides a user interface for inputting the topic and starting the content creation workflow.
