# grin-media

Pictures and narration for [nemilya/grin](https://github.com/nemilya/grin) — Alexander Grin's stories read aloud
and staged on screen ([grin.nemilya.me](https://grin.nemilya.me)).

This repository holds only binary media, at the same paths as in the code repository (`stories/<story>/…`):
cut-outs and sets (`assets/**/*.webp`, lossless WebP with alpha), character sheets (`assets/refs/*.jpg`) and
narration takes (`voicings/<voice>/takes/*.opus`). Everything else — texts, translations, bibles, storyboards,
manifests, the engine — is in `grin`. Each `grin` commit pins the media commit it was made with in `media.rev`.

Don't clone this repository on its own; from a `grin` checkout:

```bash
make media-pull     # lays out the media of media.rev into stories/ (git dir: .media.git)
make media-push     # after generating: commit and push changed media, update media.rev
```

How the two repositories work together — [docs/media.md](https://github.com/nemilya/grin/blob/main/docs/media.md)
(по-русски — [docs/media.ru.md](https://github.com/nemilya/grin/blob/main/docs/media.ru.md)).

## License

All media here were generated for the project (images — Seedream, narration — Gemini TTS) and are dedicated to
the public domain: [CC0 1.0](LICENSE). The stories themselves are by Alexander Grin (1880–1932), public domain.

---

Картинки и озвучка для [nemilya/grin](https://github.com/nemilya/grin): те же пути, что в основном репозитории;
скачивать — `make media-pull` из `grin`. Всё — общественное достояние (CC0 1.0).
