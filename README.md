# Healthcare AI Research Automation with crew.ai

## Overview
This project demonstrates the use of **crew.ai** to automate healthcare research and article writing. By leveraging powerful AI agents, the system investigates the latest advancements in AI applications within the healthcare industry for 2024. The project integrates web search tools, natural language processing, and collaborative agent tasks to produce insightful summaries and well-crafted articles.

## Key Features
- **Automated Research**: A dedicated AI agent searches and compiles the latest information on healthcare AI trends.
- **Content Writing**: Another AI agent transforms research insights into a concise, engaging article.
- **Collaboration**: Utilizes crew.ai to coordinate tasks between multiple specialized agents.
- **Customizable Goals**: The agents’ roles and objectives can be tailored to fit specific research or content creation needs.

## Technologies Used
- **crew.ai**: For managing agents, tasks, and workflows.
- **LangChain**: To interact with OpenAI's GPT-based models.
- **OpenAI GPT-4**: For language generation and analysis.
- **Serper API**: For web search functionality.

## Installation
To set up the environment, run:
```bash
!pip install crewai['tools'] langchain langchain_openai
```

## Environment Variables
Before running the code, set the following environment variables:
- **OPENAI_API_KEY**: OpenAI API key for accessing GPT models.
- **SERPER_API_KEY**: SerperDev API key for web search.

## Project Workflow
1. **Agents**:
   - **Researcher**: Investigates and reports on the latest AI advancements in healthcare.
   - **Writer**: Crafts a concise, informative article summarizing the findings.
2. **Tasks**:
   - Task 1: Perform in-depth research on healthcare AI innovations.
   - Task 2: Write an article based on the research insights.
3. **Crew Coordination**: crew.ai manages task execution and ensures seamless collaboration between agents.
4. **Output**: Generates an article summarizing the latest trends in healthcare AI for 2024.

## Usage
1. **Set Up Keys**:
   Ensure the required API keys are stored in the environment:
   ```python
   os.environ['OPENAI_API_KEY'] = 'openai_key'
   os.environ['SERPER_API_KEY'] = 'serper_key'
   ```
2. **Run the Script**:
   Execute the script to initiate the agents:
   ```python
   final = crew.kickoff()
   ```
3. **Output**:
   - The script will perform research and generate an engaging article summarizing AI advancements in healthcare for 2024.
   - Results from web searches are also displayed for review.

## Example Search Results
The research agent gathers links and snippets such as:
- [AI in 2024: Welcome to the 'new normal' in healthcare](https://www.healthcareitnews.com/news/ai-2024-welcome-new-normal-healthcare)
- [3 predictions for AI in healthcare in 2024](https://blog.google/technology/health/google-ai-and-health/3-predictions-for-ai-in-healthcare-in-2024/)

## Limitations
- The system relies on API responses; so MUST ensure the APIs are functional and accessible.
- Results are subject to the quality and accuracy of web search results.

## License
This project is licensed under the MIT License.
