# Project Title
**AI Blog Content Generation System**

# Problem Statement
The project aims to develop a system that generates high-quality blog content on any topics from YouTube videos.

# Dependencies and Requirements
* **Python version**: 3.8 or higher
* **Libraries**:
	+ crewai
	+ tools
	+ dotenv
	+ os
* **Tools**:
	+ YouTube Channel Search Tool (yt_tool)
	+ OpenAI API (openai_api_key and openai_model_name)

# Project Structure
The project consists of the following major files and folders:
* **agents.py**: Defines two agents: `Blog Researcher` and `Blog Writer`, which interact with the YouTube video and generate content.
* **crew.py**: Creates a `Crew` object, which orchestrates the tasks and agents to generate content.
* **tasks.py**: Defines two tasks: `Research Task` and `Writing Task`, which are executed by the agents.
* **tools.py**: Contains the `YoutubeChannelSearchTool` class, which searches for YouTube videos based on a given topic and channel handle.

# How to Run
1. Install the required libraries by running `pip install crewai tools dotenv`.
2. Set the OpenAI API key and model name as environment variables by running `export OPENAI_API_KEY=your_api_key` and `export OPENAI_MODEL_NAME=your_model_name`.
3. Run the `agents.py` script to create the agents.
4. Run the `crew.py` script to create the crew and execute the tasks.
5. The generated content will be stored in the `new-blog-post.md` file.

# Ideology and Solution
The project uses the `crewai` library to create a crew of agents that work together to generate blog content. The `agents` module defines two agents: `Blog Researcher` and `Blog Writer`, which interact with the YouTube video and generate content. The `tasks` module defines two tasks: `Research Task` and `Writing Task`, which are executed by the agents. The `tools` module provides a `YoutubeChannelSearchTool` class, which searches for YouTube videos based on a given topic and channel handle.

# Technologies Used
* **crewai**: A library for creating and managing AI-powered teams.
* **tools**: A library providing utility functions for tasks such as YouTube video search and processing.
* **dotenv**: A library for loading environment variables from a `.env` file.
* **os**: A Python library for interacting with the operating system.
* **OpenAI API**: A cloud-based API for generating text using AI models.

# Contact
For any queries, reach out to konashankar097@gmail.com.
