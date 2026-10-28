# uav-textbook-teacher

A Chinese-language teaching skill for *Small Unmanned Aircraft: Theory and Practice* by Randal W. Beard and Timothy W. McLain.

This is not a textbook summary. It turns the book's 14 chapters and appendices A–I into an interactive course: intuition first, then equations, worked examples, diagnostics, exercises, and simulation-project guidance. The teacher adapts explanations based on the learner's answers and states coordinate frames, units, sign conventions, assumptions, and failure conditions explicitly.

## What it covers

- Coordinate frames, kinematics, rigid-body dynamics, aerodynamics, propulsion, and wind
- Trim, linearization, transfer functions, state-space models, and flight modes
- Successive loop closure, TECS, and LQR autopilot design
- Sensors, observers, Kalman filtering, and full-state EKF
- Guidance design models, vector-field path following, path management, and Dubins paths
- RRT path planning, vision-guided navigation, geolocation, and precision landing
- Multirotor modeling, control, estimation, and trajectory following
- Appendix quick-reference material, including quaternions, implementation, trim/linearization, and probability

## Install

Copy this folder into the skills directory used by your agent, or install from the repository with a compatible skills CLI. The skill entry point is `SKILL.md`.

```bash
npx skills add https://github.com/xiaozhuwa/uav-textbook-teacher --skill uav-textbook-teacher
```

## Example prompts

```text
用 uav-textbook-teacher，从第1章开始教我。
教我第5章的配平和线性化。
给我讲EKF，讲完后出道题考我。
带我完成第10章的路径跟随项目。
```

## Source and attribution

The teaching notes are original Chinese study material based on the book. The book itself, including its PDF, figures, and full text, is **not** included or redistributed in this repository. Rights to the book remain with its authors and publisher.

This is an independent educational project and is not affiliated with or endorsed by the authors or publisher.

## Accuracy note

The chapter notes flag places where the source text is ambiguous or internally inconsistent. Verify those formulas against the original book before treating them as settled implementation guidance.
