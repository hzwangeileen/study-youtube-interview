---
name: study-youtube-interview
description: Turn a YouTube interview, podcast, subtitle file, or noisy ASR transcript into a learning-first document with a self-contained detailed core-content section and a source-faithful chronological QA transcript. Use when the user wants to 扒拉、学习、整理 or study a YouTube interview, preserve the original dialogue without over-compression, correct transcription errors, remove timestamps, or write the result to Feishu. Do not use for article publication, WeChat/Substack adaptation, promotional copy, or editorial reconstruction.
---

# Study YouTube Interview

## Goal

Produce study material that replaces watching the full interview:

1. Write detailed core-content bullets that explain the whole conversation without requiring the QA.
2. Preserve a lightly edited QA record for checking nuance, examples, reasoning, and speaker intent.

Keep this workflow separate from article publishing. Optimize for comprehension and source fidelity, not distribution.

Treat fidelity and readability as simultaneous requirements. Preserve what the speakers meant and the information they supplied, while repairing the transcript enough that a reader can understand it without hearing the audio. Fidelity does not mean copying ASR fragments, broken syntax, or unclear pronouns verbatim.

## Hard boundary: study notes, not an article

- Do not create title options, headline quotes, a promotional introduction, a cover-image slogan, a call to action, or a broad concluding uplift.
- Do not reorganize the interview into a new thesis or reader-conversion narrative.
- Do not make the guest sound more coherent, certain, strategic, or polished than the source supports.
- Do not add public background, recent developments, or analyst opinions to the body unless the user explicitly requests them.
- Use external sources only to verify proper nouns or resolve a clear ASR error. Keep substantive claims grounded in the interview.
- Do not generate Word, PDF, WeChat HTML, or publication assets unless explicitly requested.

If the user asks to publish or adapt the material later, switch to the relevant article/publishing skill in a new step. Do not silently change this output into an article.

## Source acquisition

Use this priority order:

1. Read user-provided transcripts, subtitle files, Feishu documents, or pasted text.
2. Attempt to access YouTube captions or another transcript only when tools permit.
3. Use the video title, description, official project pages, and speaker profiles only to verify names and technical terms.
4. If no transcript or captions are accessible, say so directly and ask the user to provide the transcription. Do not infer an interview from its title or description.

When multiple transcripts exist, prefer the most complete one and use the others as correction references. Treat ASR output as noisy evidence, not canonical prose.

## Workflow

### 1. Inspect the full source

- Read the full transcript before drafting the final output.
- Detect the host, guest, additional speakers, trailers, ads, and outro.
- Separate the real interview from opening montage clips, sponsor reads, and duplicated excerpts.
- Preserve the interview's original order.

For long transcripts, process sequential ranges and maintain a private coverage ledger. Record every source turn as kept, merged, corrected, excluded as filler, or excluded as non-interview material. Do not summarize chunks independently and then combine the summaries; that loses callbacks and repeated reasoning.

### 2. Build an ASR correction glossary

- Extract people, companies, products, models, papers, technical terms, acronyms, and numbers.
- Correct a term when context or a primary source makes the identity clear.
- Apply systematic corrections consistently across the document.
- Correct obvious punctuation, sentence-boundary, pronoun, and speaker-label errors.
- Phrase around an uncertain name or mark it as uncertain. Never replace an unclear term with a confident guess.
- Preserve a number only when its object, unit, and scale are understandable.

Do not treat stylistic awkwardness as an ASR error. Editing must not change the speaker's claim.

### 3. Create factual chapter boundaries

- Divide the interview into roughly 5–10 chapters according to real topic changes.
- Keep the chapters chronological.
- Write short, informative titles that state what the section discusses.
- Avoid clickbait, manufactured conflict, and article-style thesis headings.
- Place a chapter boundary before a new subject, not halfway through a continuing answer.

### 4. Produce the lightly edited QA

Preserve all substantive dialogue, including:

- the speaker's reasoning chain;
- concrete examples, stories, comparisons, and caveats;
- follow-up questions and meaningful interruptions;
- technical mechanisms and operational details;
- uncertainty, disagreement, and changes of mind.

Apply only these edits:

- remove greetings, pure filler, stutters, false starts, and exact repetition when they carry no meaning;
- merge consecutive segments from the same speaker;
- split very long answers at real topic or paragraph boundaries;
- simplify a rambling host question while retaining all factual premises;
- repair obvious ASR and punctuation errors.

Improve readability without changing meaning:

- Write complete Chinese sentences. Every declarative sentence must have an identifiable subject and predicate, plus an object or complement when the verb requires one.
- restore an omitted subject or object when the surrounding dialogue makes it unambiguous;
- replace an unclear pronoun with the actual person, company, project, or concept when safely recoverable;
- split run-on speech into complete sentences and short paragraphs;
- reorder nearby clauses when spoken-word order is difficult to follow;
- remove repeated self-corrections after preserving the speaker's final intended statement;
- add a short bracket-free clarification only when the source already supplies the meaning.

Do not leave transcript fragments such as `对`, `然后这个事情`, `所以其实是`, or a dangling noun phrase as standalone prose. Merge a meaningful confirmation into the adjacent sentence, expand it with the exact proposition being confirmed, or remove it when it is pure conversational filler. Questions may use natural Chinese ellipsis only when the referent is unmistakable in the same paragraph.

