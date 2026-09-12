<!-- Part of the Cookiy sell-sessions skill · https://github.com/cookiy-ai/sell-sessions-skill -->

![Cookiy](assets/logo.svg)

# sell-sessions-skill

**Sell your Claude Code and Codex sessions to AI labs. Local uploader, per-session opt-in, paid on every sale.**

[![stars](https://img.shields.io/github/stars/cookiy-ai/sell-sessions-skill?style=flat)](https://github.com/cookiy-ai/sell-sessions-skill/stargazers)
[![npm](https://img.shields.io/npm/v/@cookiyai/sell-agent-sessions?label=uploader)](https://www.npmjs.com/package/@cookiyai/sell-agent-sessions)
![local](https://img.shields.io/badge/runs-locally-success)
[![MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

```bash
npx @cookiyai/sell-agent-sessions
```

Opens a local web app on `localhost:4318`. It scans `~/.claude` and `~/.codex`, lists sessions by project with an estimated value each, scrubs secrets and PII on your machine, and uploads only what you tick. Installing or opening it uploads nothing.

<p align="center"><img src="assets/uploader.png" width="90%" alt="Local uploader"></p>

## Why

Your sessions are already training data under your provider's terms. This flips it: you pick which sessions to license, buyers pay per license, you get paid on every sale. What's valuable isn't the code, it's the trajectory: the plan, the corrections you made to the model, the tests, the shipped result.

| Raises value | Lowers value |
|---|---|
| Completed task with working outcome | Abandoned or trivial sessions |
| Human corrections and overrides | No verification |
| Tests, CI, verification | Duplicated or near-empty sessions |
| In-demand stacks | |

Estimates are shown before upload and are not offers. Prices are set at sale. A session can be licensed more than once and pays each time.

## Traction

- 58 stars in the first 3 days on GitHub (launched Sep 10, 2026)
- [@rishiexplainsai](https://www.instagram.com/rishiexplainsai/reel/Dc_QiLkKmmv/): 82.4K views · 320 likes · 246 comments in 4 days
- [@rishiexplainsai](https://www.instagram.com/rishiexplainsai/reel/Dc1YN1nKC95/): 69K views · 1.3K likes · 363 comments
- 20 creator videos shipped in batch 1, 200 more in production
- From the team behind [user-research-skill](https://github.com/cookiy-ai/user-research-skill) (1.5K+ stars)

<table><tr>
<td width="33%"><a href="https://www.instagram.com/rishiexplainsai/reel/Dc_QiLkKmmv/"><img src="assets/creator-rishi-82k.jpg" width="100%" alt=""></a></td>
<td width="33%"><a href="https://www.instagram.com/rishiexplainsai/reel/Dc1YN1nKC95/"><img src="assets/creator-rishi-69k.jpg" width="100%" alt=""></a></td>
<td width="33%"><a href="https://www.instagram.com/rishiexplainsai/reel/DdCMWb2KRuu/"><img src="assets/creator-rishi-5k.jpg" width="100%" alt=""></a></td>
</tr></table>

## Privacy

- Local first. Files never leave the machine until selected and confirmed.
- Redaction of secrets and PII runs on-device before upload. Review before confirming; no scrubber is perfect.
- Per-session opt-in. No background daemons. Stop the process any time.
- Open source, MIT. Read [SKILL.md](SKILL.md). Inspect the [npm package](https://www.npmjs.com/package/@cookiyai/sell-agent-sessions).

## Install

Direct:

```bash
npx @cookiyai/sell-agent-sessions
```

As an agent skill (Claude Code, Codex, Cursor, any skill-aware agent):

```bash
npx skills add cookiy-ai/sell-sessions-skill --global
```

Then say: *"I want to sell my agent sessions to earn income."* The skill installs the uploader on the host OS (not a sandbox) and keeps it running after the chat ends.

Or paste into your agent:

> Follow https://github.com/cookiy-ai/sell-sessions-skill to install the skill and start the local session uploader for me.

## FAQ

**Why would anyone pay for my sessions?** Real multi-step work with corrections and outcomes is what labs use for training and evals.

**How much?** The uploader estimates per session. Final price is set at sale. No guarantees.

**Does installing expose my data?** No. Nothing is uploaded until you select and confirm.

**When am I paid?** On each completed licensing sale, including repeat sales. Track it at [earn.cookiy.ai](https://earn.cookiy.ai/sell-sessions).

**Do I lose ownership?** No. You license selected sessions. Details in the Cookiy Earn terms.

## Star history

[![Star History Chart](assets/star-history.png)](https://www.star-history.com/#cookiy-ai/sell-sessions-skill&Date)

## License

[MIT](LICENSE) — Cookiy AI
