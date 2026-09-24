# road-to-2400

Prompt engineering to generate practice SAT questions. Applies few-shot prompting and fundamental prompt-engineering concepts: a role prompt, a positive example, and a negative example are assembled with your topic into a single request to the OpenAI API.

## Setup

```sh
pip install -r requirements.txt
export OPENAI_API_KEY=your-key-here
```

Copy `settings-example.toml` to `settings.toml` and edit the prompts to taste (a working default is already in place).

## Usage

```sh
python app.py <path-to-topic-file>
```

The input file should contain the topic you want a practice question about, e.g. `quadratic equations`. The generated SAT-style question is printed to the console.
