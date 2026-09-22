# i-want-to-learn

[🇮🇷 فارسی](README.md) · 🇬🇧

**Short answers. No spoilers.** A skill that makes your coding agent teach instead of solve.

## What it does

Two rules, in priority order:

1. Never hand over the finished implementation — give the smallest piece that unblocks you, then make you write the rest.
2. Never bury it in prose — first line is the question or the action, no preamble, no "Hope this helps!".

Plus `/exam` mode: it reads *your* code and quizzes you on it, one question at a time, in Persian.

## Before / After

**Before**

> Great question! So the issue here is that your `useEffect` is missing a dependency array, which means it runs on every render. Here's the corrected version of your whole component: ...
> *(full 40-line file follows)*

**After**

> `Dashboard.tsx:18` — this effect runs on every render.
>
> What's different between an effect with `[]` and one with no second argument at all?

## The rules

Full text in [`skills/i-want-to-learn/SKILL.md`](skills/i-want-to-learn/SKILL.md).

**Teaching**
1. Withhold the implementation, the design decision, the diagnosis.
2. Give syntax, signatures, error meanings and docs facts instantly — those aren't lessons.
3. Climb one rung per message: point → ask → show the shape → unblock.
4. "Just tell me" is honored immediately, with no lecture.
5. Stuck three turns, or anything destructive or security-related → straight answer.
6. Asked to write code → scaffold with `TODO`s plus one worked example.

**Shape**
7. First line is the question or the action.
8. No preamble, no recap, no closers, no "Almost!".
9. State line every turn (`attempt 2 of 2`, `سؤال ۳ از ۷`).
10. Cap visible lists at 5. Specific time estimates. Matter-of-fact about mistakes.

## Install

Copy/paste into your CLI:

```
Install the i-want-to-learn skill from https://github.com/taharagsanjani/i-want-to-learn
```

Or drop `skills/i-want-to-learn/SKILL.md` into your agent's skills directory.

Then invoke `/i-want-to-learn`. Turn it off with "stop learn mode".

## Tune it

Fork, edit `skills/i-want-to-learn/SKILL.md`, install your copy. The two knobs most people want:

- **"What counts as the full thing"** — move items between withhold and give.
- **The ladder** — four rungs is the default. Two makes it gentler, and removing rung 3 makes it much harder.

## Credits

Output-shape rules adapted from [`i-have-adhd`](https://github.com/ayghri/i-have-adhd) (MIT).

## License

[MIT](LICENSE).
