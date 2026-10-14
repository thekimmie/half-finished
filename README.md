# Half-Finished ✳

**A cozy little studio for all the projects you intend to finish someday.**

**Tagline:** Pick up where you left off.

A mobile-first, no-pressure app for makers, DIYers, artists, and people with a lot of good ideas. Built as a static site: no framework, npm install, database, account, or paid hosting is required.

## What works in version 0.2 (Wild Little Studio edition)

- Add, edit, and delete creative projects
- Add a project photo (resized and compressed in your browser), category, notes, and whimsical icon
- Save one **next tiny step** so future-you can resume without reconstructing the whole project
- Mark steps done; see a small history of wins
- Track supplies with a tap-to-check checklist
- Move projects between **In the making**, **On the shelf**, and **Finished**
- Filter project cards and use **Pick one for me** when you don't know where to begin
- Save locally on the device in the browser; export/restore JSON backups
- Responsive layout for phones, tablets, and desktop

The three preloaded projects are examples and can be cleared from the top notice. Your data is not uploaded anywhere.

## Try it

Open `index.html` in a modern browser, or host the files using GitHub Pages.

### Deploy on GitHub Pages

1. Create a new **public** repository called `half-finished` at GitHub, in the account where you want to publish it. Don't reuse another project's repository.
2. Upload `index.html`, `favicon.svg`, and `manifest.webmanifest` to the root of its `main` branch; include this README if you'd like.
3. In **Settings → Pages**, choose **Deploy from a branch**, set `main` and `/ (root)`, then save.
4. Once GitHub finishes deploying, the site is accessible at `https://YOUR_USERNAME.github.io/half-finished/` (unless you choose another domain/path).

### Privacy and limitations

**Version 0.1 uses local browser storage, not cloud synchronization.** Projects added on a phone are not automatically visible on an iPad or laptop, even if they visit the same app URL. The published site hosts the code only; visitors will see sample projects at first, not somebody else's private project data. Browsers can erase local data, so use **Studio tools → Back up my projects** periodically; importing that JSON restores a copy on another device. Browser storage space is limited, particularly when using many photos.

The manifest supplies home-screen metadata. Offline access is not guaranteed yet, because we haven't implemented an offline service worker.

## Next milestones (deliberately not in version 0.1)

**0.2 — Make it feel magical:** search/tagging, sort by project age, photo gallery / before-and-after, time- and energy-based project picker, optional voice-note breadcrumbs.

**0.3 — Optional sync and sharing:** opt-in accounts, private cloud sync across devices, individual read-only project share links, collaboration controls, accessible import/export migration.

**0.4 — Helper tools:** AI breakdowns for overwhelming projects, supply reuse hints, distraction-free resume mode. Keep these optional; the core experience must work without AI or a subscription.

## Product principles

1. **No guilt:** no overdue badges, streaks, or calendar-pressure UX.
2. **One breadcrumb is enough:** saving a name and next step is a real success.
3. **Keep the spark:** photos, notes, supplies, and progress live together.
4. **Make sharing optional:** user projects remain private by default.
5. **Start small:** build for real use before adding advanced features.

## Tech

Vanilla HTML, CSS, JavaScript; localStorage and canvas image compression. No external services or analytics. MIT license can be added after deciding licensing; no license is granted by this repository as-is.

## Visual direction — The Wild Little Studio (v0.2)

The maker's [Wild Rumpus Agenda](https://www.wildrumpusagenda.com/) inspired a more theatrical, storybook visual identity: inky plum, electric fuchsia, antique-gold details, a bespoke ornate key, soft paper textures, and collected-curiosity frames. `studio-theme.css` holds the visual overrides and `studio-key.svg` is the key artwork. To revert the redesign without changing the app or its data, remove the `studio-theme.css` link from `index.html` and restore the previous hero HTML.

This release changes **only presentation and microcopy**. It deliberately retains the `half-finished-v1-projects` local-storage key, project model, and all CRUD/export/import behavior; existing local projects should continue to load on the same browser/device.

## v0.3 original maker logo + Wild Rumpus colors

The ornamental logo is the exact original PNG artwork (with a secondary vector trace for scalable icons), credited to its creator, Kimmie Hamilton. Palette anchored by the original coral pink (#EA4B5F), with tangerine, marigold, teal and lilac accents. This is a visual-only update; project storage and saved records are unchanged. Do not reuse the logo outside this project without its creator’s permission.


## What changed in v0.4

- Color palette tuned closer to Wild Rumpus Agenda
- Header key moved upright at the top and turned so the crescent faces left
- App icon / installed-site widget icon updated to match the logo direction and palette