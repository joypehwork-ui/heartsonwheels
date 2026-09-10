# Hearts on Wheels

Volunteer page for the department's Meals-on-Wheels session with TOUCH Home Care —
**Sunday 20 September 2026, Hong Kah North CC.**

One file. Double-click `index.html`, or send the published link.

## One thing left to do

Create the WhatsApp group, then paste its invite link into the `EVENT` block near the top of the
script in `index.html`:

```js
organiserName:  "Joy",
organiserPhone: "",                     // see below — leave empty
whatsappLink:   "[WHATSAPP GROUP LINK]",   // <- replace this
```

Until that link is real, the two photo buttons and the Call button render dimmed and say
"coming soon", rather than looking active and silently doing nothing.

Anything still in `[SQUARE BRACKETS]` shows up highlighted in amber on the page, so you can see at
a glance what you've missed.

### Why the mobile is blank on purpose

This page is public and search-indexable. A mobile number on it would be scraped and would outlive
the event in caches long after you delete it. So Joy's number goes in the WhatsApp group message,
where only colleagues see it.

With `organiserPhone` empty, the Call button points at the group chat instead of producing a dead
`tel:` link. If you ever do want tap-to-call on the page, put the digits there and accept that they
become public.

Once TOUCH confirms the timings, set `provisional: false` and the amber warning banner disappears.

To change the run of show, edit the `schedule` list. `star: true` marks the group photo — that's
the item the page shouts about.

## What the page does

The card at the top reads the clock and changes on its own:

| When | Shows |
|---|---|
| Before | Days to go, and a nudge to pack |
| Morning of | "Be there by 3pm", counting down |
| During | The current step, and what's next |
| **3.35–3.52pm** | **Flashing group photo alert** |
| After | Thank you, and send your photos |

Below that: where and when, run of show, the photo shot list, a packing checklist, doorstep
dos and don'ts, and who to call. Checklist ticks are saved in the browser.

## Previewing any moment

Add `?now=` to the URL to see exactly what volunteers will see at a given time:

```
index.html?now=2026-09-20T15:37     <- the group photo alert
index.html?now=2026-09-20T16:40     <- mid delivery
```

## Names are deliberately not in here

Car assignments have colleagues' names in them, so they are not on this page — send those over
WhatsApp instead. There is a commented `TEAMS` block in the file if you ever want them, with a
reminder that re-publishing would make those names public.

## Still to confirm with TOUCH

- The 3–6pm timing
- How many meal packets
- Which delivery zones each car takes
- Parking at the CC for 5–7 cars

All of these are one-line edits in the `EVENT` block.
