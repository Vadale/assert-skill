# A — Interview the user after establishing both languages

This is a real project interview, not a description of the method. Reuse explicit
current-project answers; do not ask them again. Ask only remaining questions in
one plain-language numbered message, in the conversation language. Keep these
seven categories covered, even when some are already answered or inapplicable.
Use concise closed choices with the proposed default marked; an available host
question UI is optional, not required. Open facts have no invented answers.

1. **Identity and success.** What is the project called? What is its one-sentence
   goal, which problem does it solve, and who is its intended user or reader?
   What observable result will show that it is finished and works?
   If several audiences are named, identify the first intended user and one
   representative workflow, reusing known priorities. Resolve this choice only
   when it changes the initial deliverable.
2. **Constraints and private material.** Is there a meaningful deadline or API/
   plan budget? Any environment restrictions, sensitive data or credentials?
   What project-specific data, prompts, logic or other material must never be
   shared, beyond the private working scaffolding? Protect actual credentials
   from the start; use environment variables/ignored local configuration where
   appropriate, never a request to paste secrets into the interview.
3. **Non-goals.** What must this project explicitly not do?
4. **Size.** Propose the smallest credible S (bounded spike), M (maintained tool)
   or L (substantial product) setup, explaining the consequences. Start roughly
   one size below the initial impression when credible; risk still overrides size.
5. **Stack.** Propose suitable stable tools or ask about required technologies.
   Retain explicit stack/environment constraints. Python/JS/C are usual software
   starting points; prefer R for appropriate statistics. These are overridable
   defaults, not permission to replace an existing workflow or install anything.
6. **Distribution and licensing.** Should the product remain local/private or
   be public? What license should apply, and, for a software product, should it
   be open, open-core or closed? Offer local/private as a proposal when unknown.
   Mark irrelevant choices as inapplicable; never silently invent a public
   license or treat a visibility preference as permission to upload/create remotes.
7. **Quality priorities.** Propose three priorities from functionality, accuracy,
   security, bug finding, simplicity, simplification, optimization and
   maintainability. Ask for confirmation/correction if not already established;
   required risk controls apply whatever the selected priorities.

Infer project type, proportionate roles, file-based memory and comment density
without extra questions. Expose those deductions in the proposal so they can be
corrected: project files are the source of truth, internal assistant memory only
a cache; comments explain constraints the code cannot express. Add a code graph
only when repository complexity and a concrete navigation need justify its cost,
not automatically at a line-count threshold.

Wait for consequential missing facts/decisions before proceeding to the proposal
and authorized setup. A genuine unresolved gap can require clarification; do not
invent an answer to satisfy an arbitrary round limit. If answers already cover
the categories, proceed directly and state the deductions. Record unresolved
future distribution decisions without blocking unrelated authorized local work.
