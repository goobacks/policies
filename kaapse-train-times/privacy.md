# Privacy policy | Kaapse Train Times

*Last updated: 2026-10-30*

> The canonical version of this policy is published at <https://kaapsetrains.co.za/privacy/>.
> This file is generated from the same source as that page: do not edit it by
> hand; change `packages/web/src/content/privacy.ts` in the app repo and
> regenerate, so the two can never disagree.

Kaapse Train Times is an independent app for Cape Town's Metrorail timetables. It has no accounts and no adverts. It counts which pages and screens are opened, anonymously (on the website through Vercel, in the Android app on its own server), and it counts station searches that match no station, also anonymously. Beyond that it collects nothing about you unless you choose to send a problem report. This policy explains exactly what that means.

## What the app collects

**Anonymous page-view counts on the website**: The website uses Vercel Web Analytics (run by Vercel, the company that hosts the site) to count visits. Each page view records the page's address (without anything after a “?”, except that for a journey search the count records which two stations were searched, never the day, time or train, and not linked to you), the page that linked to it, the country and city the request came from, and the kind of device, browser and operating system. It sets no cookies and stores no identifier on your device; visitors are told apart by a temporary code that is discarded within a day, so views cannot be linked to you across days.

**Anonymous screen counts in the Android app**: The Android app cannot use that counter, so it counts for itself. Each time it opens a screen it sends the site's own server an anonymous count of which screen it was: the screen's address, or for a journey search which two stations were searched, never the day, time or train. The server adds one to that day's total for that screen in a database run by Upstash, a database provider, for the app's operator. Only those daily totals per screen are stored, for up to 400 days. No IP address, device identifier or anything else about you is stored with a count, so counts cannot be linked to you or across days. Your phone talks only to the site's own server; that server alone talks to Upstash. If the phone is offline the count is simply not sent.

**Station searches that match no station (website and Android app)**: When a station search finds no station by that name, the website and the app send that search word to the site's own server. It is lowercased, accents are removed, and it is limited to letters, spaces, hyphens and apostrophes, up to 20 characters. Anything with a digit or an @, or longer than that, is never sent. It is sent only once you pause typing or leave the box, never letter by letter. It is stored only as a daily count per word, in the same Upstash database, for up to 400 days, to find station nicknames and misspellings the app does not know. Searches that do match a station are not recorded. No IP address or identifier is stored with a word, so words cannot be linked to you or across days.

**No accounts, no adverts, no profile**: There is no sign-up and no advertising. The counts above say that a screen was viewed (for a journey search, which two stations), or that a word was searched, not who viewed or searched it. The app still does not know who you are, and no profile of you exists because none is ever built.

**No cookies, no third-party scripts**: The app loads only files served from its own web address: no third-party scripts, fonts or embedded content. The analytics script is served the same way, by the app's own host from the app's own address. Its Content Security Policy restricts it to its own origin, so this is enforced by your browser rather than only promised here. Besides Vercel Web Analytics, the website talks to one other address: its own server's /api/count/, for the search-word counts described above and for nothing else.

## Links to other services

**Maps and live updates**: Tapping Map on a station opens Google Maps with that station's name. The Live updates links open PRASA's WhatsApp channels. The app sends nothing itself: once you follow such a link you are on that service, under its own privacy policy.

**Google Play's rating prompt**: Now and then, the Android app may ask Google Play to show its own prompt to rate the app. Google shows and runs that prompt under its own privacy policy. The app is not told whether you rated it or what you wrote.

**Google Play app updates**: The Android app asks the Play Store on your phone whether a newer version is available, and if so shows a short note offering to update. Google runs the download and install under its own privacy policy. Nothing about this is sent to us.

## What is stored on your device

**Your saved preferences**: Favourite stations, saved journeys, recent stations and journeys, and your settings (direction preference, language, colour theme, and whether you've dismissed the install prompt) are held in your browser's local storage on your own device. They are never transmitted anywhere, and clearing the app's data or uninstalling it removes them.

**When to ask for a rating**: To keep that prompt rare, the Android app stores on your device how many days you have used it and when it last asked. This is never sent anywhere, and clearing the app's data or uninstalling it removes it.

**Closed update notes**: If you close an update note, the Android app remembers on your device which version it was about and when, so it doesn't show it again for a week. This is never sent anywhere, and clearing the app's data or uninstalling it removes it.

**The offline timetable**: The timetable and the app's own files are cached on your device so it works without a signal. This is a copy of public schedule data, not information about you.

## Problem reports

**Only if you fill in the form and tap Send**: Apart from the anonymous counts (the website's page views, the Android app's screens, and station search words that match no station) and the Android app's timetable update check (all described in this policy), nothing else leaves your device unless you actively submit a report. Apart from those unmatched search words, the report form is the only part of the app that sends anything you typed, anywhere.

**What a report contains**: What you typed; the category you chose; the screen you were on (line, station, direction, timetable day, or journey); your email address if (and only if) you entered one; the browser and device identification string your browser sends with every web request (its user agent), which helps diagnose app problems; and the time it was received. Nothing else.

**Where it goes**: The report is posted to this app's own server, which emails it on through Resend, an email delivery provider, to the app's contact inbox. Resend processes it only to deliver that message. If you gave an email address it is set as the reply address so you can be answered.

**Your IP address**: The server sees your IP address, as every web server does, and uses it briefly in memory to stop one source flooding the form with reports, or the anonymous counts (screens and search words) with false ones. It is not written to the report, not included in the email, and not stored with a count or anywhere else: it is discarded when the server instance recycles.

**How long reports are kept**: A report is an email in an inbox. It is kept while it is useful for fixing what you reported and for checking the correction later, then deleted. You can ask for yours to be deleted sooner by writing to hello@hyperfocushive.com.

## Hosting

**Vercel**: The site is hosted by Vercel, which (like any web host) processes the requests your browser makes in order to serve the pages. Vercel also provides the website's anonymous page-view counting described under “What the app collects”.

**Upstash**: The Android app's anonymous screen counts and the search-word counts of both the website and the app (all described under “What the app collects”) are stored in a database run by Upstash, a database provider, for the app's operator. Upstash holds only the daily totals per screen and per search word, which say nothing about you, and processes them only to store and return them.

**Android app timetable updates**: The Android app checks kaapsetrains.co.za for a newer version of its timetable and files at most every six hours, and downloads it from the same server. No information about you is sent with that request beyond what any web request carries.

## Your rights and contact

**Who is responsible**: Hyperfocus Hive publishes Kaapse Train Times and is responsible for the personal information described here.

**Asking about your data**: Write to hello@hyperfocushive.com. Because the app holds nothing about you beyond any report you chose to send, a request usually amounts to deleting that report, which will be done on request.

**Complaints**: If you are not satisfied with how a request was handled, you can complain to South Africa's Information Regulator (inforegulator.org.za).

**Children**: The app is a public transport timetable. It is not directed at children, and it collects nothing from anyone, of any age, who does not submit a report.

**Changes to this policy**: Last updated 2026-10-30. If what the app collects ever changes, this page changes with it, and so does the shorter privacy summary on the app's help page, which states the same facts in fewer words.
