# An illustrative first conversation

This is an example of the intended interaction, not a recorded evaluation.
The actual question wording follows the selected conversation language.

**User:** Use Assert Skill. I have an idea for a small research-data tool.

**Assistant:** Which language should I use when talking with you, and which
language should the project's files and documentation use?

**User:** Conversation in English; project artifacts in Spanish.

**Assistant:** Before proposing the setup, please fill in the missing details:

1. What is its name, one-sentence goal and problem? Who will use it? What observable
   result will show that it is finished and works?
2. Any deadline, API/plan budget, environment constraints or sensitive data? What
   project-specific material must remain private? Please do not send credentials.
3. What must it explicitly not do?
4. I propose S, one bounded local task with a compact working document. Does that
   fit, or should it be M/L?
5. I propose stable R tools if this is statistical analysis; otherwise a suitable
   existing stack. Is a particular language or environment required?
6. Should it remain local/private (proposed default) or be public? Which license
   and, for a software product, open/open-core/closed model apply?
7. I propose functionality, accuracy and simplicity as the three priorities.
   Would you change them?

Once answered, the assistant presents the deductions, plan, selected roles/review
levels and files. It writes Spanish project artifacts only within authorized scope.
It does not ask these questions again when the original request already supplied
clear answers, or infer permission to upload from a public-visibility preference.
