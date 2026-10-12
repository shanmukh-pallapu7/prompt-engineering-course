# Prompt Engineering Course

Hands-on notes and runnable Python examples for learning prompt engineering with the Gemini API. Each module explains a technique, shows a working example and ends with practice tasks.

## Modules

| Module | Topics | Status |
|---|---|---|
| [00-prompting-techniques](00-prompting-techniques) | Zero-shot, one-shot, few-shot, multi-shot, Chain-of-Thought, zero-shot Chain-of-Thought | Done |

More modules (structured output, evaluation, tool use) will be added as I work through the course.

## What is inside each module

- `examples/` - runnable Python scripts, one per technique
- `prompts/` - short concept notes for each technique
- `assignments/` - practice tasks
- `helper.py` - a small reusable function for calling the API
- `.env.example` - the format of the environment variables you need

## Quick start

```bash
git clone https://github.com/shanmukh-pallapu7/prompt-engineering-course.git
cd prompt-engineering-course/00-prompting-techniques
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env   # then add your own GEMINI_API_KEY
```

Never commit your `.env` file or API keys.

## What I am learning

- How the way a prompt is written changes the model's output
- When to use examples (few-shot) and when step-by-step reasoning (Chain-of-Thought) helps
- Writing small reusable helpers around an LLM API

## Next

See my [LLM tool-calling agent](https://github.com/shanmukh-pallapu7/llm-tool-calling-agent), which applies these ideas to an agent that picks and runs tools.
