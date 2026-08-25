# acro-catalog

**Generated. Do not edit by hand.** Every commit here is written by
[acro-docs](https://github.com/acronym-lol/acro-docs) CI.

`showcase.json` is the public list of Acronym tools, and this repo exists so it can be
fetched **without a credential**:

```
https://raw.githubusercontent.com/acronym-lol/acro-catalog/main/showcase.json
```

## What is in it

Only tools whose repo declares `visibility: public` in its `docs/_meta.yml`, and only
the fields a public page needs: name, summary, category, status, public links, and
showcase metadata.

Deliberately **not** here: internal tools, owner and maintainer handles, support tier,
dependency and hardware lists, documentation freshness, and internal links such as
runbooks, dashboards and Slack channels. Narrowing happens in the producer, so a mistake
by a consumer cannot expose any of it.

Schema: `showcase.schema.json` on the docs site. Check `schema_version` and refuse to
build on a value you do not recognise rather than crashing mid-render.

## Why the history matters

Publication here is **irreversible** — a public git history is permanent, and deleting a
tool later removes it from the tip, not from the past. So the commit log of this repo is
the record of what has ever been public, and each commit message names the tools that
became public in it. That is deliberate: it is the audit trail for a field
(`visibility`) whose effect is otherwise invisible to the person setting it.
