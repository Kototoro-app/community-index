# Kototoro community index

Static index of Kototoro's community ratings and comments, built from public Nostr events.

- `main`: the workflow (`.github/workflows/build-index.yml`) that builds the index every six hours.
- `archive`: every Kototoro event the indexer has seen, as `events/<yyyy-MM>.jsonl.gz`.
- `gh-pages`: the latest snapshot the app downloads (`v1/manifest.json` and the files it lists).

Nothing here is authoritative: the events live on public relays, the archive is a copy of them, and the snapshot is
derived from the archive. The indexer's code and the rules it applies are in
[Kototoro/community-indexer](https://github.com/Kototoro-app/Kototoro/tree/devel/community-indexer); the design is in
[docs/architecture/community-nostr-plan-2026-11.md](https://github.com/Kototoro-app/Kototoro/blob/devel/docs/architecture/community-nostr-plan-2026-11.md).
