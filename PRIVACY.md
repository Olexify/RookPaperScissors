# Privacy

*Last updated 10 September 2026*

The canonical version of this document lives at
**<https://rookpaperscissors.com/privacy.html>**. This copy is here for reference.

You can play the whole game without telling us anything at all. If you choose to sign in, we keep
the smallest thing that lets your army follow you to another browser — and not one field more.

**The short version.** No cookies. No advertising. No analytics. No tracking. Nothing is sold or
shared with anybody who is not needed to run the game. If you never sign in, nothing you do leaves
your own browser except the moves in an online game.

## Who we are

Rook, Paper, Scissors! is a browser game run by an independent developer. For anything in this
document, write to <support@olexify.dev>.

## What stays in your browser

Most of the game is stored on your own device, in your browser's `localStorage`. We cannot read
it, and it is never sent anywhere unless you sign in. It holds:

- your settings — sound, theme, board size, house rules;
- an **anonymous identity**: a random id, a private token, and a made-up name such as
  "Gambit #4821", invented on your first visit;
- your record — games played, won, lost, streaks and badges;
- your army, the names your pieces have earned, and the hats they wear;
- your vault — gold, keys and chests;
- how far you have got in the campaign.

**We use no cookies** — not for the game, not for sign-in, not for anything. Clearing your browser
data deletes all of the above, permanently, unless you were signed in.

## What reaches the server

The game runs on Cloudflare. The only things kept on the server are these:

| What | When it is written | How long it is kept |
|---|---|---|
| **The ledger** — your id, display name, rating, wins, losses, draws, streak and when you were last seen | when you play a game against another person online, including as a guest | until you ask us to delete it |
| **A session** — a random token, your account id, display name and which provider you used | when you sign in | 60 days, then deleted automatically; sooner if you sign out |
| **Your profile** — the army, vault, campaign and record described above | only while you are signed in | until you ask us to delete it |
| **A sign-in link** — your email address and a single-use code | when you ask for an email sign-in link | **15 minutes**, or until the link is opened, whichever is sooner |
| **An anti-abuse note** — your IP address and your email address, with a timestamp | when you ask for an email sign-in link, to stop a robot asking ten thousand times | **one hour**, then deleted automatically |

### About your email address

If you sign in by email, we deliberately do not keep the address. Your account is identified by a
**one-way cryptographic digest** of it — a fixed-length string that cannot be turned back into your
address. The address itself exists only in the sign-in link row above, for at most fifteen
minutes. Your display name is taken from the part before the `@`.

There is no password. There is nothing to reset, nothing to reuse on another site, and nothing
worth stealing.

### If you sign in with Google or Twitch

We ask that provider for two things only: **an account identifier and a display name**. We do not
ask for, receive or store your email address, your contacts, your videos, your followers or
anything else. From Google we request the scopes `openid` and `profile`, and nothing more.

## Who else is involved

Running the game means a small number of other companies see some data. There are no others.

- **Cloudflare** — hosts the game and stores everything in the table above. As the host,
  Cloudflare processes your IP address to deliver the page.
- **Cloudflare Turnstile** — the "are you a robot" check in front of the email sign-in form. It
  runs only on that form.
- **Resend** — delivers the sign-in email. They see your address in order to deliver it.
- **Google** — only if you press "Sign in with Google". Separately, the game loads its typefaces
  from Google Fonts, which means Google's servers see your IP address on every visit, as they do
  on a great many websites.
- **Twitch** — only if you press "Sign in with Twitch", or if you use the play-with-chat feature,
  which connects to Twitch chat *anonymously*: we do not log in as you and we do not read anything
  but the votes in the channel you name.

## What we do not do

- No advertising, and no advertising identifiers.
- No analytics, no telemetry, no session recording, no heat maps.
- No cookies, and no tracking pixels.
- No selling, renting or sharing of anything, to anyone, ever.
- No profiling and no automated decisions about you.
- No location data beyond the country your IP implies to our host.

## Why we are allowed to keep it

Under the GDPR, and for anyone else who asks: the ledger, the session and the profile are kept to
**perform the service you asked for** — a game that remembers you. The anti-abuse note is kept
under our **legitimate interest** in not having our mail service used by robots. That is the whole
legal basis, because that is all the data there is.

## Your rights

You may ask us to show you, correct, export or delete everything we hold. Write to
<support@olexify.dev> from the address you signed in with, or tell us your display name if
you signed in with Google or Twitch, and we will do it within thirty days and usually the same
week. Deleting your profile removes the army, the vault, the campaign, the record and the
sessions. It cannot be undone.

Signing out, on its own, deletes nothing on the server — it only stops this browser from speaking
to it. Say the word "delete" if that is what you want.

If you are in the EU or the UK you also have the right to complain to your national data
protection authority.

## Children

The game is not directed at children under 13, and we do not knowingly keep data from them. If you
are under the age at which your country lets you agree to this on your own — 13 in most places, 16
in some of the EU — please ask a parent or guardian first. If you believe a child has signed in,
write to us and we will delete the account.

## Where the data lives

On Cloudflare's network, which is global; the data may be processed in a country other than your
own. Cloudflare's terms provide the safeguards required for transfers out of the EU and UK.

## Security, honestly

Everything travels over HTTPS. There is no password to leak, no card number anywhere near the
game, and your email address is kept for fifteen minutes rather than for ever. That said, this is
a game made by one person: we cannot promise a system nobody could ever break into, and we would
rather say so than pretend otherwise. Do not put anything in your display name you would not want
a stranger to read.

## When this changes

If we ever collect something new, this page changes first and the date at the top changes with it.
A change that materially affects you will be announced in the game before it takes effect.
