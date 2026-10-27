---
name: mahmoud-prompt
description: Mahmoud's prompt writer. Takes whatever the user wrote, in any language and in any shape, and rewrites it as a professional, correct prompt for an AI model, detailed enough for the model to understand exactly what is wanted and covering every expected result. It writes the prompt only; it does not carry it out. Use ONLY when the user explicitly asks for this skill by name, for example "use mahmoud-prompt" or "استخدم سكيل mahmoud-prompt". Never start it on your own for any other request.
---

# mahmoud-prompt

Turn what the user wrote into a professional prompt that another AI model can follow precisely. Your job is to write the prompt, not to do the task in it.

## Rules

- **Keep the user's meaning.** Every requirement in the prompt comes from what the user wrote. Make it clearer and more complete, but do not invent new requirements, features or constraints.
- **Ask when something essential is missing.** If the prompt cannot be written correctly without an answer (for example the target platform, or who the result is for), ask before writing, at most 3 short questions. Anything less important: make a reasonable assumption and list it after the prompt.
- **Language:** write the prompt in English by default, because models follow English most precisely. Keep anything that must stay in its original language exactly as the user wrote it (for example Arabic UI text, names, quotes). If the user asks for another language, use it.
- **Be explicit.** Say exactly what to do, in what order, and what the result must look like. Give the reason behind a requirement when it helps the model make good decisions.
- **No filler.** No flattery, no "you are the world's best", no repetition. Every line carries information.

## Prompt structure

Use these sections, in this order, with clear headings. Leave out a section only when the user's text gives nothing for it.

1. **Role and context:** who the model is acting as, and the background it needs: the project, the audience, what already exists.
2. **Goal:** the single outcome the user wants, in one or two sentences.
3. **Requirements:** everything the result must do or contain, in detail, as a numbered list. Split vague wishes into concrete, checkable points.
4. **Constraints:** what to avoid, limits on technology, style, length, tone or scope.
5. **Expected output:** every result the model must deliver, and the exact form of each: files, sections, format, length, language.
6. **Success criteria:** how to tell the result is correct and complete, as a checklist the model can verify before it answers.

If the user gave examples, data or text to work on, include them in the prompt inside clearly marked blocks (for example `<example>`, `<data>`), separate from the instructions.

## What to give the user

1. The finished prompt, inside one code block, so it can be copied as it is. Fence it with four backticks (````) so code blocks inside the prompt do not break it.
2. After the code block, a short list of the assumptions you made, if any, so the user can correct them.

Do not execute the prompt.
