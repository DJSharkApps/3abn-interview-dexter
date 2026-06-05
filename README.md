# 3ABN Interview Materials

Private repository for sharing **3ABN interview** video files with **Dexter Thomas** (read-only access).

## Contents

Place interview MP4 files in the `videos/` folder (or the repo root). Large files should use **Git LFS** (see below).

## For maintainers (uploading videos)

1. Install [Git LFS](https://git-lfs.com/) if any single MP4 is over ~50 MB.
2. Copy your `.mp4` files into this repo (e.g. `videos/`).
3. Commit and push:

```bash
cd /path/to/3abn-interview-dexter
git lfs install   # once per machine, if using LFS
git add videos/*.mp4
git commit -m "Add interview videos"
git push origin main
```

## For Dexter (downloading)

**Option A — Clone the whole repo**

```bash
gh auth login   # or use HTTPS with a personal access token
gh repo clone DJSharkApps/3abn-interview-dexter
cd 3abn-interview-dexter
git lfs pull    # if videos use Git LFS
```

**Option B — GitHub website**

1. Open https://github.com/DJSharkApps/3abn-interview-dexter
2. Browse to each `.mp4` file and use **Download**.

**Option C — Zip from GitHub**

Use **Code → Download ZIP** after videos are pushed (works for moderate total size; very large repos may be slow).

You need **read** access to this private repo (collaborator invite must be accepted).

---

*DJSharkApps · private materials*
