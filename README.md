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
| `mittari/` | privacy policy URL (11 locales), support URL (11), marketing URL (6), 1.1 | Mittari 1.2 |

`mittari/privacy.html` is the one to be careful with: it is the privacy
policy link on a live listing in eleven languages. Do not remove it
before Mittari's next version is approved.

`404.html` redirects any other old path — `/sikku/...`, `/tulos/...`, a
deep link nobody wrote down — to the matching subdomain, so the removed
folders still lead somewhere for an old build or a stale bookmark.
