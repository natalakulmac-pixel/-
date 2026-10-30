---
name: instagram-browser-risk
description: "Logging into Instagram in the built-in browser got the user's account suspended (selfie check) on 2026-10-08"
metadata:
  node_type: memory
  type: feedback
  originSessionId: 7f27dc96-4c55-4e15-920a-d709c123d81b
  modified: 2026-10-08T14:30:14.835Z
---

On 2026-10-08 the user logged into Instagram in the built-in browser pane so I could read reel view counts for /ig-viral. Instagram immediately redirected to accounts/suspended and demanded a selfie; the user filed an appeal. Earlier that day I had paged through several carousels in that same browser while logged out (JS clicking "Далее", collecting image URLs).

**Why:** a new-device login plus scripted carousel browsing likely looked automated; a suspended account risks permanent disablement for the user's (or Vasiliy's) work profile.

**How to apply:** do not ask the user to log into Instagram in the built-in browser again. For competitor research use what's visible logged-out (single post pages), screenshots/links the user sends from their phone, or YouTube Shorts. Keep logged-out Instagram browsing minimal and human-paced. See [[vasiliy-alekseev-instagram]].
