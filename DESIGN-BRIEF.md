# Movie Night: UX overhaul brief

Use this as the prompt for any future redesign pass.

> Redesign Movie Night (a single-file `index.html` that recommends films, series and documentaries
> on our Dutch Netflix / Prime Video / Apple TV / HBO Max subscriptions) so it looks and feels like a
> product from a top streaming company: calm, confident, poster-first. Mobile is the main device.
> Keep every feature and the recommendation logic; change the presentation and the interaction model.
>
> **Look**
> - Dark, cinematic theme with a refined light theme; one warm accent colour; Inter type; consistent
>   8px spacing; 12px radii on posters, 20px on sheets; soft shadows, no hard borders.
> - Line icons (one consistent set) in the interface instead of emoji; emoji only in the mood chips.
> - Posters carry the design: match % badge, service logo and your rating as small overlays on the poster,
>   title + one meta line below. No walls of buttons on cards.
>
> **Structure**
> - Desktop: a slim top bar (logo · sections · search · profile · settings), one toolbar
>   (Movies / Series / Docs segmented control · Filters with an active-count badge · New picks · Surprise me),
>   then a horizontally scrolling mood row.
> - Mobile: a bottom tab bar (Tonight, For you, Watchlist, Seen) within thumb reach and respecting the safe area;
>   a compact top bar with full-width search; all tap targets at least 44px; inputs at 16px so iOS doesn't zoom.
> - Services, minimum rating, Rotten Tomatoes and length move into a Filters sheet
>   (bottom sheet on mobile, centered dialog on desktop).
> - Tapping a poster opens a detail sheet: backdrop image, meta, genres, "Watch on <service>" buttons,
>   overview, trailer and reviews, and clearly labelled rating options (Favourite / Liked / OK / Disliked,
>   Watchlist, Not for me). On desktop the same rating actions also appear on poster hover.
> - Tonight: one large poster card with the title over a gradient, NOPE / WATCH stamps while dragging,
>   big round ✕ and ♥ buttons, the reasons as a tidy grid, what it has learned shown as chips, and a clear
>   "Tonight's pick" result screen.
>
> **Feel**
> - Skeleton loaders instead of "Loading…" text; designed empty states (icon + one line + next step);
>   small toasts confirming actions; smooth, short transitions that respect reduced-motion.
> - Every state is reachable by keyboard; visible focus rings; meaningful labels for screen readers.
>
> **Constraints**
> - Stay a single static HTML file with no build step and no frameworks; GitHub Pages hosting.
> - Must work from a 360px phone to a wide desktop with no horizontal scrolling.
