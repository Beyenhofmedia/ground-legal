---
title: Privacy policy
layout: default
---
# Privacy policy — Ground

**Last updated: 11 October 2026**

> **TODO(dev): before submitting to the App Store**
>
> 1. Fill in the contact address at the bottom. Apple requires a working one.
> 2. Publish this at a public URL (GitHub Pages is fine), put that URL in
>    `src/content/links.ts` and in App Store Connect. An app cannot be
>    reviewed without it.
> 3. Fill in the Privacy Nutrition Label in App Store Connect to match this
>    document. The short version is below under "What Apple's label should
>    say".
> 4. If this ever gains an account, a backup, an analytics provider, a crash
>    reporter or an advertisement, **this document is wrong** and has to be
>    rewritten before that ships. The app has an analytics seam with nothing
>    behind it (`src/data/analytics.ts`); the day a provider is installed,
>    the "No analytics" line below becomes false and must change first.

Ground is a prayer app. What people write in it is about the hardest things
in their lives, so the way it handles that is the shortest it can be: almost
nothing leaves the phone, and nothing at all is collected about who you are.

## There is no account

Ground has no sign-in, no email address, no phone number and no password.
Your subscription, if you take one, belongs to your Apple ID and is handled
by Apple; we never see who you are.

## What stays on your phone

All of it, unless it is in the next section.

- Your prayers, and anything you write about them later
- Your journal
- Your garden — every seed, every time you brought a prayer back, every
  answer, and everything you have set down on an island
- Your name, if you gave one
- Your settings, including the times you asked to be reminded

These are stored in a database inside the app on your device. They are not
backed up to us, not synced, and not readable by us. If your phone backs
itself up to iCloud or to a computer, that database goes with the backup,
under Apple's encryption and your Apple ID; we have no part in it and no
access to it. If you delete the app, they are gone from the phone.

## What leaves your phone

**One thing on its own: the messages you type to the Companion.**

When you send a message to the Companion, that message and the conversation
it belongs to are sent to a relay we run, which passes them to **Anthropic**
(the makers of Claude) to be answered. Anthropic's handling of that text is
governed by their own terms.

What is **not** sent, ever:

- Your journal
- Your garden
- Your name
- Your check-ins
- Anything identifying you or your device. One random token, made the
  first time you use the Companion and kept only on your phone, goes with
  each message so our relay can limit how many messages a day it answers.
  It names this install of the app and nothing about you; deleting
  everything in Settings, or deleting the app, discards it. To enforce the
  daily limit, our relay keeps a count of messages per token and per
  network address (stored as a one-way hash, never the address itself) for
  two days, and nothing else.

Ground does not save the conversation; closing it forgets it. Anthropic
receives the message in order to answer it and handles it under its own
terms, which may retain it for a limited time for safety purposes. Ground
cannot delete a copy Anthropic holds.

Our relay records only whether a request succeeded, how long it took, and the
name of any error. **It never records the content of a message.**

**Things you choose to send yourself.** Ground can hand things to your
phone's share sheet when you ask it to: the words of an answered prayer, a
seed link for a friend's garden, your season as a picture, or your whole
journal as a file. These go wherever you send them — a message, an email,
your files — and never to us. A seed link carries a Bible reference, the
name you typed, and your own words; it is sent by you, through an app you
choose, to a person you choose.

## Subscriptions

[REPLACE WITH ATTORNEY-REVIEWED TEXT. Facts for the drafter: if you
subscribe, the purchase is made with Apple through your Apple ID. The app
uses RevenueCat to confirm the purchase and keep the subscription in step
across your devices; to do that, RevenueCat receives the App Store receipt,
an anonymous identifier for this install, and basic device information, and
handles them under its own privacy policy (link). Neither we nor RevenueCat
receive your name, email or payment details from Apple. No purchase data is
used for advertising or shared with anyone else.]

## What we do not do

- **No account and no password.** There is nothing to remember and nothing
  for us to leak.
- **No profile.** No name, no photo, no bio, nothing about who you are.
- **No analytics.** No event tracking, no usage statistics, no session
  recording.
- **No advertising**, and no advertising identifiers.
- **No third-party SDKs that collect data for their own purposes.** The app
  contains no analytics, attribution, crash-reporting or advertising
  libraries. The subscription library is described under Subscriptions.
- **No selling or sharing of data.** There is nothing to sell.
- **No location, contacts, photos, microphone or health data.** The app does
  not ask for them and cannot read them.
- **Your prayers are never held behind a payment.** When the free trial
  ends the app needs a subscription to open, but from that screen you can
  save every prayer to a file or delete them all, without paying, and the
  crisis line stays open.

## Notifications

If you turn reminders on, they are scheduled on your phone by your phone.
They contain the same words every day and never mention what you have
written or how many days you have missed. No notification server is involved.

## Deleting everything

Settings → *Delete everything*. It removes every prayer, every journal entry
and the whole garden from the device, immediately and permanently. There is
nothing held elsewhere for us to delete, and no way to undo it.

You can also take your journal with you first: Settings → export.

## Children

Ground is not directed at children. It is intended for people aged 13 and
over. We do not knowingly collect anything from anyone, of any age, because
we do not collect anything.

## The Companion is not a counsellor

The Companion is an AI. It is not a pastor, a counsellor, a therapist or a
person, and it cannot help in an emergency. If you are in danger, call your
local emergency number. In the United States, the 988 Suicide & Crisis
Lifeline can be reached by calling or texting 988.

## Your rights

Everything you write stays on your phone, so the only copy of it is yours and
you control it completely: Settings holds both the export and the delete.

We hold nothing about you. If you believe otherwise, write to the address
below and we will look.

## Changes

If this policy changes, the date at the top changes with it. A change that
means more data leaves the phone will be put in front of you in the app
before it takes effect, not published quietly here.

## What Apple's label should say

Three things to declare, all *Used for App Functionality*, **not** linked to
the user's identity, **not** used for tracking:

- **Other User Content** — the Companion message text, sent to be answered
  and not retained by us.
- **Identifiers → User ID** — the random per-install token sent with each
  Companion message so the relay can count messages.
- **Purchases → Purchase History** — the App Store receipt that RevenueCat
  checks to confirm a subscription. Declare this only once subscriptions
  are switched on.

Declare no contact info, no usage data, no diagnostics, no advertising
identifiers, no location, and no tracking of any kind.

## Contact

[REPLACE WITH ATTORNEY-REVIEWED TEXT: a monitored contact address for
privacy questions and requests.]
