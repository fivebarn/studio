# studio

Small, readable [Claude](https://claude.ai) skills for everyday life admin — inbox, shopping, travel, scheduling, goals, and creator/small-business work.

Each skill is a single `SKILL.md` file you can read in a couple of minutes before installing.

## Skills

| Area | Skill | What it does |
|---|---|---|
| Inbox & admin | [inbox-triage](skills/inbox-triage/SKILL.md) | Clears a backlog by sender, sorts the rest, and drafts replies in your voice |
| | [email-action-items](skills/email-action-items/SKILL.md) | Pulls to-dos out of email, builds carts, fills forms, and adds due dates to your calendar |
| Shopping & money | [cart-builder](skills/cart-builder/SKILL.md) | Turns a list, photo, recipes, or past order into the best-priced cart, stopping before checkout |
| | [subscription-saver](skills/subscription-saver/SKILL.md) | Finds every recurring charge, hunts for better deals, and cancels on approval |
| | [price-drop-tracker](skills/price-drop-tracker/SKILL.md) | Catches price drops and refunds owed, files claims on approval, and keeps watching weekly |
| Travel & going out | [flight-delay-helper](skills/flight-delay-helper/SKILL.md) | Watches your flights, rebooks when things go wrong, fixes the rest of the trip, and files claims |
| | [trip-planner](skills/trip-planner/SKILL.md) | Itinerary built around your bookings and saved spots, booked on approval, with pre-trip check-ins |
| | [saved-posts-organizer](skills/saved-posts-organizer/SKILL.md) | Turns saved posts into lists, a spreadsheet, and a map, then books, plans, or shops from them |
| | [reservation-booker](skills/reservation-booker/SKILL.md) | Books dinner or movie seats on approval, watches sold-out times, and handles the follow-up |
| Briefing & scheduling | [morning-briefing](skills/morning-briefing/SKILL.md) | A 5-line daily brief: schedule, weather, key emails, commute, birthdays, news (text or audio) |
| | [calendar-guard](skills/calendar-guard/SKILL.md) | A weekly look-ahead that fixes conflicts, adds travel time, and protects focus and family time |
| Goals & projects | [goal-to-tasks](skills/goal-to-tasks/SKILL.md) | Breaks a goal into tasks, routes them to the right skill, and checks in until it is done |
| | [training-plan](skills/training-plan/SKILL.md) | Race training plans from your fitness data, on your calendar, adjusted every week |
| | [folder-tidy](skills/folder-tidy/SKILL.md) | Organizes a messy folder into your own system, renames vague files, never deletes anything |
| Creator & business | [brand-deal-tracker](skills/brand-deal-tracker/SKILL.md) | Tracks brand deals from email and DMs, prices them from your insights, and chases payment |
| | [hiring-assistant](skills/hiring-assistant/SKILL.md) | From job post to offer: fair screening, an applicant tracker, interviews, and candidate emails |
| | [event-ticketing](skills/event-ticketing/SKILL.md) | Sets up ticket sales, promotes the event, tracks sales against goal, and handles follow-up |

## Install

### Claude app (web, desktop, mobile)
1. Download the skill's `.zip` from the [Releases](../../releases) page (or download this repo and zip the skill's folder yourself — the zip should contain the folder, e.g. `inbox-triage/SKILL.md`).
2. In Claude, open **Customize → Skills**, click **+**, then **Create skill → Upload a skill**, and choose the `.zip`.
3. Make sure the skill is switched on. Claude will use it automatically when a request matches, or you can ask for it by name.

### Claude Code
Add this repo as a plugin marketplace, then install one skill or all of them:

```bash
/plugin marketplace add fivebarn/studio

# one skill (any name from the table above)
/plugin install inbox-triage@fivebarn-studio

# or all 17
/plugin install all-skills@fivebarn-studio
```

Or copy a skill's folder into your skills directory by hand:

```bash
# for all your projects
cp -r skills/inbox-triage ~/.claude/skills/

# or for one project only
cp -r skills/inbox-triage .claude/skills/
```

### Connections
Most skills work best with the matching connections turned on in Claude (email, calendar, a browser, a fitness app). Without them, each skill falls back to working from text, screenshots, or files you paste in.

Found a problem? Please [open an issue](../../issues).

## Support

These skills are free to use with no obligation. To support Five Barn Studio, tips are welcome at [buymeacoffee.com/fivebarn](https://buymeacoffee.com/fivebarn) or [venmo.com/u/fivebarn](https://venmo.com/u/fivebarn).

## License

[MIT](LICENSE)
