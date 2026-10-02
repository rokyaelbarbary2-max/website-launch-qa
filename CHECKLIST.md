# Website launch QA checklist

Tick items as they are verified on the **live** site, not on staging, unless the item says otherwise.

## 1. Ownership and rollback

- [ ] One named person decides "go / no go" on launch day.
- [ ] Each section of this checklist has an owner.
- [ ] A full backup of the current site and database exists, and someone has confirmed it can be restored.
- [ ] The rollback steps are written down, with an estimate of how long they take.
- [ ] Launch is not scheduled on the last working day before a weekend or holiday.

## 2. Content and copy

- [ ] No placeholder text remains ("Lorem ipsum", "Heading", "TBD", "111111", sample prices).
- [ ] Prices, phone numbers, addresses and opening hours match what sales and support use.
- [ ] Legal pages (privacy, terms, cookies) exist and are linked from every page.
- [ ] Every page has a unique, descriptive title and meta description.
- [ ] Images have alt text that describes them; decorative images have empty alt text.
- [ ] The 404 page is helpful: it explains the problem and links to the main sections.

## 3. Forms and lead handling

- [ ] Every form has been submitted at least once on the live site, from a phone and a desktop.
- [ ] Each test submission arrived where it should (CRM, inbox, sheet), with all fields intact.
- [ ] Required fields, validation messages and error states make sense to someone who did nothing wrong.
- [ ] The thank-you message or page explains what happens next and when.
- [ ] Spam protection is on, and it does not block real people using common browsers.
- [ ] Auto-replies and notification emails come from a monitored address and do not land in spam.
- [ ] Test submissions are removed or labelled so they do not pollute reports.

## 4. Analytics, tags and consent

- [ ] Analytics is installed once per page (no duplicate tags from both a plugin and a tag manager).
- [ ] Key events (form submit, call click, purchase, sign-up) fire once per action, on the live domain.
- [ ] Ad platform conversion tags fire on the same actions and are not double-counting.
- [ ] Internal and test traffic is filtered or clearly marked.
- [ ] The consent banner works as the law in your markets requires: tags that need consent do not fire before it.
- [ ] UTM-tagged links from live campaigns still land on working pages.

## 5. Search engines

- [ ] The staging block is removed: no site-wide `noindex`, and `robots.txt` does not contain `Disallow: /`.
- [ ] Every old URL that changed has a single permanent (301) redirect to its closest new equivalent, not to the homepage.
- [ ] A sample of old URLs (top traffic pages and pages with external links) has been tested on the live site.
- [ ] Canonical tags point to the live domain, not staging.
- [ ] The XML sitemap lists only live, indexable URLs and has been submitted in Search Console.
- [ ] Internal links point directly to final URLs, not through redirects.
- [ ] Structured data on key templates validates without errors.

## 6. Performance

- [ ] The homepage and the main landing pages have been tested on a mid-range phone over a mobile connection.
- [ ] The largest image on each key page is compressed and correctly sized.
- [ ] Fonts and hero images do not cause the layout to jump as the page loads.
- [ ] Third-party scripts (chat, heatmaps, widgets) are only on the pages that need them.
- [ ] Caching and a CDN are configured, and a cache purge has been tested.

## 7. Accessibility

- [ ] Every page can be used with a keyboard alone, with a visible focus indicator.
- [ ] Form fields have labels that stay visible while typing.
- [ ] Text has enough contrast against its background, including text on images.
- [ ] Headings follow a logical order and each page has one main heading.
- [ ] Videos have captions; audio has a transcript.

## 8. Arabic / English and right-to-left layouts

- [ ] Each language has its own URL, and pages link to their translation.
- [ ] `hreflang` tags are present and reciprocal between language versions.
- [ ] Arabic pages use `dir="rtl"`; layout, icons that imply direction, and carousels are mirrored correctly.
- [ ] Icons that should not be mirrored (logos, media controls, checkmarks) are not.
- [ ] Numbers, prices, dates and phone numbers display correctly in both languages.
- [ ] Forms accept Arabic input and the CRM stores it without corrupting characters.
- [ ] Arabic titles, descriptions and alt text are written natively, not machine-translated and left unchecked.

## 9. Launch day

- [ ] DNS, SSL certificate and the `www` / non-`www` redirect are correct.
- [ ] Redirects are deployed together with the new site.
- [ ] The live site has been crawled and every 404 or redirect chain found has been fixed or logged.
- [ ] Forms, tracking and consent have been re-tested on the live domain.
- [ ] Someone is available for the next few hours to fix urgent problems.

## 10. First week after launch

- [ ] Leads per day are compared with the weeks before launch; a sudden drop is investigated the same day.
- [ ] Search Console coverage and crawl errors are checked daily.
- [ ] Pages that previously brought traffic are checked for drops and missing content.
- [ ] Feedback from sales, support and real users is collected in one place.
- [ ] Anything skipped on launch day has an owner and a date.
