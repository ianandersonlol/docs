# Ian's Docs (Mintlify)

This repository contains documentation for bioinformatics, HPC, protein engineering, and lab workflows.

## Local Development

1. Install the Mintlify CLI:

```bash
npm i -g mint
```

2. Run the local docs server from the repo root:

```bash
mint dev
```

3. Open `http://localhost:3000`.

## Repository Structure

- `docs.json`: Mintlify site config and navigation.
- `index.mdx`: Homepage.
- `hpc/`: General SLURM docs plus UC Davis HIVE and Stanford Sherlock guides.
- `protein-engineering/`: Structure prediction, design, and docking workflows.
- `genomics/`: Genomics section.
- `misc-bioinfo/`: Miscellaneous guides including Mac setup and ordering workflows.
- `images/`: Shared image assets used by docs pages.
- `changelog.mdx`: Human-readable changelog for notable docs updates.

## Authoring Conventions

- Use frontmatter (`title`, `description`, and optional `icon`, `toc`, `mode`) on each page.
- Keep examples copy-pasteable and avoid user-specific values unless explicitly labeled.
- Prefer placeholders like `YOUR_USERNAME`, `your_account`, and `JOBID` for commands.
- Use section overview pages (`index.mdx`) with cards to route readers to detailed pages.
- Add changelog entries for meaningful reader-facing documentation changes.

## Pre-PR Checklist

- Run `mint dev` and click through edited pages.
- Verify internal links and image paths.
- Confirm commands are accurate and safe (especially anything destructive).
- Check for stale placeholders (`TODO`, `placeholder`, outdated hostnames, and unintended personal usernames).

## Deployment

Docs are deployed via Mintlify/GitHub integration when changes are pushed to the default branch.

## Useful Links

- [Mintlify docs](https://mintlify.com/docs)
- [Site repository](https://github.com/ianandersonlol/docs)
