# Sources and coverage

## Interview extension on 21 November 2026

Primary source: NetworkChuck, How to Actually Code with AI (ft. Matt Pocock), published 20 November 2026, https://www.youtube.com/watch?v=mU8WKII1gpk . The full English captions and publisher metadata were retrieved; the analysis was not a frame-by-frame visual audit.

- Shared terminology and ADRs: https://www.youtube.com/watch?v=mU8WKII1gpk&t=1204s
- Context, specifications, and task-sized sessions: https://www.youtube.com/watch?v=mU8WKII1gpk&t=1551s
- Model effort as a deliberate choice: https://www.youtube.com/watch?v=mU8WKII1gpk&t=1813s
- Worktrees, delegation, and two-axis review: https://www.youtube.com/watch?v=mU8WKII1gpk&t=2088s
- Evidence and risk-based trust: https://www.youtube.com/watch?v=mU8WKII1gpk&t=2440s
- Deep modules and behavioral checks: https://www.youtube.com/watch?v=mU8WKII1gpk&t=3309s
- Deterministic delivery: https://www.youtube.com/watch?v=mU8WKII1gpk&t=5061s

The portability adapters and task templates are synthesis. Spec Kit, the cumulative 10-attempt cap and the architecture/refactor rule are the author's own choices, not Matt Pocock's. The interview's model preferences and context comfort point are observations, not universal settings. Harness behavior sources are in harnesses.md. The official package remains the source for its engineering procedures; this coordinating skill is the author's own.

## Earlier source review

Reviewed November 12, 2026. This skill synthesizes Matt Pocock's public teaching. The Spec Kit mapping and the cumulative ten-attempt cap are the author's own additions.

| Decision | Evidence |
| --- | --- |
| Start agents in a home checkout, preserve local instructions and add navigation pointers | [The exact X post in the screenshot](https://x.com/mattpocockuk/status/2120847219788308872), [earlier Home Repo post](https://x.com/mattpocockuk/status/2120260969750540327), [Matt's setup procedure and FAQ](https://www.aihero.dev/the-home-repo-pattern) |
| Size the planning effort to the diff and introduce a decision map only when needed | [October 8 X post](https://x.com/mattpocockuk/status/2108216899439894574) |
| Use consistent domain language when describing a business process | [Matt's reply on domain modeling](https://x.com/mattpocockuk/status/2120606575819956439) |
| Build trustworthy feedback before increasing unattended throughput | [Software factory post](https://x.com/mattpocockuk/status/2115538750147023323), [Matt's Ralph workshop](https://www.aihero.dev/workshops/day-5-ralph-dj2dh) |
| Capture visual evidence in a PR | [Matt's watch app example](https://x.com/mattpocockuk/status/2116172513801863211) |
| Carry an idea from interview through vertical tickets, implementation and QA | [Worked feature](https://www.aihero.dev/real-world-feature-build-with-claude-code), [official skills guide](https://www.aihero.dev/skills), [upstream repository](https://github.com/mattpocock/skills) |

These links are a selection of Matt Pocock's public posts, not a complete review of his account.

## Further resources named in the interview

Checked against the full transcript (00:00:00 to 02:02:29), not a visual rewatch.

- AI Coding Dictionary and its GitHub source: 48:33–49:23; repeated 1:44:45.
  https://www.aihero.dev/ai-coding-dictionary
  https://github.com/mattpocock/dictionary-of-ai-coding
- Retro: 42:31–42:48 and 51:05–52:28; review batches at 1:03:03.
- Improve Codebase Architecture: 56:59 and 1:01:28; Teach: 1:08:42.
- Sandcastle: 1:27:10; Evalite: 1:27:31; Course Video Manager source: 1:49:51.
- Additional recommended books: The Pragmatic Programmer, Refactoring and
  Extreme Programming at 1:38:00–1:38:14, alongside the earlier Ousterhout,
  Evans and Feathers recommendations.
- Contribution evidence: 1:29:46; check speed/CI sharding: 1:38:51;
  product attention and QA: 1:41:53.

Spec Kit and bounded loops are the author's adaptations, not part of Matt Pocock's skills.
