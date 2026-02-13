# 🤖 LLM Prompts (Generate Paste-Ready Rules)

This repo maintains abuse/keyword lists in plain text for easier community contributions.

However, Reddit AutoModerator requires regex formatting, and YAML formatting must remain valid.

Use the prompts below to convert a plain list into a paste-ready rule.

---

# Prompt 1: Generate AutoModerator Rule (Copy-Paste YAML)

Copy the prompt below into any LLM (ChatGPT / Claude / Gemini), then paste your keyword list at the bottom.

```text
You are a Reddit AutoModerator config generator.

TASK:
Convert the keyword list below into a fully copy-paste ready AutoModerator rule in YAML format.

REQUIREMENTS:
- Output ONLY the final YAML rule, nothing else.
- Maintain proper YAML indentation.
- Use this exact structure:

---
type: comment
body (regex, includes): 
  - "<REGEX_PATTERN>"
action: filter
action_reason: "Abuse / hate keyword detected"
moderators_exempt: true
---

- Combine all keywords into ONE regex string.
- Each keyword must be wrapped like this:
  \b(?:KEYWORD)\b
- Keywords must be joined using pipe separators: |
- Do not remove any keyword.
- Do not rewrite keywords.
- Escape regex characters if required.
- Output must be valid YAML and directly pasteable into AutoModerator.

KEYWORD LIST STARTS BELOW:
(PASTE LIST BELOW THIS LINE)

You are a regex generator.

TASK:
Convert the keyword list below into a single regex pattern usable in Reddit moderation Automations.

REQUIREMENTS:
- Output ONLY the regex string, nothing else.
- Format each keyword as:
  \b(?:KEYWORD)\b
- Join keywords using pipe separators: |
- Keep output as ONE LINE.
- Do not remove or rewrite keywords.

KEYWORD LIST STARTS BELOW:
(PASTE LIST BELOW THIS LINE)
