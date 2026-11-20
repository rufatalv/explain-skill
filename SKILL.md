---
name: explain
description: Explain code, a flow, a task or a concept in ASD-STE100 (Simplified Technical English) style for a reader with ADHD. Use when the user invokes /explain, or asks to "explain", "walk me through", "what does this do", "how does X work", or asks for an explanation "for an ADHD-er" or "with the STE / ASD-STE100 standard".
---

# Explain

## Goal

Give an explanation the reader can scan in seconds and act on. Use ASD-STE100 writing rules and an ADHD-friendly layout.

## Language

Answer in the language of the user's request (English, Russian or Azerbaijani). Keep code, file names, identifiers and API names as they are.

## Before you write

1. Find the real answer first. Read the code, the task or the docs the question is about. Trace the whole flow end to end. Do not explain from guesses.
2. Find the one thing the reader must remember. That is the TL;DR.

## Layout

1. **TL;DR** first: 1–3 sentences. The answer, not an introduction.
2. Then short sections with `##` headings. One topic per section.
3. Use bullets and small tables in place of paragraphs. Use a table when items share the same fields (step, file, purpose).
4. Use numbered steps for a sequence or a flow ("Step 1 → Step 2").
5. Bold only the key word of a bullet, not whole sentences.
6. Put a short code snippet only when it shows the point better than words. Keep it to the lines that matter.
7. Link files as clickable references with line numbers (`[file.ts:42](path/file.ts#L42)`).
8. End with what to do next, or a "Warning" / "Note" section for risks and open questions. Do not end with a recap of what you already said.

## STE writing rules

- One idea per sentence. One instruction per step.
- Sentences of 20 words or fewer. Steps of 20 words or fewer.
- Active voice: "The filter removes the tab", not "The tab is removed by the filter".
- Use simple, common words. Use one word for one meaning, and keep the same term every time.
- Put the condition first: "If the user has no permission, the tab does not show."
- No filler: no "basically", "actually", "it is worth noting that", "as you can see".
- No long chains of nouns ("report tab permission filter logic"). Break them up.

## Code walkthroughs

When the user asks what code does:
- Show the flow as a table: step, file and line, what happens.
- Explain each important line or block in one short sentence.
- Say what the code does, then why, then any trap (a bug, a leak, an edge case).

## Length

- Match the depth to the question. A small question gets a short answer.
- If the explanation grows long, keep the TL;DR and the tables, and cut the prose.
