# PTCB Practice Exam (GitHub Pages)

A single-file browser app that generates a 90-question PTCB-style practice test with:
- 4 choices per question
- Optional 90-minute timer
- Learning mode (missed questions appear more often)
- Optional dynamic medication questions via NIH/NLM RxNav (RxNorm) API

## How to host on GitHub Pages

1. Create a new GitHub repo (public recommended for free Pages).
2. Add `index.html` (this app) to the root of the repo.
3. (Optional) Add `.nojekyll` to the root.
4. Go to **Settings → Pages**:
   - **Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
5. Save. GitHub will give you a Pages URL.

## Notes
- Learning data uses `localStorage` on each device/browser. It does not sync between devices.
- RxNav requires internet. If RxNav fails or is rate-limited, the app backfills with local question bank items.
- This is a practice tool and is not affiliated with PTCB.
