# Testing

Testing is what turns guessing into knowing. You do not decide which hook is best by feel. You film a batch, put real money behind them, and let the data point at the winner. The whole reason the build works the way it does (one body, many hooks) is so the test actually means something.

## One variable at a time

If you change two things at once and the numbers move, you do not know which change did it. So you hold everything still except the one thing you are testing.

The body stays locked. The audience stays the same. The placement stays the same. The only thing that changes between variations is the hook on the front. That is why we write [one body and 15 to 20 hooks](hooks.md). When one variation beats another, you know exactly why: the hook.

This is also why the [editing setup](editing-capcut.md) builds each variation by dropping a different hook onto the same master body. Same body, different first three seconds, nothing else.

## What you are testing for, and how a winner gets picked

A hook has two jobs, in order: stop the scroll, then earn the click. So you do not crown a winner on one number. You read it as a short funnel, because the hook is the only thing changing between your ads and you want the numbers that isolate it. In order:

- **Hook Rate, target above 25 percent.** Three-second plays divided by impressions. This is the primary read. It measures the one thing the hook controls: did the first three seconds stop the scroll. If a hook is low here, nothing downstream matters.
- **CTR (Link), target above 3 percent.** The decider. Attention only pays if it turns into a click to the webclass. When two hooks both clear Hook Rate, the higher link CTR wins, because the click is the step that feeds the funnel.
- **Hold Rate (above 15 percent) and CPC-Link (under $1.50).** Supporting context. Hold Rate tells you the hook pulled in the right person and not just a cheap stop. CPC tells you it is doing that efficiently.
- **CTR (All), above 6 percent.** A general gut-check on overall engagement, not the hook decider.

Why this order: the hook is the lever you built to be swappable, so you judge it on the number that most isolates it (Hook Rate), then confirm with the action that pays (the click). A hook that stops the scroll but does not earn the click grabbed the wrong attention. Swap the hook, do not rewrite the ad.

You log all of this in the [hook test tracker](swipe-files/hook-test-tracker.md), which calculates the rates for you. Full definitions of every number live in [Understanding your KPIs](understanding-kpis.md).

## How a hook test runs

The shape of it, start to finish:

1. **Film the batch.** One body, 15 to 20 hooks you actually believe in, all against the same setup.
2. **Build the variations.** Each hook on the front of the same master body. Now you have 15 to 20 ads that differ by three seconds.
3. **Put them up together** and let them run long enough to gather real data. Do not call it after a handful of clicks. Small numbers lie.
4. **Read the scoreboard.** Sort by Hook Rate to see what stopped the scroll, then by link CTR to see what earned the click. The hooks clearing both are your live set. The ones well under are done.
5. **Cut and keep.** Kill the losers without sentiment. The winning hooks move forward and become the base you test the next batch against.
6. **Iterate.** Write fresh hooks on new angles, test them against the current champion. The bar keeps rising.

## Patience is part of the method

The most common way to ruin a test is to call it too early. A hook that looks weak on day one can settle in once enough people have seen it, and a hook that looks great on twenty clicks can fall apart at two hundred. Let it gather a real sample before you decide anything. The data only means something once there is enough of it.

## Next

- The bigger plan this fits into (hooks first, then the body): [The Ads Strategy](strategy.md).
- Reading the full scoreboard, and when to keep, kill, or scale: [Metrics](metrics.md).
- Need more hooks to test: [Hooks](hooks.md).
