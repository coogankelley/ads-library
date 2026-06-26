# Posting in Meta With Claude

Your hooks are filmed, cut, and captioned. Now the campaign goes live. You can build it by hand in Ads Manager, clicking through a new ad for every single hook, or you can have Claude build the whole thing for you and just hit publish yourself. This page is the second way, because once it is set up it turns an hour of clicking into a few minutes of reviewing.

This is exactly how The Next Wave campaign went up. Claude was connected to the ad account, it built the campaign with one ad per hook all sharing the same copy, and then we reviewed it and published. Claude never pressed go. That is the whole point.

## The Idea

Building a hook test by hand is repetitive. Same headline, same caption, same audience, same budget, and the only thing that changes from one ad to the next is which hook video sits on the front. Doing that 15 to 20 times by hand is where mistakes creep in (a wrong caption here, a mismatched setting there).

Claude can talk directly to Meta's ad system. So instead of clicking, you hand Claude the pieces once and it assembles every ad identically: one campaign, one ad set, and one ad per hook video, all carrying the same locked copy. The only variable across them is the hook, which is exactly what a clean [test](testing.md) needs.

## The Safety Model (Read This First)

The thing that makes this safe to do: **Claude builds everything paused, and only you publish.**

- Every campaign, ad set, and ad Claude creates is built in the paused or draft state. Nothing spends money the moment it is created.
- Claude never sets anything live, never changes your budget, and never publishes. You do that yourself, from Ads Manager, after you have looked at it.
- If the build stops partway (an upload drops, the wifi blips), it is safe to pick up again. It tracks what it already made and skips it, so you never end up with duplicates.

So the worst case is a paused campaign sitting in your account that you delete. Nothing goes out into the world without your finger on the button.

## What You Need Set Up Once

To let Claude build in your account, it needs a connection to your Meta ad account. This is a one-time technical setup, and it is the part you get walked through rather than figure out alone. At a high level it is two things:

- A secure access token that gives Claude permission to build (not publish) in your ad account.
- Your ad account ID, so it builds in the right place.

Both of these are secrets, so they live in your Doppler account (a secure secrets manager), never pasted into a chat window and never saved in a plain file. When Claude runs the build, it reads them straight from Doppler at the moment it runs. If anyone ever asks you to paste a token or password into a chat, stop, because that is not how this works.

You only do this setup once. After that, every future campaign is just the flow below.

## The Flow

Once the connection exists, building a campaign looks like this:

1. **Hand Claude the pieces.** Your finished hook videos (the folder of exports from [CapCut](editing-capcut.md)), your headline, your primary text caption, your daily budget, your audience and geo, and where the ad should send people (your webclass landing page).
2. **Claude builds it, paused.** It creates the campaign, one ad set with your budget and audience, then uploads each hook video and creates one ad per hook, all sharing your headline and caption. Nothing is live.
3. **Claude tells you what it made.** A plain list: the campaign name, the ad set, and every ad, so you can see the whole thing without digging.
4. **You review in Ads Manager.** Open the account, find the paused campaign, and look it over against the checklist below.
5. **You publish.** When it looks right, you flip it live yourself. That is the only step Claude does not touch.

## What to Hand Claude

Have these ready before you start, so the build is one clean pass:

- The folder of finished, captioned hook videos (one file per hook).
- Your **headline** (one line, claim-free). See [Headlines and primary text](headlines-and-text.md).
- Your **primary text** caption (the full thing, written and compliance-checked).
- Your **daily budget** (what you are willing to spend per day on the test).
- Your **audience**: geo, age range, and any targeting from your [ICA](finding-your-ica.md) Snapshot.
- The **destination URL** (your webclass landing page).

## Before You Publish: The Review Checklist

Claude builds it, but you own what goes live. Look at these in Ads Manager before you flip it on:

- **The copy is right.** Headline and caption read exactly as you wrote them, no typos, no cut-off text.
- **Compliance holds.** Run the [compliance](compliance.md) sweep on the headline and caption one more time. No income claims, no "you're exhausted" call-outs, no banned words. Meta reviews the caption and the landing page, not just the video.
- **Every hook is there.** One ad per hook video, and each is the right video.
- **Budget is what you intended.** Daily budget matches the number you gave, currency is right.
- **The destination is correct.** The link goes to your live webclass page and the page loads clean.
- **It is still paused.** Confirm nothing went live by accident before you intentionally publish.

When all six pass, publish it. Then move to reading the numbers.

## A Note for When You Are Starting Out

If the connection is not set up yet, you can still build the campaign by hand in Ads Manager: one ad set, one ad per hook, the same headline and caption on each, pointed at your webclass page. The Claude workflow is the time-saver once you are running tests regularly, not a requirement to get your first ad live. Either way, the rules above (paused until you publish, full compliance check, one variable) are the same.

## Next

- Now read what comes back: [Metrics and optimizing](metrics.md).
- Why the campaign is built one-ad-per-hook: [Testing](testing.md).
