# Production links and UTM scheme

Production landing domain:

```text
https://www.openclawlaunchkit.site
```

Payment backend used by the landing:

```text
https://openclaw-launch-kit-backend.onrender.com
```

## Files that now contain production landing links

```text
README.md
paid-kit-preview/whats-inside.md
paid-kit-preview/free-vs-paid.md
```

## Current UTM scheme

GitHub README / free repo links:

```text
utm_source=github
utm_medium=free_repo
utm_campaign=openclaw_starter_free
```

Paid-kit preview links:

```text
utm_source=github
utm_medium=paid_kit_preview
utm_campaign=openclaw_starter_free
```

Free vs paid page links:

```text
utm_source=github
utm_medium=free_vs_paid
utm_campaign=openclaw_starter_free
```

## Notes

- Keep UTMs when editing links.
- If a custom domain is added later, replace only the domain and preserve the path/query strings.
- `sitemap.xml` and `robots.txt` in the landing folder also use this Vercel domain.
