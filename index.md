---
title: Tiktoklizando
---

# Tiktoklizando

A personal desktop application that schedules and publishes its owner's own
travel videos to their own TikTok account.

It runs locally on one computer. There is no server, no database and no
analytics. It does not collect anyone's data, and it publishes nothing without
the owner reviewing the caption and the privacy settings for that specific
video first.

* [Privacy Policy](privacy.md)
* [Terms of Service](terms.md)

---

### How it works

1. The owner connects their own TikTok account through TikTok's official OAuth
   flow, with PKCE. The resulting token is stored only on that computer.
2. The owner picks a video from their own disk and writes a caption.
3. Before publishing, the application shows which account will receive the
   video and asks the owner to choose who can watch it and whether comments,
   Duet and Stitch are allowed. Nothing is pre-selected.
4. The video is uploaded through TikTok's Content Posting API.

### Permissions it asks for

| Scope | Why |
|---|---|
| `user.info.basic` | To show which account is about to receive the post |
| `video.upload` | To send the owner's video file to TikTok |
| `video.publish` | To publish it with the caption and settings the owner chose |

Nothing else is requested, and no other account is ever touched.

<small>Not affiliated with, endorsed by or sponsored by TikTok or ByteDance.</small>
