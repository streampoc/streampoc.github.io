# streampoc.github.io

Developer site for **AuraGames**, required by Google Play and AdMob.
Served at <https://streampoc.github.io>.

| Path | Purpose |
|---|---|
| `index.html` | Developer website listed on Play |
| `sort-reveal/privacy/index.html` | Privacy policy for Sort &amp; Reveal |
| `app-ads.txt` | AdMob ownership record. **Must stay at the domain root** |
| `.nojekyll` | Serve files as-is, without Jekyll processing |

## Don't move these URLs

`https://streampoc.github.io/sort-reveal/privacy` is compiled into shipped
Android builds (`lib/config/app_info.dart` in the app repo) and is filed with
Play and AdMob. Changing the path breaks released apps.

## Editing the policy

The Markdown source of record lives in the app repo at `store/privacy_policy.md`,
and the app repo's `site/` folder mirrors this one. Update both together, and
bump the "Last updated" date.
