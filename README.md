## Pin convention for stakwork forks

- Projects on remote `stakwork` are pinned to immutable lightweight tags named `<upstream release tag>-peel<N>` (e.g. `2026111800-peel1` = GrapheneOS release `2026111800` plus Peel patches).
- A project with no Peel patches stays on the plain upstream tag (`refs/tags/2026111800`).
- `vendor/peel` is pinned to a full commit SHA with `upstream="refs/heads/17"`.
- Tags are never moved or deleted. A new Peel change means a new `-peel<N+1>` tag and a manifest bump PR.
- Branch `17` is a pure upstream mirror; `peel/17` is the custom branch.
