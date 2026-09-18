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
