<p align="center"><img src="icons/icon.svg" alt="" width="160"></p>

# Amethyst Viewer

Amethyst Viewer watches Beat Saber replays and autoplays Beat Saber maps, competitive (ranked)
maps first, the way a top player would. Its autoplay, the bot, writes the play as a
[BSOR](https://github.com/BeatLeader/BS-Open-Replay) replay, the format BeatLeader records
players' plays in, which the viewer's own replayer plays beside theirs.

Each release on the [Releases](../../releases) page provides:

- **Installer** (`.exe`): installs the app. It is unsigned, so Windows SmartScreen may warn on
  first launch.
- **Archive** (`.zip`): the app alone, to extract and run without installing.

## Usage policy

Amethyst only computes replays locally. It never submits replays or scores and never makes a
POST or any other write request to any service. It makes only read-only GET requests, one per
action of its user, to download maps from BeatSaver and a difficulty's top scores and their
replays from BeatLeader or ScoreSaber, with a project User-Agent, a cache and throttling.
