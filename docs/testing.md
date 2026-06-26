# Testing

Testing is what turns guessing into knowing. You do not decide which hook is best by feel. You film a batch, put real money behind them, and let the data point at the winner. The whole reason the build works the way it does (one body, many hooks) is so the test actually means something.

## One Variable at a Time

If you change two things at once and the numbers move, you do not know which change did it. So you hold everything still except the one thing you are testing.

The body stays locked. The audience stays the same. The placement stays the same. The only thing that changes between variations is the hook on the front. That is why we write [one body and 15 to 20 hooks](hooks.md). When one variation beats another, you know exactly why: the hook.

This is also why the [editing setup](editing-capcut.md) builds each variation by dropping a different hook onto the same master body. Same body, different first three seconds, nothing else.

## What You Are Testing for, and How a Winner Gets Picked

A hook has two jobs, in order: stop the scroll, then earn the click. So you do not crown a winner on one number. You read it as a short funnel, because the hook is the only thing changing between your ads and you want the numbers that isolate it. In order:

- **Hook Rate, target above 25 percent.** Three-second plays divided by impressions. This is the primary read. It measures the one thing the hook controls: did the first three seconds stop the scroll. If a hook is low here, nothing downstream matters.
- **CTR (Link), target above 3 percent.** The decider. Attention only pays if it turns into a click to the webclass. When two hooks both clear Hook Rate, the higher link CTR wins, because the click is the step that feeds the funnel.
- **Hold Rate (above 15 percent) and CPC-Link (under $1.50).** Supporting context. Hold Rate tells you the hook pulled in the right person and not just a cheap stop. CPC tells you it is doing that efficiently.
- **CTR (All), above 6 percent.** A general gut-check on overall engagement, not the hook decider.
- **Webclass registrations.** The bottom line. A click only pays if it becomes a registration, so the hook that turns clicks into actual webclass leads is the one carrying the funnel. Your [hook test tracker](swipe-files/hook-test-tracker.md) now counts registrations per hook (it reads the hook off the UTM tag on each ad), so you see which hook earned the lead, not just the click.

Why this order: the hook is the lever you built to be swappable, so you judge it on the number that most isolates it (Hook Rate), then confirm with the action that pays (the click). A hook that stops the scroll but does not earn the click grabbed the wrong attention. Swap the hook, do not rewrite the ad. And when two hooks both earn the click, the tiebreaker is which one earns the registration. That is the number closest to revenue.

You log all of this in the [hook test tracker](swipe-files/hook-test-tracker.md), which calculates the rates for you. Full definitions of every number live in [Understanding your KPIs](understanding-kpis.md).

## How the Test Campaigns Roll Out

The test runs in three phases, and the first two each have their own campaign version. You leave winners running, keep narrowing, and let the data do the cutting.

### Phase 1: Find Your Winning Hooks

This is the hook hunt, and it runs across more than one campaign round.

**V1: test every hook.** Build one campaign (V1) with all your hooks, one ad each, same body. Let it run about 7 days with no changes. Resist touching it, even when one looks weak on day two. At the end, read the scoreboard: which hooks are clearing the CTR floors, pulling webclass registrations, and eating the most of your budget. That last one is a quiet tell. Once a campaign has a few days on it, Meta pushes spend toward the ad it thinks is winning, so the hook taking the most budget is usually Meta agreeing with your numbers.

**V2: retest the rest.** Once you have a winner, duplicate the campaign into V2 and run all the hooks again except the winner. The winner keeps running in V1. Give V2 another 7 days, same metrics deciding it. A hook that looked soft in a crowded V1 sometimes proves itself with room to breathe.

Keep narrowing this way, round by round, until you have your **3 to 5 winning hooks.** Those are your proven openers.

### Phase 2: Test the Visual (V3)

Now you have about 4 winning hooks, and you already know the wording works. Phase 2 tests the visual. Take each winning hook and film it again in different places: new location, setting, backdrop, outfit. The hook and the body stay the same. Only the surroundings change. Build V3 with **one ad set per winning hook**, each ad set holding that hook's variations:

```
V3
  Ad set 1:  H01 body, recorded 4 ways
  Ad set 2:  H08 body, recorded 2 ways
  (one ad set per winner, as many versions as you filmed)
```

This tells you not just which hook wins, but which version of it wins.

### Phase 3: Test the Body, Then Keep Optimizing

Now the lever moves to the body. Same discipline: one variable at a time. You only ever change one thing at a time, whether that is the relatability beat, the content, where you filmed, or how you edited the body. Change one thing, run it, read the result, keep or kill.

Phase 3 does not really end. It is the ongoing operation where you keep optimizing off what the numbers tell you. Your top hooks and best body become the base everything new gets measured against, and the bar keeps rising.

## Patience Is Part of the Method

The most common way to ruin a test is to call it too early. A hook that looks weak on day one can settle in once enough people have seen it, and a hook that looks great on twenty clicks can fall apart at two hundred. Let it gather a real sample before you decide anything. The data only means something once there is enough of it.

## Next

- The bigger plan this fits into (hooks first, then the body): [The Ads Strategy](strategy.md).
- Reading the full scoreboard, and when to keep, kill, or scale: [Metrics](metrics.md).
- Need more hooks to test: [Hooks](hooks.md).
