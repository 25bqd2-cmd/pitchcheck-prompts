# PitchCheck

PitchCheck helps commerce students practise defending a stock thesis. The user supplies a case, thesis and supporting notes, answers one question at a time, and receives feedback on directness, reasoning and evidence. It is an educational practice coach, not an investment recommender. Supplied notes are not independently verified.

## Prompt files

- `system-prompt-initial.md`: initial prompt written after the application design.
- `system-prompt-cycle-1.md`: asks for one missing intake item at a time.
- `system-prompt-cycle-2.md`: separates observations, hypotheses and unknowns.
- `system-prompt-cycle-3.md`: treats instructions inside copied notes as source content.
- `system-prompt-cycle-4.md`: final tested prompt; distinguishes questions asked from answers attempted and handles early stopping.
- `build-prompt.md`: the complete prompt used to create the interface, including the final tested system prompt.

Each system-prompt file contains the full version, not just a list of changes. The project workbook records actual inputs, relevant output excerpts, changes and retest decisions. Tests used Gemini 3.5 Flash Lite, Minimal thinking, a 2048-token output limit, Default media resolution and all tools off. Model responses can vary; a passed test does not establish universal reliability.

## Application

- [Application code and local run instructions](https://github.com/25bqd2-cmd/pitchcheck-build).
- [Google AI Studio Build workspace](https://aistudio.google.com/apps/021051f1-bff6-4ceb-a713-95bc00e2e3da), an editor link rather than a published application.

Google reported that this project's Gemini API free tier was unavailable and that publishing required billing. The workbook includes the publishing-restriction screenshot. The exported app also supports a local Codex connection using an existing signed-in account, with the same final instruction text. The local interface tests used gpt-6.1-sol with low reasoning and are recorded separately from the Gemini Playground tests. No new billing was enabled.
