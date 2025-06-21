This project creates an automated system to:

- Fetch content from a given web URL
- Use AI to rewrite ("spin") and review the content
- Involve human input for editing and approval
- Save final versions with version control
- Retrieve content intelligently using a reinforcement learning-inspired method

---------------------------------------------------------------------------------------

Key Features : 

1. Scraping and Screenshots :
- Automatically scrapes text content from web pages
- Captures full-page screenshots

Example URL:
https://en.wikisource.org/wiki/The_Gates_of_Morning/Book_1/Chapter_1

Tool: Playwright

2. AI Writing and Reviewing :
- AI Writer: Rewrites chapters to make them more engaging
- AI Reviewer: Edits for tone, clarity, and structure

Tool: OpenAI GPT-4 (can be replaced with Gemini)

3. Human-in-the-Loop Editing :
- CLI interface allows humans to:
- Review AI output
- Suggest improvements or approve directly

4. Agentic API-style Flow :
- Modular design that routes content through:
- Scraper → AI Writer → AI Reviewer → Human → Final Save

5. Versioning and Retrieval
- Uses ChromaDB for content version control
- Intelligent retrieval system based on:
- Embeddings
- Cosine similarity
- Bandit-style exploration-exploitation logic

---------------------------------------------------------------------------------------------

Tools Used and Purpose :

Python - Main development language
Playwright	- Web scraping and screenshots
OpenAI / Gemini	- AI writing and reviewing agents
ChromaDB	- Document storage and versioning
scikit-learn	- Cosine similarity calculations
JSON	- Logging feedback for retrieval learning

