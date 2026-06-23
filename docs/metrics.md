# Metrics and optimizing

Numbers tell you where the funnel is leaking. Each stage has a minimum it has to clear. Above the minimum, that stage is doing its job. Below it, that is the stage to fix before you touch anything else. These are not dream numbers. They are floors. Hitting them means the stage works. Beating them means it works well.

The point of reading metrics this way: you stop guessing and you stop optimizing the wrong thing. If the ad is fine but the page is leaking, no new hook saves you. The numbers tell you exactly where to put your attention.

This page is how to *act* on the numbers. For what each number means, its floor, and how the tracker calculates it, see [Understanding your KPIs](understanding-kpis.md).

## The top of the funnel (what the ad is judged on)

This is the part you control directly when you make ads.

| Metric | Minimum | What it means when it lags |
|---|---|---|
| **CTR (All)** | **6%** | Below 3 percent, the creative is not engaging enough. Rework the hook or the visuals. |
| **CTR (Link)** | **3%** | Below 1 percent, the hook or value prop is not earning the click. The hook is the lever. |
| **Landing Page Conversion** | **20%** | Below 20 percent, the page messaging, layout, or offer needs work. A great ad leaks here. |

This is the whole reason you batch [15 to 20 hooks](hooks.md) against one body. You are hunting for the hooks that clear those CTR bars. A low link CTR points straight at the hook, which is the one thing you built to be swappable.

One trap to watch: the ad can be doing its job and still look like it is failing, because the page behind it is leaking. The ad dumps cold traffic onto the webclass landing page. If that page still carries old income-claim language or a clumsy layout, a great ad bleeds out right there. Worth fixing the page before you scale spend behind a winning ad.

## Downstream (context, not ad levers)

These are further down the funnel. You do not fix them by changing the ad, but it helps to know what good looks like, because a problem here can look like an ad problem if you are not watching the whole chain.

| Metric | Minimum | What it points at when it lags |
|---|---|---|
| Saw Offer Rate | 20% | Webclass retention, delivery, engagement |
| Front-End Sale (the $99 start) | 3% | Offer clarity, pitch strength, perceived value |
| Booked Call Rate | 70% | Lead quality, discovery process, CTAs |
| Show-Up Rate | 80% | Reminders, confirmation messaging, scheduling friction |
| Close Rate (back-end sale) | 10% | Lead quality, sales process, discovery questions, objections |

(Full definitions and the diagnosis for each are in [Understanding your KPIs](understanding-kpis.md).)

## Keep, kill, or scale

Once an ad has gathered enough data to trust (not a handful of clicks, a real sample), you make one of three calls:

- **Keep** when it is hitting the CTR floors but not running away. It works. Leave it running and keep testing fresh hooks against it.
- **Kill** when it is well under the floors after a real sample. Do not nurse a loser or get attached to a line you loved writing. Cut it and move the budget.
- **Scale** when it is clearing the floors with room to spare and staying stable as spend grows. Raise the budget gradually and watch that the numbers hold. If they crack as you scale, ease back.

The discipline is the same one from [Testing](testing.md): give it enough data first, then decide without sentiment. Small numbers lie, and a hook you love is not a hook that earned its spot.

## The daily tracker

You log the numbers daily into one sheet so the whole funnel sits in one row and a leak shows up the next morning instead of three weeks and a lot of spend later. There are two versions (Landing Page, and DM / Instant Form), one row per day grouped into months, with the targets written right into the column headers. Pick the one that matches your ad, make your own copy, and never type over the master.

Which one to use, every column defined, and how each metric is calculated all live in [Understanding your KPIs](understanding-kpis.md). The point is not the logging, it is that the tracker tells you which stage broke before you have wasted budget on it.

## Let Claude pull and read the numbers

You do not have to export CSVs or copy cells by hand. Claude is connected to your Meta ad account for reads, so you can just ask: pull the numbers on my live hook test. It reads CTR (All), CTR (Link), and landing-page conversion for each hook, lines them up against the floors above, and tells you which hooks are clearing the bar and which are not. It can drop the day's numbers straight into your tracker copy so the row is filled for you.

It is reads only, on purpose. Claude pulls and reports, but it never changes a budget and never flips anything live or off. Those calls stay yours, the same rule as [Posting in Meta](posting-meta.md). What you get is the read done in seconds, so your time goes to deciding instead of collecting.

## How to actually run this

You do not stare at a dashboard all day. You check the top-of-funnel numbers, find the lowest stage that is under its floor, and fix that one thing. Then you re-check. One leak at a time, in order, from the top. Chasing five metrics at once is how you spend a week optimizing and move nothing.

## Next

- Need to understand how the test that feeds these numbers is set up: [Testing](testing.md).
- Hook CTR low? That is the lever: [Hooks](hooks.md).
