# Cheddar Hub | Real tests and evidence

Read the [complete cyberpunk test report (PDF)](test-report.pdf) for the visual evidence, full procedures, outcomes, and limitations. [Evidence index](evidence/evidence-index.csv) provides filenames and source timecodes.

## 01 · Physical touchscreen navigation — historical PASS

- **Setup:** Raspberry Pi 4, 5-inch Elecrow 800 × 480 display, Chromium kiosk. Dashboard 2.0/2.0.1; deployment ID `cyberpunk-dashboard-e8f29aea05c8`.
- **Steps:** Open Home; switch to Media; open System; navigate back to Home.
- **Expected:** Correct page content and functional navigation appear on the live touchscreen.
- **Actual:** The owner reported seven physical touchscreen acceptance checks passed on October 23, 2026. November 17 footage shows the Home, Media, and System pages. Footage does not independently prove each individual tap.
- **Evidence:** `evidence/videos/Touchscreen_Home_Media_System_Nov17_FULL.mp4` and the dated authentic screenshots.

## 02 · Supported hands-free voice request — historical PASS

- **Setup:** Same Pi; BY Y02 USB microphone; Vosk local recognition, Piper speech, WM8960 speaker HAT. Release `cheddar-voice-basic-v1-20261113`.
- **Steps:** Check listener; say “Hey Cheddar, what time is it?”; listen for spoken answer.
- **Expected:** The supported request is processed and a time answer is spoken.
- **Actual:** November 13 owner acceptance records confirm an ordinary-volume request and audible answer. November 17 recording supplies a subsequent live demonstration. No controlled response-time benchmark was performed.
- **Evidence:** `evidence/videos/Hands_Free_Voice_Nov17_00-02min_ORIGINAL_AUDIO.mp4`; matching stills and the source-linked Voice v1 journals.

## Before and after (two distinct comparisons)

**User-facing modes:** Home-screen readout versus supported spoken time query. The two recordings differ in conditions; they **do not establish faster interaction**.

**Technical audio repair:** WM8960 DAC Playback Volume was observed at **−20 dB** (raw 215/215) before controlled adjustment, then **0 dB** (255/255) with owner-accepted clean spoken output. These are mixer readbacks, not sound-pressure measurements or matched recordings.

**Offline regression:** Earlier Dashboard deployment controller V1 rejected legitimate CSS/JS paths with `unapproved_http_route`; controller V2 derived an allowlist from validated release files and passed offline acceptance. The live Pi was not downgraded to recreate that failure.

## Limits

These are **documented historical tests**; preparation of this submission was not a fresh physical acceptance run. The full Pi cold boot, repeated response-time measurements, and general conversation capabilities remain unverified or out of scope. The source repository may require additional access for an instructor; local evidence and full report are included here.
