# Persona Trainer

Welcome to the AI Persona Trainer for Slang language Game(https://github.com/tanaka-0224/hackathon)! 

This application serves as an innovative tool, utilizing advanced language models to interact and engage users through unique, conversational experiences.

- **Slang Sensei**  
*who can set up a persona by assistant_id*

- **Assistant Api from ChatGPT**  
*assist remember all of chat by thread_id*

## Installation

- **Requirement**:

```bash
git clone https://github.com/YoRsk/persona-trainer.git
cd persona-trainer
pip install -r requirements.txt
```
add CHATGPT_API_KEY in .env file of home page like this
```bash
OPENAI_API_KEY = "sk-xxxxxxxxxxxxxxxxxxxxxxxxx"
```


## Usage

This will launch the Flask API server. 

/gpt/process_slang: Processes input slang and returns a contextual sentence.
```bash
{
  "slang": "The slang term to process",
  "thread_id": "(Optional) The specific thread ID",
  "assistant_id": "(Optional) The specific assistant ID"
}

```

/gpt/scene_chat: Engages in a scene chat with the predefined assistant.
```
{
  "input_sentences": "The sentence(s) to include in the scene chat",
  "thread_id": "(Optional) The specific thread ID",
  "assistant_id": "(Optional) The specific assistant ID"
}

```
