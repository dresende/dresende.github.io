# dresende.github.io

Redirects for App Store listing fields that still point here.

Each app's site moved from `dresende.github.io/<app>/` to
`<app>.dresende.pt`, and the old project repositories are gone. Most of
those URLs could simply be dropped — but a listing field cannot be edited
once its version is live. Apple answers:

    409 The field 'privacyPolicyUrl' can not be modified in the current state

So the fields below keep pointing here until each app ships its next
version, at which point its metadata push corrects them and the folder
can be deleted.

**A folder here means an App Store field still points at it.** That is
the whole index — `ls` is the status report.

| Folder | Still named by | Cleared when |
| --- | --- | --- |
| `kirjo/` | marketing URL, en-US, iOS **and** tvOS 1.0 | Kirjo 1.1 |
| `helmi/` | marketing URL, en-US, 1.0 | Helmi 1.1 |

Mittari was the third, and the reason this repository exists at all: its
privacy policy link, in eleven languages, pointed here. 1.2 went live on
15 September carrying the corrected URLs, so its folder is gone — which
is how each of these ends.

`404.html` redirects any other old path — `/sikku/...`, `/tulos/...`, a
deep link nobody wrote down — to the matching subdomain, so the removed
folders still lead somewhere for an old build or a stale bookmark.
