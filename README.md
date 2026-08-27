# ppsspp-ci

Scratch runner for the Switch (libnx) build of PPSSPP.

It holds no source: the workflow checks out a branch of
[WizzardSK/ppsspp-libretro](https://github.com/WizzardSK/ppsspp-libretro) and builds it
in the `devkitpro/devkita64` container. It exists only because GitHub keeps workflows
disabled on forks behind a one-time toggle, and that toggle is not reachable through the
API - a repository that is not a fork runs them straight away.

Pick the branch to build with **Run workflow** (`workflow_dispatch`); it defaults to
`switch-build`. Delete this repo once the work lands upstream.
