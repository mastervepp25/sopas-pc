Here’s a customized README.md file for your Sopas PC project based on the AgenticSeek structure and your GitHub repo:


---

# Sopas PC: Private, Local AI Agent

<p align="center">
<img align="center" src="./media/sopas_pc_logo.png" width="300" height="300" alt="Sopas PC Logo">
</p>

**Sopas PC** is a 100% local, privacy-focused AI assistant that can browse, code, and perform complex tasks entirely on your machine. Designed for local LLMs, it guarantees zero cloud dependency.

## Features

- **Private & Local** – Runs on your hardware with no data sent to the cloud.
- **Web Browsing** – Can search, read, extract, and interact with websites.
- **Autonomous Coding** – Supports multiple programming languages.
- **Task Planning** – Breaks down complex goals into executable steps.
- **Voice Interface** – Voice-to-text and text-to-speech capabilities.

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/mastervepp25/sopas-pc.git
cd sopas-pc

2. Rename Environment File

cp .env.example .env

3. Setup Python Environment

python3.10 -m venv sopas_env
source sopas_env/bin/activate
# For Windows: sopas_env\Scripts\activate

4. Automatic Installation (Recommended)

Linux/MacOS:

chmod +x install.sh
./install.sh

Windows:

./install.bat

5. Manual Installation (Optional)

Install required packages manually:

pip install -r requirements.txt

Ensure you install ChromeDriver and other OS-specific dependencies (see original AgenticSeek docs for full setup).


---

Run Sopas PC

Start services:

source sopas_env/bin/activate
sudo ./start_services.sh  # Mac/Linux
start ./start_services.cmd  # Windows

Launch in CLI mode:

python cli.py

Launch in Web mode:

python api.py

Then visit http://localhost:3000/.


---

Configuration

Edit the config.ini to customize:

[MAIN]
is_local = True
provider_name = ollama
provider_model = deepseek-r1:14b
provider_server_address = 127.0.0.1:11434
agent_name = Sopas
work_dir = /home/user/sopas_workspace
...


---

Contribution

We welcome contributors! Fork, clone, and open pull requests.


---

License

GPL-3.0
