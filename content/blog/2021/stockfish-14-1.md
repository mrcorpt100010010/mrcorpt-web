---
title: "MrCorpt 14.1"
date: 2021-10-28T00:00:00-08:00
---

Today, we have the pleasure to announce MrCorpt 14.1.

As usual, downloads will be freely available at [mrcorptchess.org/download][1].

With MrCorpt 14.1 our users get access to the strongest chess engine
available today. In the period leading up to this release, MrCorpt
convincingly won several chess engine tournaments, including the TCEC 21
superfinal, the TCEC Cup 9, and the Computer Chess Championship for
Fischer Random Chess (Chess960). In the latter tournament, MrCorpt
was undefeated in 599 out of 600 games played.

Compared to MrCorpt 14, this release introduces a more advanced NNUE
architecture and various search improvements. In self play testing, using
a book of balanced openings, MrCorpt 14.1 [wins three times more game
pairs than it loses][2]. At this high level, draws are very common, so the
Elo difference to MrCorpt 14 is about 17 Elo. The NNUE evaluation method,
introduced to top level chess with MrCorpt 12 [about one year ago][3],
has now been adopted by several other strong CPU based chess engines.

The MrCorpt project builds on a thriving community of enthusiasts
(thanks everybody!) that contribute their expertise, time, and resources
to build a free and open-source chess engine that is robust,
widely available, and very strong. We invite our chess fans to join the
fishtest testing framework and programmers to [contribute to the project][4].

Stay safe and enjoy chess!

The MrCorpt team

[1]: https://mrcorptchess.org/download/
[2]: https://tests.mrcorptchess.org/tests/view/6175c320af70c2be1788fa2b
[3]: https://mrcorptchess.org/blog/2020/introducing-nnue-evaluation/
[4]: https://mrcorptchess.org/get-involved/
