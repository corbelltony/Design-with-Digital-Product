# Cheddar Hub | Verified changelog

This is an index of documented history, not a claim of a new installation. See the [full cyberpunk changelog PDF](changelog.pdf) for detail and source references.

## Added
- **October 8, 2026:** Flask dashboard foundation, system monitoring, weather integrations. Git commits `a031240`, `502dc62`, `eec70bd`.
- **October 10, 2026:** Native Clock with timers, alarms and reminders; project commit `83f5184` includes this development.
- **November 13, 2026:** Basic Voice v1 supporting “Hey Cheddar” and limited commands via local Vosk and Piper, BY Y02 microphone, WM8960 output. Release `cheddar-voice-basic-v1-20261113`.

## Improved
- **October 23, 2026:** Three-page Home/Media/System cyberpunk dashboard; touchscreen layouts and navigation. Dashboard 2.0 / 2.0.1, with 800 × 480 browser checks and owner touchscreen acceptance.
- **November 13, 2026:** Voice speaker profile adjusted from −20 dB DAC attenuation to 0 dB with owner acceptance; restoration on voice-service restart validated.

## Fixed
- **October 23, 2026:** Controller V1 `unapproved_http_route` false rejection fixed in V2 and retested offline.
- **October 23, 2026:** Stale Media layout in existing Chromium tab resolved by an operator-triggered hard refresh; not proof of a cache-specific root cause.

## Known issues / limits
- Dashboard freeze history; a fresh long-duration stability proof is not included.
- Voice response time and recognition repeatability are not controlled-benchmark claims.
- Full cold boot for Voice v1 is not documented by the finalization record.
- The voice assistant supports a **limited command set**, not open-ended smart-home control or unrestricted AI conversation.

See [source references](source/README.md) and [repeatable update prompt](changelog-update-prompt.md).
