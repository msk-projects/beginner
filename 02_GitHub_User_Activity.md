---

# 2. GitHub User Activity (Beginner)

**🎯 Overview**
Create a CLI tool to fetch and display **GitHub user activity** using the GitHub API. Supports caching to avoid repeated API calls.

**✅ Features / Requirements**

* Fetch user **events, repos, and stats** (stars, forks, top languages)
* Use `--token` for authenticated requests (optional, via env `GITHUB_TOKEN`)
* Cache responses locally (JSON) with TTL (e.g., 5–10 minutes)
* Display data in a **human-readable table**
* Handle errors like user not found or API limit exceeded

**💻 Example CLI Commands**

```bash
gh-activity events MrSumitKumar --limit 20
gh-activity repos MrSumitKumar --sort stars --limit 10
GITHUB_TOKEN=*** gh-activity stats MrSumitKumar --top-langs 5
```

**🗂️ JSON Cache Structure**

```json
{
  "cachedAt": "2025-09-03T06:00:00Z",
  "username": "MrSumitKumar",
  "events": [
    { "type": "PushEvent", "repo": "example-repo", "timestamp": "2025-09-03T06:00:00Z" }
  ]
}
```

**🚀 Getting Started**

1. Implement HTTP client with retries and error handling
2. Parse CLI arguments (`events`, `repos`, `stats`)
3. Add caching layer with TTL and `--no-cache` option
4. Format output in readable tables
5. Test with valid and invalid usernames

---
