<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" style="height:64px;margin-right:32px"/>

# generate a readme.md file for this that i can download

Absolutely! Here’s a full **README.md** for your project, formatted for GitHub. You can copy this text and save it as a file named **README.md** in your repository.

***

# AI Video Blog Content Generator

Automate the research and writing of blog posts on trending tech topics, directly from YouTube videos, using a crew of collaborating agents powered by local LLMs.

## 🚀 Overview

This repository turns YouTube video content into compelling blog posts. Agents research, transcribe, and write—from a specific channel—using privacy-focused, locally-hosted LLMs (Ollama/Llama3.2). Orchestration is handled by CrewAI.

- **Researcher Agent:** Finds, transcribes, and analyzes relevant videos.
- **Writer Agent:** Summarizes and crafts the blog post.
- **YouTube Channel:** Currently set to `@krishnaik06` (AI, ML, Data Science topics).


## 🛠️ Features

- Multi-agent collaboration (CrewAI)
- Local LLM (Ollama/Llama3.2) for privacy
- Memory and caching for efficiency
- Automated blog post markdown output
- Easily configurable topic and channel


## 📁 Folder Structure

```
.
├── agents.py             # Agent definitions & LLM configuration
├── crew.py               # Orchestrates agent workflow
├── tasks.py              # Specifies research & writing tasks
├── tools.py              # Sets YouTube channel search tool
├── requirements.txt      # Dependencies
└── new-blog-post.md      # Generated blog post
```


## 🔧 Setup \& Installation

1. **Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/ai-video-blog-generator.git
cd ai-video-blog-generator
```

2. **Install Python dependencies**

```bash
pip install -r requirements.txt
```

3. **Install \& Run Ollama (Llama3.2 model)**
    - Download and install [Ollama](https://ollama.com).
    - Pull and run the Llama3.2 model:

```bash
ollama pull llama3:2
ollama serve
```

4. **Set up environment variables**
    - Create a `.env` file in your repo root:

```
OPENAI_API_KEY=your_openai_api_key
```


## ⚡ Usage

To generate a new blog post:

```bash
python crew.py
```

- The default topic is `AI VS ML VS DL vs Data Science`.
- Output is saved as `new-blog-post.md`.
- Change topic by editing `crew.py` or support CLI arguments.


## 📝 Configuration

- **Change YouTube Channel:** Edit the `youtube_channel_handle` in `tools.py`.
- **Agents \& Models:** Edit `agents.py` to change agent goals or LLM settings.
- **Output file:** Customize file name/output in `tasks.py`.


## 🤖 Agents

- **Blog Researcher:** Transcribes and analyzes video content.
- **Blog Writer:** Writes compelling markdown blog posts from research.


## 🗃️ Dependencies

- `crewai`
- `crewai_tools`
- `load_dotenv`
- `yt_dlp`
- `youtube-transcript-api`
- `langchain-huggingface`

Install with `pip install -r requirements.txt`.

## ✨ Example Output

See `new-blog-post.md` for a sample generated post.

## 📄 License

Specify your license here (MIT, Apache 2.0, etc).

***

**Questions or issues?**
Raise a GitHub issue or reach out to the maintainer.

*Automated blog writing—powered by AI agents and YouTube content!*

***

You may now copy this README and save it as **README.md** in your project folder. If you need the file output, you can create and download it using your code editor.

<div style="text-align: center">⁂</div>

[^1]: crew.py

[^2]: tasks.py

[^3]: tools.py

[^4]: requirements.txt

[^5]: agents.py

