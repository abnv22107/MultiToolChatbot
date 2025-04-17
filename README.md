# MultiToolChatbot

# 🧠 Agentic AI with Tool Usage via ReAct Framework

This project showcases how a Large Language Model (LLM) can intelligently respond to user queries by either:
- Answering directly, or
- Calling external tools like Arxiv and Wikipedia through APIs to retrieve and integrate real-time information.

## 🚀 Project Overview

Using the ReAct framework, this notebook demonstrates:
- **Tool Calling LLMs**: LLMs that understand which tool to invoke for which question.
- **Dynamic Tool Integration**: Responses are generated either directly by the LLM or after integrating tool outputs.
- **Modular Tool Setup**: Arxiv and Wikipedia tools are created using LangChain's community wrappers.

## 🔧 Tools Used

- **LangChain**:
  - `ArxivQueryRun` for fetching academic papers.
  - `WikipediaQueryRun` for retrieving encyclopedia data.
- **ReAct Framework**: A prompting pattern allowing reasoning and action.
- **LLMs**: Powering the intelligent response generation.

## 📚 Workflow Summary

1. **Input**: User poses a question.
2. **Decision**:
   - If the question can be answered directly, LLM responds.
   - Otherwise, the LLM selects and invokes the most relevant tool.
3. **Tool Response**: Tool fetches information and passes it back.
4. **Final Answer**: LLM composes or relays the answer to the user.
