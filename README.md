# ai-pr-desc

Writes your PR description so you don't have to. It reads the diff between your branch and the base branch, looks at your commit messages, and spits out a proper title and description.

## Install

```bash
npm install -g ai-pr-desc
```

## Setup

```bash
export OPENAI_API_KEY=sk-your-key-here
```

## Usage

```bash
# Diff against main (default)
npx ai-pr-desc

# Diff against a different base
npx ai-pr-desc --base develop
```

You'll get a title, a "what changed" section, a "why" section, and testing notes. Copy paste it right into GitHub.

## How it works

1. Figures out what branch you're on
2. Diffs it against the base branch
3. Grabs your commit messages
4. Sends all that to OpenAI
5. Returns a formatted PR description

No more staring at a blank PR template for 5 minutes.
