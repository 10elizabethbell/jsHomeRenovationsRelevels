# J's Home Renovations & Relevels — handoff at ~60%

**Live:** https://10elizabethbell.github.io/jsHomeRenovationsRelevels/ · **Repo:** https://github.com/10elizabethbell/jsHomeRenovationsRelevels · **Built:** 2026-10-18 from Muse brief (run 2026-10-18, Facebook group "Essex County Contractor Referrals")

## What's built
- Single-file `index.html` (~43 KB, no images except og/favicon), phone-first, system font stack.
- **World:** storm-slate sky, rain, a single-wide home on cinder-block piers, a red bottle jack and a yellow spirit level on the roof. Built from the owner's own line, "Rain or shine we work all the time".
- **Signature element (hero canvas):** the home settles out of level, the crew jacks it back, the vial bubble slides to center and the windows light up ("Level. That's how we leave it."). Then it settles the other way and the loop repeats. Visitors take over by dragging either end up or down (mouse or finger, any direction; vertical drags don't scroll the page inside the scene), and the rain parts around the pointer. The low side's piers sink into the mud as it tilts.
- Animated puddle-surface seams between sections. One shared rAF loop, paused off screen, still frame under reduced motion.
- **Sections:** header (J's wordmark, tap-to-call number top right) → hero (BACK TO LEVEL., promise, Free quote + What's a relevel?) → What we do (Home sets / Relevels / Renovations rows; each opens the form with that job picked) → Is your home settling? (5 signs + what a relevel is) → How it goes (3 steps + care line + Facebook button) → Free quote form → close (name, "Ask for Joshua") → footer.
- **Contact:** the quote form builds a pre-filled text to (580) 775-1897 (`sms:+15807751897?&body=…`), with an inline call link under it. Tested: errors show for name/job/town, and the encoded body decodes correctly.

## Assumptions I made
- **Colors:** none exist (no logo). Slate ground (#1b2a39), level-tool yellow (#f2c230) accent, rain-blue (#8fcbff) for form hover/focus, paper (#eceae4) band.
- **Favicon / home-screen icon:** no logo, so they use the site's own "J's" lettering over a level vial.
- **Voice "we":** the caption says "give us a call", so they're treated as a crew. "Ask for Joshua" uses the owner name from the posting profile.
- **Services:** only "set" and "relevel" are stated; "Renovations" comes from the business name, with no specifics.
- **Signs of settling** and **How it goes** (come look, give a price, lift/shim/check) are general trade knowledge, not the owner's words. Confirm with him.
- **Care line** ("We lift it slow, check it twice…") is written in his voice but not quoted from him.
- **Audience:** not treated as 40+ (the brief doesn't say), so motion is on. If Ellie thinks his customers skew older, switch to a still scene per `older-audience.md`.

## Placeholders and gaps
- **Service area:** unknown (580 = Oklahoma, but the ad ran in a NJ group). The page says "Call for service area" / "Ask about your area" and never names a place.
- **Does the number take texts?** Unknown. The form hands off by text, with the call link right under it. If it's a landline, make the form call-first.
- **Facebook** is Joshua's personal profile (no business page); the button says "See us on Facebook", not "see our work", because the timeline couldn't be checked.
- No email (none in the footer), hours, prices, reviews, logo or photos. The only video is shot from inside a truck in the rain (a home on blocks is visible through a wet window); it's too blurry and personal to use and is not published.

## Questions for the owner
- Where do you work (towns/counties/states)? Is it NJ or Oklahoma?
- Can customers text (580) 775-1897?
- 3+ photos of a set or relevel (before/after if possible), and a logo if you have one.
- Hours? Do you do new sets from dealers, used-home moves, or both? Anything under "renovations" worth naming (skirting, decks, floors)?
- A business Facebook page, or should the site link your personal one?
- Any reviews or customers willing to give one?

## Ideas not built (yours to pick)
- **Runner-up world:** "the job site at golden hour": a dry, warm palette with tie-down straps and a laser line sweeping across the home. Less on-brand than rain-or-shine, but brighter.
- Photo strip or before/after slider under "How it goes" once photos exist, with the Facebook link moved directly under it.
- Short haptic tick (`navigator.vibrate(12)`) when the home snaps level (Android only).
- Wet-ground reflection of the windows lighting up when level; more rain on desktop.
- Pressing the level with the arrow circle on the service rows (fill like a vial bubble on hover).
- Desktop leaves empty columns beside "Is your home settling?". Could put "How it goes" beside it, or a photo once one exists.
- The hero promise line names the services; trim it to just the promise if you prefer.

## Not verified
- Real-device touch (iOS Safari, the Facebook in-app browser, Android Chrome). Tested only with simulated pointer/touch events in headless Chrome.
- The real SMS handoff on iOS/Android, and whether the number receives texts at all.
- Frame rate on old phones (rain count is 150 on phones; the backdrop is cached).
- WebKit audit not run.
