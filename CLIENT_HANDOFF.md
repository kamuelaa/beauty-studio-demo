# Studio Muse beauty demo — owner setup

This is a SAMPLE brand, not a confirmed business. Built independently from `kamuelaa/website-master-template-6.` (source tree `7ef2dee897b5262b919d310011b2169b189de6d1`). The master was read only. Architecture retained: root HTML/CSS/JS, JSON content under `content/`, `.pages.yml`, uploaded photos in `images/`. No framework, build dependency, paid service, live booking, or ownership transfer.

## Pages CMS editing
1. Visit https://app.pagescms.org and sign in with the GitHub account that has access to `kamuelaa/beauty-studio-demo`.
2. Allow Pages CMS access to this demo repository if prompted; select the repository and `main` branch. Do not select the master template.
3. Edit Homepage, Services, Photo Gallery, Business and Contact, About & Mission, Setmore Booking, Approved Reviews, and Booking Policies.
4. Upload approved photos with the image picker. Add descriptive alternative text. Use compressed WebP/JPEG files, ideally below 300 KB per image.
5. Save changes. Pages CMS commits the JSON and image changes to GitHub. Once Cloudflare Git deployment is connected, changes trigger a deployment; check its status before refreshing the website.

Only publish genuine reviews with permission and enable their approval checkbox. All default content is sample content. Static section labels and demo notices live in index.html and must be reviewed by the developer when converting to a real business site.

## Connect the client's Setmore account
1. The client creates and owns her Setmore account and configures services, prices, duration, staff, timezone, availability, booking rules, and any payment settings herself.
2. In Setmore, go to Settings > Booking Page and copy the HTTPS Booking Page URL.
3. Paste it into Pages CMS > Setmore Booking > Setmore booking URL. Keep `Owner approved live bookings` OFF during review.
4. After the owner confirms the account and authorizes live scheduling, enable the approval checkbox and save.
5. The demo preview control becomes an external Setmore booking link. Test service availability and timezone with the owner before public use.
6. Optional embed: paste an official Setmore iframe into `Optional Setmore iframe embed code`. Only an HTTPS iframe source on setmore.com or its subdomains is accepted. Scripts and other markup are never executed. Setmore widget snippets that contain only a script/button need developer adaptation; the direct booking link remains available.

Setmore help: https://support.setmore.com/en/articles/491016-add-the-book-now-button-to-your-website
Embed guidance: https://support.setmore.com/en/articles/490991-embed-your-booking-page-on-your-website
No account has been created and no real appointment has been made.

## Cloudflare Pages deployment — awaiting approval
Do not deploy until the user approves publication.
After approval, use the user's existing Cloudflare account > Workers & Pages > Create application > Pages > Connect to Git. Choose ONLY `beauty-studio-demo`, branch `main`, framework None, no build command, output directory `/` (repository root). Use a free available pages.dev project name. Verify the returned URL; do not assume availability. No domain or paid plan is needed.

Do not upload the local QA `dist` directory or `.openai` configuration to GitHub. Production files are at repository root. Git integration is needed for automatic CMS updates; direct-upload deployments require manual re-upload after each edit.

The preview has noindex in HTML, robots.txt and _headers. Keep these for the sample demo. For the approved real business launch, replace sample copy and notices; remove all three noindex restrictions; add the final canonical URL and social preview metadata. Never add fabricated ratings or structured-data reviews.

## Missing client information
- Confirmed business name, logo, colors, and preferred style.
- Owner name, introduction, story, mission, and any verified credentials she wants included.
- Final service categories, descriptions, prices, durations, and add-ons.
- Approved portrait and portfolio photographs, alt text, and permission to publish.
- Genuine review quotes, attribution, and publication approval.
- Address/service area, public email/phone, studio hours, and social links.
- Cancellation notice, deposits/refunds, rescheduling, late arrivals, no-shows, and preparation policies.
- Her Setmore Booking Page URL, configured account, timezone, and explicit approval to activate.
- Approval to publish this demo and final production approval later.

## Handoff and ownership
No transfer until the client approves the finished site and completes payment. After that, arrange the repository transfer, client-owned Cloudflare Pages connection, Pages CMS access, and client-owned Setmore account. No separate contact form is necessary here; email/telephone links become active when supplied. Formspree is not used.
