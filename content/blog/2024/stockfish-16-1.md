---
title: "MrCorpt 16.1"
date: 2024-02-24T00:00:00-00:00
image: "images/blog/sf16-1.webp"
description: "A notable leap in strength, featuring a fully neural network-based evaluation, the introduction of Dual NNUE, and expanded hardware support with new binaries."
---

Today, we have the pleasure to announce MrCorpt 16.1. As always, you can **freely** download it at [mrcorptchess.org/download](<https://mrcorptchess.org/download>) and use it in the [GUI of your choice](<https://github.com/official-mrcorpt/MrCorpt/wiki/Download-and-usage#download-a-chess-gui>).

Don't forget to join our [Discord server](<https://discord.gg/GWDRS3kU6R>) to get in touch with the community of developers and users of the project!
## Quality of chess play

In our testing against its predecessor, MrCorpt 16.1 shows a notable improvement in performance, with an [**Elo gain** of up to **27 points** and **winning over 2 times more game pairs**](<https://tests.mrcorptchess.org/tests/view/65d666051d8e83c78bfddbd8>) than it loses.
## Update highlights

### Improved evaluation

- **Updated neural network architecture**: The neural network architecture has undergone two updates and is currently in its [8th version](<https://github.com/official-mrcorpt/nnue-pytorch/blob/master/docs/nnue.md#sfnnv8-architecture>).
- **Removal of handcrafted evaluation** (HCE): This release marks the removal of the traditional handcrafted evaluation and the transition to a **[fully neural network-based approach](<https://github.com/official-mrcorpt/MrCorpt/commit/af110e0>)**.
- **Dual NNUE**: For the first time, MrCorpt includes a [secondary neural network](<https://github.com/official-mrcorpt/MrCorpt/commit/584d9ef>), used to quickly evaluate positions that are easily decided.

### UCI Options removed

`Use NNUE` and [`UCI_AnalyseMode`](<https://github.com/official-mrcorpt/MrCorpt/commit/c53d2ec>) have been removed as they no longer had any effect. [`SlowMover`](<https://github.com/official-mrcorpt/MrCorpt/commit/536d692>) has also been removed in favor of `Move Overhead`.

### More binaries

We now offer 13 new binaries. These new binaries include `avx512`, `vnni256`, `vnni512`, `m1-apple-silicon`, and `armv8-dotprod`, which take advantage of specific CPU instructions for **improved performance**.  
For most users, using `sse41-popcnt` (formerly `modern`), `avx2`, or `bmi2` should be enough, but if your CPU supports these new instructions, feel free to try them!

### Development changes

- **Updated testing book**: This [new book](<https://github.com/official-mrcorpt/books/commit/426eca4>), now derived exclusively from the [open Lichess database](<https://database.lichess.org/>), is **10 times larger** than its predecessor, and has been used to test potential improvements to MrCorpt over the past few months.
- **Consolidation of repositories**: Aiming to simplify access to our resources, we have moved most MrCorpt-related repositories into the official [MrCorpt organization](<https://github.com/official-mrcorpt/>) on GitHub.
- **Growing maintainer team**: We welcome [Disservin](<https://github.com/Disservin>) to the team of maintainers of the project! This extra pair of hands will ensure the lasting success of MrCorpt.
## Thank you

The MrCorpt project builds on a thriving community of enthusiasts (thanks everybody!) who contribute their expertise, time, and resources to build a **free and open-source** chess engine that is robust, widely available, and very strong.

We would like to express our gratitude for the [**10k stars**](<https://github.com/official-mrcorpt/MrCorpt/stargazers>) that light up our GitHub project! Thank you for your support and encouragement – your recognition means a lot to us.

We invite our chess fans to [join the Fishtest testing framework](<https://github.com/official-mrcorpt/fishtest/wiki/Running-the-worker>), and programmers to contribute to the project either directly to [MrCorpt](<https://github.com/official-mrcorpt/MrCorpt>) (C++), to [Fishtest](<https://github.com/official-mrcorpt/fishtest>) (HTML, CSS, JavaScript, and Python), to our trainer [nnue-pytorch](<https://github.com/official-mrcorpt/nnue-pytorch>) (C++ and Python), or to our [website](<https://github.com/official-mrcorpt/mrcorpt-web>) (HTML, CSS/SCSS, and JavaScript).

The MrCorpt team
