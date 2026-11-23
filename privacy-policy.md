# Ad Defense — Privacy Policy

**Last updated: 23 November 2026**

This policy is published at [addefense.me/privacy](https://addefense.me/privacy/). The [Terms & Conditions](https://addefense.me/terms/) are on the same site.

---

## 1. Who We Are / Contact

Ad Defense (formerly AdImmunity) is a Chrome browser extension that blocks ads, trackers and pop-ups, removes unwanted page weight, and can show web pages in dark or other colours you choose. It is developed and maintained by an independent maker based in the United States.

If you have any questions about this Privacy Policy, please contact us at:

**Email:** support@addefense.me

We will respond to all privacy-related enquiries within a reasonable time, and no later than 30 days for requests under applicable data protection law.

---

## 2. Summary

Ad Defense is built with a privacy-first design. **Everything the extension does happens locally on your device.** The extension has no user accounts, does not require you to sign in, and does not send your browsing activity, personal information, or any usage data to us or to any third party.

We operate no servers that receive your data. There is no analytics and no telemetry of any kind. There is nothing to sign up for; every feature works immediately and anonymously.

---

## 3. What Stays on Your Device

Ad Defense relies exclusively on local browser storage. The following is stored in your browser and **never transmitted to us or anyone else**:

- **Blocking statistics** — counts of ads, trackers, pop-ups and scripts blocked, including the on-device "all-time" totals. These are counts only. No record of *which* site a block happened on is ever kept.
- **Extension settings** — your master on/off toggle, the feature switches (cookie banners, the number on the toolbar icon, Turbo and each of its categories), and whether Page Colours is on and which colour you chose. Page Colours keeps no site names. Settings may sync across your own signed-in Chrome profiles via Chrome's built-in `chrome.storage.sync`; this is handled entirely by Google Chrome and is never sent to us.
- **Two small popup details, on this device only** — whether the popup itself is shown light or dark, and which "What's New" note you have already seen.
- **Short-lived items that are erased when you close Chrome.** The number shown on the toolbar icon for each tab is kept in Chrome's session storage; it is a count only, never the page's address. If you click **Load it** on a deferred embed, a temporary Chrome filter rule lets embeds from that provider load in that tab; it is also removed as soon as a new page loads in that tab or you close the tab.

What you hide with the **Element Zapper** is not stored at all: it lasts only while that page is open, and reloading the page brings everything back.

This data lives entirely on your device (or, for settings, within your own Google Chrome account). We have no access to it and no ability to retrieve it.

The blocking mechanism matches network requests against filter lists using Chrome's built-in `declarativeNetRequest` API, plus content scripts that hide ad elements. This happens entirely within your browser. **We do not intercept, log, or store the URLs you visit, the requests you make, or any other browsing data.**

The optional **Anonymous** tool simply reopens the current page in a standard Chrome Incognito window. It uses Chrome's built-in incognito mode (which you enable for the extension once in your browser's settings) and transmits nothing to us. Note that Incognito mode is a local browser feature; it does not make you anonymous to the websites you visit, your network, or your internet provider.

---

## 4. Network Requests

