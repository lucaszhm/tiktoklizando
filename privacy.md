---
title: Privacy Policy
---

# Privacy Policy

**ViajanteUp**
Last updated: 10 October 2026

## In short

ViajanteUp is a personal desktop application that runs on its owner's own
computer. It has no server, no database and no analytics. It does not collect,
transmit or sell anyone's data. It posts the owner's own videos to the owner's
own TikTok account, and nothing else.

## Who runs this application

ViajanteUp is built and used by a single creator to publish their own travel
videos to their own TikTok account. It is not offered as a service to other
people and has no other users.

## What the application stores, and where

Everything the application stores is written to the folder it runs from, on the
owner's computer. Nothing is uploaded anywhere except to TikTok's own API.

| What | Why | Where |
|---|---|---|
| TikTok access and refresh tokens | To post on the owner's behalf without logging in every time | A local file on the owner's computer |
| Video files | They are the content being published | The owner's own disk |
| Captions, dates and upload status | So the application knows what to post and when | A local spreadsheet file |

The access token is obtained through TikTok's official OAuth flow, with PKCE,
and is never sent to any party other than TikTok.

## What the application does NOT do

* It does not collect data about any TikTok user, including the owner's
  followers, viewers or commenters.
* It does not read, store or process other people's content.
* It does not send any information to the developer or to any third party.
* It does not use cookies, trackers or advertising identifiers.
* It has no server component, so there is nothing to breach remotely.

## Information received from TikTok

When the account is connected, the application requests only the permissions it
needs to do its job:

* `user.info.basic` — to show which account is about to receive a post, which
  TikTok requires before publishing.
* `video.upload` and `video.publish` — to upload and publish the owner's own
  videos.

The basic profile information returned (display name, avatar, open id) is held
in memory while the application is open and is used only to show the account
name on screen. It is not written to disk and not transmitted anywhere.

## Retention and deletion

Because all data is local, deleting it is entirely under the owner's control:
deleting the token file disconnects the TikTok account, and deleting the
application folder removes everything the application ever stored.

The TikTok connection can also be revoked at any time from TikTok's own
settings, under *Manage app permissions*. Revoking there immediately stops the
application from being able to post.

## Children

The application is a personal publishing tool and is not directed at children.

## Changes

If this policy changes, the new version is published on this page with an
updated date.

## Contact

Questions about this policy can be sent to the repository that hosts this page:
<https://github.com/lucaszhm/viajanteup>
