# mahmoud-prompt

An agent skill that turns whatever you write, in any language and any shape, into a professional, correct prompt for an AI model. It works in both **Claude Code** and **Codex**.

[العربية](#بالعربي)

## What it does

- Keeps your meaning: every requirement comes from what you wrote, nothing invented.
- Asks up to 3 short questions when something essential is missing.
- Writes the prompt in English by default (models follow it most precisely), keeping text that must stay in its original language as is.
- Structures it into: role and context, goal, detailed requirements, constraints, expected output, and success criteria.
- Gives you the prompt in one code block ready to copy, followed by any assumptions it made.

It writes the prompt only; it does not run it.

## Install

**Claude Code** (all projects):

```bash
git clone https://github.com/MahmoudSalem322/mahmoud-prompt ~/.claude/skills/mahmoud-prompt
```

**Codex** (all projects):

```bash
git clone https://github.com/MahmoudSalem322/mahmoud-prompt ~/.agents/skills/mahmoud-prompt
```

Restart the agent after installing.

## Use

```text
use mahmoud-prompt: I want an app for my gym where members book classes and pay monthly
```

Shortcuts: `/mahmoud-prompt` in Claude Code, `$mahmoud-prompt` in Codex.

---

## بالعربي

سكيل بتاخد أي شي بتكتبه، بأي لغة وبأي شكل، وبتحوّله لبرومت احترافي وصحيح للذكاء الاصطناعي، مفصّل وفيه كل النتائج المتوقعة. بتشتغل على **Claude Code** و **Codex**.

- بتحافظ على كلامك وما بتزيد متطلبات من عندها.
- إذا في شي ضروري ناقص، بتسألك 3 أسئلة كحد أقصى.
- البرومت بالإنجليزي بشكل افتراضي، والنصوص اللي لازم تضل بالعربي بتضل متل ما هي.
- بتعطيك البرومت جاهز للنسخ، وتحته الافتراضات اللي عملتها.

**التشغيل:** اكتب فكرتك وقول "استخدم سكيل mahmoud-prompt".

## License

MIT. See [LICENSE](LICENSE).
