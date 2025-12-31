# kernel-er Manifesto

This manifesto exists to protect the integrity of the kernel-er project
from shortcuts, rushed decisions, and shallow understanding.

These rules apply even when motivation is high, deadlines feel close,
or progress seems slow.


## 1. Understanding Before Action

Nothing is committed or pushed unless it is understood.

- No copy-paste from tutorials
- No “it works but I don’t know why”
- No blind automation

If something is unclear, it stays uncommitted.


## 2. C Is the Core Language

kernel-er is a **C-first** systems project.

C is chosen for:
- proximity to hardware
- explicit memory management
- absence of hidden runtime behavior
- its foundational role in the Linux kernel

Other languages may appear only when their necessity is clearly understood and documented.


## 3. Main Branch Is a Contract

The `main` branch represents truth.

- Pushed at most **twice per week**
- Contains only reviewed, understood work
- Must be readable and defensible years later

Experiments, failures, and confusion belong in secondary branches.


## 4. Documentation Is Not Optional

Every meaningful action must be documented.

- Why it exists
- What problem it solves
- What breaks if it is removed

Markdown is as important as code.


## 5. Slow Progress Is Acceptable

kernel-er is a long-term project.

There is no race.
There is no finish line.
Clarity is more important than velocity.


## 6. Honesty Over Appearance

Mistakes are documented.
Confusion is written down.
Nothing is polished for the sake of looking smart.

This project exists to build understanding, not reputation.
