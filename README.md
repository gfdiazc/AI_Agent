# SEO Content Automation with CrewAI

This project demonstrates how to automate SEO content creation using CrewAI, an AI-powered framework for building autonomous agents.

## Project Overview

This project leverages CrewAI to build a team of specialized AI agents that collaborate to produce high-quality, SEO-optimized content. The agents are designed to handle different stages of the content creation process, including keyword research, content writing, editing, and outreach for backlinks.

## Agents and Their Roles

The project defines four key agents:

- **SEO Researcher:** Conducts in-depth keyword research and develops a content strategy.
- **SEO Content Writer:** Writes compelling, SEO-optimized articles.
- **Content Editor:** Proofreads and improves content quality, ensuring clarity, readability, and SEO effectiveness.
- **Outreach/Link Builder:** Identifies guest posting opportunities and builds backlinks for SEO content.

## Workflow

The agents collaborate in a sequential workflow:

1. **Keyword Research:** The SEO Researcher identifies relevant keywords and trends for the chosen topic.
2. **Backlink Research:** The Outreach Specialist finds guest post and backlink opportunities.
3. **Content Writing:** The SEO Content Writer creates an SEO-optimized article based on the keyword research and backlink suggestions.
4. **Content Editing:** The SEO Content Editor refines and optimizes the article for clarity, readability, and SEO effectiveness.

## Tools Used

The project utilizes various tools from CrewAI and Langchain to enhance the agents' capabilities:

- **CrewAI Tools:** `SerperDevTool`, `WebsiteSearchTool`, `TXTSearchTool`, `ScrapeWebsiteTool`, `MDXSearchTool`, `JSONSearchTool`
- **Langchain Tools:** `GoogleTrendsQueryRun`, `GoogleTrendsAPIWrapper`, `GoogleSerperAPIWrapper`

## Setup and Installation

1. **Install Required Libraries:**
2. **Set Environment Variables:**
   - Obtain API keys for SerpAPI, Serper, DeepSeek, and OpenAI.
   - Store these keys in your Colab user data or a `.env` file.
   - Set the environment variables in your Colab notebook:
  
3. ## Usage

1. **Define Agents:** Create instances of each agent, specifying their role, goal, backstory, LLM, memory, verbosity, delegation permissions, and tools.
2. **Define Tasks:** Create instances of tasks, outlining the description, expected output, assigned agent, and tools.
3. **Assemble the Crew:** Create a `Crew` instance, adding the agents, tasks, and desired workflow (sequential in this case).
4. **Kickoff the Workflow:** Initiate the content creation process by calling the `kickoff` method on the `Crew` instance, providing the topic as input.

## Example

## Contributing

Contributions to this project are welcome! Feel free to submit pull requests for bug fixes, feature enhancements, or new agent implementations.

## License

This project is licensed under the [MIT License](LICENSE).
