# harmony-tts

**Harmony TTS — Sovereign Formant Synthesis Engine**  
Harmony Labs · Klatt-style real-time voice generation · Kyle S. Whitlock

---

## Status: v92 Prototype (Browser-Based Formant Lab)

Two browser-based implementations of the Harmony formant synthesis engine are included:

- `formant_lab.html` — Full G2P + formant synthesis lab (44KB, most complete)
- `formant_lab_v92.html` — Version 92 stable build (32KB)

Both are zero-dependency HTML files. Open in any modern browser to run the synthesis lab.

---

## Architecture

Harmony TTS uses Klatt-style formant synthesis — the same approach used in classic speech synthesis research, enhanced with CC-governed phoneme selection:

1. **G2P (Grapheme-to-Phoneme)** — Text → phoneme sequence
2. **Formant synthesis** — Phoneme → acoustic formant parameters
3. **CC gating** — Synthesized output scored through CC v1 before playback
4. **Real-time rendering** — Web Audio API for zero-latency output

---

## Roadmap

| Phase | Status |
|-------|--------|
| v1 — Browser formant lab | ✓ Complete |
| v92 — Stable synthesis build | ✓ Complete (this repo) |
| v3 — Python backend synthesis | 🔧 Handoff (see HANDOFF_NOTES.md) |
| v4 — Harmony Chip native audio | 📋 Planned |

---

*Part of Harmony Labs sovereign AI stack · See: `harmony-llm`, `Resonance-Calculus`*
