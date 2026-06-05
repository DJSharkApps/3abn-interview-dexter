# 3ABN Interview Materials

**Public** repository for **3ABN interview** video files. Anyone can download — **no GitHub account** required.

## Contents

Interview MP4 files live in the `videos/` folder. Large files are stored with **Git LFS** (see below).

## For maintainers (uploading videos)

1. Install [Git LFS](https://git-lfs.com/) (recommended for MP4s; required for files over GitHub’s ~100 MB per-file limit).
2. Copy your `.mp4` files into `videos/`.
3. Commit and push:

```bash
cd /path/to/3abn-interview-dexter
git lfs install   # once per machine
git add videos/*.mp4
git commit -m "Add interview videos"
git push origin main
```

On this Mac, the local clone is at `/Users/djshark12/GitHub/3abn-interview-dexter`.

## For Dexter (and anyone) — downloading without an account

**Option A — Direct links on GitHub**

1. Open https://github.com/DJSharkApps/3abn-interview-dexter
2. Go to `videos/`, open each `.mp4`, and click **Download**.

**Option B — Download ZIP**

1. On the repo page, click **Code → Download ZIP**
2. Unzip; files are in `videos/`.

For very large totals, ZIP can be slow. Prefer per-file download or git + LFS if needed.

**Option C — Clone with Git LFS**

```bash
git clone https://github.com/DJSharkApps/3abn-interview-dexter.git
cd 3abn-interview-dexter
git lfs install   # once per machine
git lfs pull      # fetch the actual MP4 files from LFS
```

No login is required for this public repo over HTTPS.

## Git LFS notes

- `*.mp4` files are tracked with Git LFS (see `.gitattributes`).
- **Public repos** on GitHub’s free plan have [Git LFS bandwidth and storage limits](https://docs.github.com/en/billing/managing-billing-for-git-large-file-storage/about-billing-for-git-large-file-storage). ~12 interview MP4s are usually fine for a one-time share; repeated large downloads can hit limits.
- If `git clone` leaves tiny pointer files instead of videos, run `git lfs pull`.

---

*DJSharkApps · public interview materials*
