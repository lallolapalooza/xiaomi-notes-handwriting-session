# Xiaomi Notes Handwriting Session Archive

Session archive for the MIUI Notes handwriting-stack investigation.

## Contents

- `xiaomi-notes-session-archive.zip` — full session transcript, standalone HTML viewer, agent/job state, and untruncated tool logs.

The archive does not contain the APK, extracted native libraries, or model files. Those are proprietary Xiaomi/Sunia/ASA/KSP assets and remain only in the local session bundle.

## Open the archive

```bash
unzip xiaomi-notes-session-archive.zip -d session
xdg-open session/viewer.html
```

Or inspect the raw transcript:

```bash
unzip -p xiaomi-notes-session-archive.zip session.jsonl | less
```

## Archive SHA-256

```text
ab625249e41df83d841f7116ca802577eb07666a6b828e4f5d5ae892d0f7c35a
```

## Context

The investigation covers:

- `com.miui.notes` 7.8.6 (versionCode 786), Poco F4 global ROM
- Bundled Sunia handwriting recognition models for Chinese and English
- Sunia/KSP native recognition libraries and ASA path estimation
- The tablet/non-international device gate that disables recognition on this phone
- `.ent` handwritten-note format and Notes database integration
- ASA license layer and Xiaomi APK signing
- Clean-room reimplementation options using ML Kit Digital Ink Recognition

## Notice

The session transcript may contain local filesystem paths and analysis notes. No proprietary binaries or model files are included. Do not redistribute Xiaomi/Sunia/ASA/KSP binaries or models.