Ad Defense makes **no network requests of its own**. It downloads no lists, contacts no server (ours or anyone else's), and sends nothing about you anywhere. Its filter lists ship inside the extension and change only when the extension itself is updated through the Chrome Web Store.

Versions up to 1.9.0 downloaded a public phishing blocklist from URLhaus (abuse.ch) once a day. Those versions also remembered, until you closed Chrome, any site you chose to open anyway after a warning. Version 2.0 (November 2026) removed that feature, because the list's provider stopped offering free downloads. Chrome's own built-in Safe Browsing still warns you about dangerous sites. When you update, any copy of the old list stored on your device is deleted.

---

## 5. How Ad Defense Changes the Pages You Visit

Blocking ads means altering the page you are looking at. So that there is no surprise about what that involves, here is everything Ad Defense does to a page. All of it happens locally in your browser, and none of it is reported to us.

- **Hides and removes ad elements** — ad containers, sponsored placements, and the empty boxes left behind when an ad request is blocked are hidden with CSS or removed from the page.
- **Blocks network requests** to advertising and tracking hosts, using Chrome's `declarativeNetRequest` API.
- **Removes tracking parameters from links** — campaign tags and ad click identifiers (`utm_*`, `gclid`, `fbclid`, `msclkid` and similar) are stripped from links on the page and from the address bar. When you open a page that carries them, for example from a link in an email or another app, they are also removed from its address before the page is requested, so the site never receives them. Parameters that a site needs in order to work are deliberately **not** removed: this includes the recipient identifier on an unsubscribe or email-preference link, and affiliate attribution that pays the site you are visiting. Unsubscribe, email-preference and confirmation pages keep their whole address.
- **Dismisses cookie-consent banners** (optional, on by default, switchable under Settings → Options). When Ad Defense finds a recognised consent banner it clicks that banner's **"Reject"/"Decline"** button, or if there is none, its **close/dismiss** button. **It never clicks "Accept" or "Agree", and it never grants consent on your behalf.** If a banner offers neither a reject nor a close control, Ad Defense leaves it completely alone so that you can answer it yourself. Clicks are only ever sent to buttons inside a recognised consent banner, and never inside a login, sign-up, or payment form.
- **Skips video advertisements** by clicking a "Skip Ad" button when one appears, and by seeking past an ad break in a video player. On YouTube it also removes the ad instructions from the video player's data inside the page, so a video can start without its ad.
- **Keeps pages working when their ad code is blocked.** Some pages stop working when their advertising library is missing, so Ad Defense gives them harmless stand-ins that answer like the real library but load and show nothing. For one ad request that would otherwise break a news site's video player, Chrome is told to answer with an empty reply made inside your browser, so nothing is fetched.
- **Blocks pop-up windows** opened by known advertising and pop-under networks. Pop-ups from any other destination — including the ones payment and sign-in flows depend on — are allowed through.
- **Reports a neutral answer to ad-blocker detection scripts.** Some sites add a hidden decoy element purely to test whether a blocker is present. Ad Defense reports an ordinary size for those decoys. It does not alter measurements of any element that holds real content.
- **Shows web pages in dark or other colours you choose (Page Colours, a Beta feature, off until you switch it on).** While it is on, Ad Defense adds a colour filter to every website you visit. In Dark, light backgrounds turn dark grey and dark text turns light. With another colour, the page background takes that colour and the text turns light or dark so it stays readable; very strong colours are softened for the same reason. Photos, videos and video or map embeds are corrected back so they keep their colours. A site that already has dark colours of its own is normally recognised and left alone, and printing is not affected. Switching it on or off, or picking another colour, changes your open tabs at once, without a reload. While it is off, it does not run on any page, with one exception: when you open the popup's Page tab, the popup checks once whether the page in front of you is already dark (only its background and text colours are looked at, and nothing is kept or sent), and if it is, the switch cannot be turned on from that page.
- **Reloads the page you are looking at when you change a setting.** Turning Ad Defense on or off, or changing any feature switch, refreshes the current tab so the change takes effect immediately on the page in front of you. This is necessary because filtering rules only apply to requests a page makes *after* the change. (Page Colours and the number on the toolbar icon are the exceptions: they change without a reload.) Only the tab you are currently viewing is reloaded — never your other tabs — and nothing about the page is sent anywhere. **Note that a reload discards anything you have typed into a form on that page but not yet submitted**, so it is worth submitting or copying unsaved work before toggling a setting.

**Turbo (optional, off by default).** Turbo is a speed feature that blocks page extras which are not advertising. **Turbo itself is off until you switch it on.** The first time you do, Ad Defense switches on four of its five categories for you — Load videos on click, Hide chat bubbles, Block page experiments, and Ask for lighter pages — so that the switch does something you can see. **Use simple fonts (which blocks web fonts) is never switched on for you**, because it changes the way every page looks. You can change any of these at any time under Settings → Options, your choices are kept from then on, and this initial set-up happens only once. Each switch says what it costs you:

- **Load videos on click** — social, video and comment embeds (YouTube, Vimeo, Spotify, SoundCloud, Instagram, Facebook, X, TikTok, Reddit, Disqus, OpenWeb and similar) are not loaded with the page. Where Ad Defense can place one, you get a labelled placeholder with a **Load it** button; clicking it loads that embed, and lets others from the same provider load in that tab until a new page loads there or you close the tab. Where a provider already supplies its own visible fallback — X, TikTok, Reddit and LinkedIn leave the quoted post readable as text — that fallback is left in place instead of covering it with a placeholder. **Nothing is removed without either a placeholder or the provider's own visible fallback in its place.**
- **Hide chat bubbles** — live-chat and support widgets (Intercom, Drift, Zendesk, Tawk and similar). If a site's only support channel is its chat widget, you will need to turn this off to reach it.
- **Block page experiments** — experiment and tag-manager scripts (Optimizely, VWO, Google Tag Manager containers). A site running a visual experiment will show you its default version.
- **Ask for lighter pages** — adds the standard `Save-Data: on` header to outgoing requests, which tells sites you would prefer smaller images and video. It is a fixed value that contains no information about you and is the same for every user who enables it.
- **Use simple fonts** — skips font downloads. **This includes the site's own fonts, not only third-party ones**, so text will render in your browser's standard typefaces and pages will look visibly different.

Turbo never blocks anything needed to pay, sign in, or submit a form: payment providers, sign-in providers and CAPTCHA services are explicitly excluded, and this is enforced by an automated test.

Turning the master toggle off stops all of the above, Turbo included, and undoes it on pages you already have open: hidden ads and collapsed ad boxes reappear and deferred embeds are put back, without reloading those pages. What is not undone until you reload the page: a cookie banner Ad Defense already answered stays answered, links it already cleaned of tracking tags stay clean, elements you hid yourself with the Element Zapper stay hidden (Undo restores them), and an embed that loads through a script (such as a comment widget) keeps its "Load it" button.

---

## 6. The Permissions Ad Defense Asks For

Chrome shows you a permission list at install time. Here is what each one is for, and what it is *not* used for:

- **Access to all websites** — ads and trackers exist on virtually every site, so the filter rules and the ad-hiding scripts must be able to run anywhere. To do their job, those scripts look at the structure of the page inside your browser (for example, to recognise an ad box, a tracking tag in a link, a cookie banner or, for Page Colours, the page's colours). Nothing from the page is collected, kept or sent anywhere.
- **declarativeNetRequestWithHostAccess** — Chrome's own filtering engine. Rules are declared in advance and enforced by Chrome itself; the extension does not see the requests it blocks. Some of those rules also remove tracking tags from the address of a page you open, as described in Section 5. This is the narrower of the two available filtering permissions: it confines rule matching to sites you have already granted access to, rather than requesting the broader capability to filter without host access.
- **storage** — the settings (including Page Colours), statistics and popup details described in Section 3, plus one short-lived item in session storage that is erased when you close Chrome: the number shown on the toolbar icon for each tab.
- **alarms** — to run one hourly check that resets the daily statistics when the date changes.
- **webNavigation** — to notice when a tab moves to a new page, so that the number on the toolbar icon starts again from zero and any temporary "Load it" permission for that tab ends. Only the tab and its new address are used. The address is held in memory only, never saved, and nothing is sent anywhere.
- **scripting** — to register and unregister Ad Defense's own content scripts when you switch it on or off; to add them to tabs that are already open when you install or update it; to put the Element Zapper on a page when you activate it; to switch Page Colours on or off in your open tabs and change their colour; when you click **Load it** on a comment widget that a page loads with its own script, to put that page's own blocked script back on that page; and, when you open the popup's Page tab while Page Colours is off, to check once whether the page in front of you is already dark. That check looks only at the page's background and text colours, and nothing is kept or sent.

Ad Defense deliberately does **not** request the `tabs` permission. It reads the address of the tab you are actively viewing for three things only: to decide whether that tab can be refreshed after a setting change; on the Page tab, to tell you when it is a page Chrome lets no extension recolour; and, when you press **Anonymous**, to reopen that address in an Incognito window. When Page Colours is switched on or off or its colour changes, and when Ad Defense is installed or updated, it also finds your open web tabs so they change too, skipping pages Chrome does not let it change. These addresses are never saved or sent anywhere, and the website access above already covers this.

Ad Defense contains no remote code. Everything it runs is included in the package you install and reviewed by the Chrome Web Store.

---

## 7. What We Never Collect

Ad Defense **never** collects:

- Your browsing history or the URLs of pages you visit
- The content of any web page you view
- Search queries you enter
- Your name, email, phone number, or any account information (there are no accounts)
- Payment or financial information
- Location data
- Any persistent identifier tied to you or your browsing

We have no servers that receive your data, no analytics, and no telemetry. This is a foundational design principle of Ad Defense.

---

## 8. No Accounts, No Third-Party Processors in the Extension

Ad Defense has no login or sign-up. We do not use any third-party analytics, advertising, error-reporting, or database service that receives your data. The extension contacts no external endpoint at all (Section 4).

We do not sell or share personal information, and we do not use or transfer it for any purpose unrelated to the extension's single purpose — because we do not collect any.

**If you email us.** Messages you send to support@addefense.me reach us through our domain's email forwarding (provided by Namecheap) and are kept in our support inbox (Gmail, provided by Google). We see your email address and whatever you write, and use them only to answer you. You can ask us to delete your messages at any time.

---

## 9. Your Rights (GDPR / UK GDPR / CCPA-CPRA)

Because Ad Defense collects no personal data and holds nothing about you on any server, there is no extension data for us to access, correct, delete, or export. (If you have emailed us, you can ask us to delete those messages.)

- All on-device data (statistics and settings) is under your control. You can clear it at any time by removing the extension.
- Settings synced through your Google Chrome account are governed by Google's privacy policy and are managed from your Google account, not by us. You can delete them by resetting Chrome sync from your Google account's Chrome sync page (chrome.google.com/sync).

If you are in the EEA, UK, Switzerland, or California and have any question about your rights, contact us at support@addefense.me. You also have the right to lodge a complaint with your local data-protection supervisory authority.

---

## 10. Children

Ad Defense is a general-audience extension that collects no personal information from anyone, including children. It is not directed to children, and because there are no accounts and no data collection, no personal information from any user — of any age — is ever gathered.

---

## 11. Changes to This Policy

We may update this Privacy Policy to reflect changes in the extension's features or applicable law. When we make a material change, we will update the "Last updated" date at the top of this document and, where reasonably practicable, note it within the extension.

The version history of this document is available in the extension's public GitHub repository.

**Last updated: 23 November 2026**
