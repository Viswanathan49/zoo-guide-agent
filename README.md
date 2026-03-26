# Zoo Tour Guide AI Agent 🦒

An interactive **multi-agent AI tour guide** that answers questions about zoo animals using Google ADK and Gemini 2.5 Flash. It acts like a smart zoo companion, helping visitors learn fun facts, habitats, diets, and behaviors through natural language chat.

## 🚀 Features

- Natural language Q&A about any zoo animal  
- Multi-agent workflow with dedicated **Researcher** and **Formatter** agents  
- Live lookups from Wikipedia for fresh, accurate information  
- Friendly, human-like responses optimized for visitors and learners  
- Cloud-ready deployment for demos or real-world kiosks  

## 🧠 Architecture

The app follows a simple but powerful multi-agent pattern:

1. **User** asks a question like:  
   - “What do giraffes eat?”  
   - “Are tigers nocturnal?”  
   - “Tell me an interesting fact about penguins.”
2. **Researcher Agent**  
   - Uses Google ADK + LangChain Wikipedia tool to search for relevant animal information.  
   - Extracts key facts, behaviors, and interesting details.
3. **Formatter Agent**  
   - Takes the raw research and rewrites it into a clear, friendly answer.  
   - Adapts tone to be concise, visitor-friendly, and engaging.

This separation keeps research and presentation clean and makes it easy to extend with more agents later (e.g., a Kid-Friendly Agent, Fun-Facts Agent, or Quiz Agent).

## 🧰 Tech Stack

- **Google ADK** – Orchestrates the AI pipeline and multi-agent logic  
- **Gemini 2.5 Flash** – Core LLM powering the agents  
- **LangChain Wikipedia Tool** – Fetches up-to-date facts about animals  
- **Google Cloud Run** – Serverless deployment for scalable hosting  
- **Python** – Core application logic and glue code  

## 🔧 How it works (flow)

- Receive user question → route to Researcher Agent  
- Researcher queries Wikipedia, extracts key information  
- Formatter Agent rephrases the result into a friendly response  
- Final answer is returned to the user in a chat-like interface  

## 🌱 Possible Extensions

- Add **kid mode** with simpler language and emojis  
- Support for **multiple languages** for international visitors  
- Integrate **images or short videos** of animals  
- Build a **kiosk UI** for on-site zoo installations  

## 📦 Getting Started

> Adapt these commands to your actual project structure if file names differ.

```bash
# Clone the repo
git clone https://github.com/Viswanathan49/zoo-guide-agent.git
cd zoo-guide-agent

# (Optional) Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

Set your environment variables (API keys, project IDs, etc.), then run the app (example):

```bash
python app.py
```

## 🤝 Contributions

Contributions, ideas, and feature requests are welcome!  
Feel free to open an issue or submit a pull request.

## 📫 Contact

**Viswanathan S**  
[viswanathansk49@gmail.com](mailto:viswanathansk49@gmail.com)