Keep uncertainty when the intended meaning cannot be recovered. Do not smooth an ambiguous answer into a definite claim. The finished Chinese should read like a careful transcript editor's work: natural and understandable, while still sounding like the original speakers rather than an article author.

Never compress a long answer into one conclusion. Never replace several examples with “她举了几个例子.” Do not invent a host question to make an answer neater; use a neutral subsection boundary when necessary.

Use the speakers' real names when known. Keep the name label and the first paragraph on the same line. For continued paragraphs from the same uninterrupted turn, omit the repeated label.

#### Mandatory sentence-by-sentence readability pass

After drafting the complete QA, reread every dialogue block in chronological order. This is a full-coverage editing pass, not a spot check of the longest or noisiest answers.

For each question and answer:

1. Identify what person, company, system, project, or idea performs the action.
2. Confirm that every declarative sentence has an explicit or unmistakable subject and predicate.
3. Add the object, complement, scope, unit, or referent required to understand the verb or claim.
4. Repair ASR sentence boundaries before polishing wording. Join clauses that the ASR split incorrectly; split run-ons only at genuine semantic boundaries.
5. Replace dangling `它 / 他 / 这个 / 那个 / 这件事` with the concrete referent when the source makes it recoverable.
6. Expand a meaningful short confirmation into the proposition being confirmed, merge it into the adjacent turn, or remove it if it contains no information.
7. Preserve the speaker's first-person viewpoint, uncertainty, emotional force, examples, and reasoning length. Do not turn the answer into an editor's summary.

Do not accept a paragraph merely because its individual words are recognizable. A reader who has not heard the audio must be able to identify who did what, to what object, for what reason, and with what limitation when the source supplies those elements.

Maintain a private dialogue-block audit for long interviews. Mark every host and guest block as `already clear`, `revised`, `merged`, or `removed as filler`. The audit exists to prove full coverage; do not add it to the delivered document unless requested.

### 5. Write the core-content section from the full source map

Write this section after mapping the complete QA, even though it appears before the QA in the document.

- Use as many bullets as the source requires; 10–18 is a useful range for a long interview, not a quota.
- Make every bullet independently understandable to someone who never watched the video.
- Start with a specific bold label.
- Include the actor, background, central point, reason or mechanism, representative example, and important limitation when present.
- Cover every major chapter and the interview's important closing ideas.
- Keep source uncertainty visible and avoid unsupported implications.
- Remove duplication across bullets, but do not make bullets so short that the reader must consult the QA.

The core section is a detailed substitute for the interview. It is not a list of teaser phrases and not a table of contents.

## Default output structure

Use this order unless the user requests otherwise:

```text
文档标题
视频链接 / 嘉宾 / 主持人 / 时长（when known）
整理说明

核心内容
- 10–18 detailed, self-contained bullets

QA 整理
01. Chapter title
Host：...
Guest：...

02. Chapter title
...
```

Do not include timestamps by default. Add them only when the user explicitly asks.

## Feishu formatting

When the destination is Feishu, also use the `lark-doc` skill and follow its update/fetch rules.

- Use H1 for `核心内容` and `QA 整理`; use H2 for numbered interview chapters.
- Use a native bullet list for the detailed core content.
- Put one independent blank paragraph between every top-level title, paragraph, dialogue block, and adjacent section. In Feishu XML, use `<p></p>` as the blank block.
- Keep the speaker label and dialogue in the same paragraph.
- Style the host label with an orange background and the guest label with a light-orange background plus orange text when the existing document supports those styles.
- Preserve the user's existing colors and hierarchy when updating a document.
- Do not overwrite unrelated content. Read the edited section back after writing.

## Validation

Before delivery, check all of the following:

- The core bullets cover every major chapter and can be understood without the QA.
- The QA retains the original chronology, reasoning, examples, caveats, and meaningful follow-ups.
- Every paragraph is understandable without replaying the audio; subjects, referents, sentence boundaries, and causal links are clear.
- No standalone fragment depends on tone, gesture, or the previous audio turn to supply its subject, predicate, or required object.
- Every dialogue block has been included in the sentence-by-sentence audit; count the host and guest blocks before delivery and investigate any unlabeled or unaudited block.
- Search the finished QA for common ASR residue: duplicated words, broken punctuation, dangling confirmations, unexplained pronouns, and uncertain proper nouns. Fix each hit or intentionally qualify it.
- No content was promoted into a stronger claim than the transcript supports.
- Real speaker names replace generic labels when safely known.
- Proper nouns are consistent; unresolved terms remain qualified.
- No timestamps remain unless requested.
- No opening montage, ad, or duplicated trailer dialogue was mistaken for the main interview.
- No publishing artifacts appear: title variants, headline quotes, promotional intro, CTA, or broad editorial conclusion.
- For Feishu, read the edited content back from Feishu rather than trusting the write response. Confirm headings, every speaker label, final paragraphs, and blank blocks are present, and spot-check the first, middle, and last chapters for fluent complete sentences.

If coverage is uncertain, report the missing source range or inaccessible transcript instead of claiming completion.
