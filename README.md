# Breach the Clocks

An exercise in breach notification deadlines. When an incident becomes a breach, the clocks don't line up: they come from different laws and contracts, and they start at different moments. Pick a company, map who has to be told, when each clock starts and when it runs out, then check your work.

**Try it:** https://jckesler.github.io/breach-the-clocks/

It takes about 10 minutes per case. There's no login and nothing to install.

It's a companion to [The 2AM Page](https://jckesler.github.io/the-2am-page/), an incident response tabletop that uses the same three companies. You don't need to play one to do the other.

## The cases

| Case | Company | What it tests |
|---|---|---|
| **Harbor Ridge Health** | Regional health system, Norfolk, Virginia | HIPAA's individual, HHS and media notices; when "discovery" happens; why Virginia's laws and the SEC don't apply |
| **Pinecrest Outfitters** | Publicly traded retailer, Asheville, North Carolina | SEC Form 8-K timing from the materiality determination; North Carolina and Colorado notice duties; credit bureau and Attorney General thresholds |
| **Larkspur HR** | HR software vendor, Denver, Colorado | A processor's duties to its customers under GDPR, a customer contract, and Colorado and North Carolina law; its own controller clock for its CRM data |

The companies are invented.

## How it works

- Each case has a brief: the facts that decide which laws apply, and a timeline of what happened when.
- For each requirement, you choose the deadline rule and the event that starts the clock, or say it doesn't apply. The app works out the actual deadline as you go.
- A clock reference lists the rules (who tells whom, what starts the clock, the deadline), including some that apply to none of the cases, so the work is matching rules to facts.
- Checking your map explains every answer, including the ones that don't apply, and lists the clocks in the order they run out.
- A "Copy my answers" button puts a plain-text summary on the clipboard, for anyone who needs to hand it in.

## Accuracy

The legal details (HIPAA, SEC Form 8-K Item 1.05, GDPR Article 33, and the Virginia, North Carolina and Colorado breach laws) were checked against primary sources in November 2026. They're simplified to fit an exercise, and laws change. Where the answer depends on judgment, such as the moment a breach counts as "discovered," the app accepts the defensible readings and explains why one is safer. Nothing here is legal advice. In a real incident, your counsel decides what applies.

## Technical notes

- One HTML file with plain JavaScript. There are no frameworks and no build step.
- Nothing is stored or sent anywhere. There are no cookies, no local storage and no analytics.
- The only external request is for fonts from Google Fonts. Offline, the page falls back to system fonts and still works.
- It works on phones as well as desktops, and supports light and dark mode.

## License

© 2026 Chuck Kesler. Licensed under [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/). See [LICENSE](LICENSE).

You're welcome to use and adapt it for teaching, training and other non-commercial purposes, with credit. For commercial use, please get in touch.

## About

Written by [Chuck Kesler](https://www.linkedin.com/in/chuckkesler/), who has more than 15 years of experience as a CISO. He's a member of the IANS faculty, is a frequent speaker at industry conferences, and also teaches a graduate-level data security and privacy course at NC State University.
