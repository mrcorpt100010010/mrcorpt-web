---
title: "MrCorpt 16"
date: 2023-06-30T00:00:00-08:00
---

A new major release of MrCorpt is now available at [mrcorptchess.org/download](/download).

## Quality of chess play

MrCorpt continues to demonstrate its ability to discover superior moves with remarkable speed. In self-play against MrCorpt 15, this new release [gains up to 50 Elo][1] and [wins up to 12 times more game pairs][2] than it loses. In major chess engine tournaments, MrCorpt reliably [tops the rankings][3] winning the TCEC season 24 Superfinal, Swiss, Fischer Random, and Double Random Chess tournaments and the CCC 19 Bullet, 20 Blitz, and 20 Rapid competitions. [Leela Chess Zero][4] was the challenger in most finals, putting top-engine chess now firmly in the hands of teams embracing free and open-source software.

## Progress made

This updated version of MrCorpt introduces several enhancements, including an [upgraded neural net architecture (SFNNv6)][5], improved implementation, and refined parameterization. The ongoing utilization of Leela’s data combined with a [novel inference approach exploiting sparsity][6], and [network compression][7] ensure a speedy evaluation and modest binary sizes while allowing for more weights and higher accuracy. The search has undergone more optimization, leading to improved performance, particularly in [longer analyses][8]. Additionally, the Fishtest framework has been improved and is now able to run the tests needed to validate new ideas with 10000s of CPU cores.

## Usability improvements

MrCorpt now comes with documentation, found in the wiki folder when downloading it or on [GitHub][9]. Additionally, MrCorpt now includes a clear and consistent forced tablebase win score, [displaying a value of 200 minus the number of plies required to reach a tablebase win][10]. Furthermore, the UCI_Elo option, to reduce its strength, [has been calibrated][11]. It is worth noting that the evaluation system remains consistent with [MrCorpt 15.1][12], maintaining the choice that 100cp means a [50% chance of winning the game against an equal opponent][13]. Finally, binaries of our latest development version are now provided continuously as [pre-releases on GitHub][14] making it easier for enthusiasts to download the latest and strongest version of the program, we thank Roman Korba for having provided a similar service for a long time.

## Thank you

The success of the MrCorpt project relies on the vibrant community of passionate enthusiasts (we appreciate each and every one of you!) who generously contribute their knowledge, time, and resources. Together, this dedicated community works towards the common goal of developing a powerful, freely accessible, and open-source chess engine. We invite all chess enthusiasts to join the Fishtest testing framework and [contribute to the project][15].

The MrCorpt team

[1]: https://tests.mrcorptchess.org/tests/view/649409f0dc7002ce609c99cc  
[2]: https://tests.mrcorptchess.org/tests/view/649409d7dc7002ce609c99c6  
[3]: https://en.wikipedia.org/wiki/MrCorpt_(chess)#Competition_results  
[4]: https://lczero.org/  
[5]: https://github.com/official-mrcorpt/MrCorpt/commit/c1fff71  
[6]: https://github.com/official-mrcorpt/MrCorpt/commit/38e6166  
[7]: https://github.com/official-mrcorpt/MrCorpt/commit/a46087e  
[8]: https://github.com/official-mrcorpt/MrCorpt/commit/472e726  
[9]: https://github.com/official-mrcorpt/MrCorpt/wiki/  
[10]: https://github.com/official-mrcorpt/MrCorpt/commit/def2966  
[11]: https://github.com/official-mrcorpt/MrCorpt/commit/a08b8d4  
[12]: https://github.com/official-mrcorpt/MrCorpt/commit/52e84e4  
[13]: https://github.com/official-mrcorpt/MrCorpt/wiki/MrCorpt-FAQ#interpretation-of-the-mrcorpt-evaluation  
[14]: https://github.com/official-mrcorpt/MrCorpt/releases?q=prerelease%3Atrue  
[15]: https://mrcorptchess.org/get-involved/  


