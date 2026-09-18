# dresende.github.io

Redirects for App Store listing fields that still point here.

Each app's site moved from `dresende.github.io/<app>/` to
`<app>.dresende.pt`, and the old project repositories are gone. Most of
those URLs could simply be dropped — but a listing field cannot be edited
once its version is live. Apple answers:

    409 The field 'privacyPolicyUrl' can not be modified in the current state

So a field keeps pointing here until its app ships a next version, at
which point that app's metadata push corrects it and the folder can be
deleted.

**A folder here means an App Store field still points at it.** That is
the whole index — `ls` is the status report. As of 18 September it
reports nothing: there are no folders left.

Mittari was the first to go, and the reason this repository exists at
all: its privacy policy link, in eleven languages, pointed here. 1.2 went
live on 15 September carrying the corrected URLs, so its folder is gone.
Kirjo followed on 18 September — 1.1 shipped on both iOS and tvOS with
the marketing URL corrected in all twelve locales. Helmi went the same
day, and was the last: 1.1 went live carrying
`https://helmi.dresende.pt` as the marketing URL in all twelve locales.

The repository stays, empty of folders. `404.html` still redirects any
old path — `/helmi/...`, `/sikku/...`, a deep link nobody wrote down — to
the matching subdomain, so a stale bookmark or a build installed before
the move still lands somewhere. And the next listing field that gets
stranded has a place to point while it waits for its version.

## When this can be retired

One thing keeps it alive, and it is not a listing field: **Mittari 1.0
and 1.1 have `https://dresende.github.io/mittari/` compiled into their
About screen.** The move to `mittari.dresende.pt` was commit `0d03a6c`
on 28 August; 1.0's build was uploaded on the 18th and 1.1's on the
21st, both before it. A URL inside a shipped binary cannot be changed
for someone who never updates, and it is the privacy policy link, which
is the one link Apple requires.

Every other app is clear, checked rather than assumed:

- **Helmi** 1.0 shipped build 61 with `helmi.dresende.pt` already in it.
- **Kirjo** 1.0 iOS is build 51, and the commit that moved the URL is
  commit count 51 — the same commit, so it was built from it, not
  before it. tvOS is build 57, later still.
- **Tulos** carried it between 20 and 28 August, but 1.0 was never
  approved, so no copy of it exists on anyone's device.
- **Sikku, Cruzadas, Talo, Pilvi, Roihu** never had it in their sources.

Helmi's and Kirjo's 1.0 *version records* still name this domain in
their marketing URL and always will — Apple will not edit a released
version — but the store shows only the current version, so nobody
follows them.

**How to know when it is over.** Every forward from `404.html` carries
`?from=legacy-redirect`, so traffic arriving at `mittari.dresende.pt`
with that marker is exactly the population this repository exists for:
someone on an old build who tapped Privacy. Apple cannot answer this —
its analytics suppress small segments, and the Analytics Reports API is
not retroactive, so it would only describe the future anyway.

The marker undercounts, and only in the safe direction: a person has to
actually tap the link to appear. So when it reads zero over a long
enough window, the real number is at most that — and this repository has
finished.
