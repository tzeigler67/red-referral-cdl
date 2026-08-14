DRIVER TO DRIVER REFERRAL — PRODUCTION BUILD 3.1
================================================

Build 3.1 is a corrective and content-update release based directly on Production Build 2.

CHANGES
-------
- Tablet-only hero treatment now oversizes and left-anchors the image, physically extending
  it beyond the right edge. This keeps the tractor visible and crops the rear of the trailer.
- Phone presentation remains unchanged.
- Form submission now uses FormSubmit through an AJAX request instead of opening a mail app.
- Updated the opening Why I Refer Drivers sentence.
- Updated the company-growth paragraph.
- Added “Tiered driver certification program.”
- Swapped “Pass It Along” and “Know a Driver?” in the referral card.
- Updated referral supporting text to “Know a driver who might be looking?”

REQUIRED FORM CONFIGURATION
---------------------------
In index.html, replace this placeholder in the form action:

REPLACE-WITH-YOUR-EMAIL@example.com

with the address that should receive inquiries. The same action is used by script.js to send
the form through FormSubmit. FormSubmit may send a one-time activation email the first time
the endpoint is used. Complete that activation before relying on the form publicly.

GITHUB PAGES
------------
Upload the CONTENTS of this folder to the root of the GitHub Pages repository.
Do not upload the ZIP itself.


PRODUCTION BUILD 3.2 CHANGES
----------------------------
- Tablet hero image reduced from 118% to 106% width and shifted right so the full tractor remains visible while only the trailer's rear edge is cropped.
- FormSubmit CAPTCHA re-enabled. Successful validation now continues to FormSubmit's verification step before the email is delivered.

BUILD 3.3 HERO FIX
------------------
- The stylesheet has been renamed to style-build-3-3.css to bypass stale browser/CDN caches.
- Phones and portrait tablets now anchor the hero image to the left edge so the tractor's front is not cropped.
- Landscape tablets (900-1100 px) display the image at a smaller scale and place it to the right of the copy.
- The tractor remains visible and the rear portion of the trailer is allowed to fall outside the viewport.

After uploading, delete the prior style.css file from the live repository if it remains there.
A hard refresh may still be useful once: iPad Safari can be refreshed by closing the tab,
reopening the page, or clearing Website Data for the site in Safari settings.


BUILD 3.6.1 CHANGES
-----------------
- Moved the “Bonus $” callout beside Company-funded ESOP, Quarterly Profit-sharing, and Performance-based scorecard.
- Phone number is now required in both HTML and JavaScript validation.
- Email remains optional.
- Updated the instruction above the submission button.
- Renamed CSS and JavaScript files with Build 3.6.1 versioning to reduce stale browser caching.

Build 3.6.1 change: on phone layouts, the Bonus $ callout now stays beside the ESOP, quarterly profit-sharing, and performance scorecard rows instead of dropping below the full list.


Build 3.6.1 refinement:
- Enlarged and slightly raised the dollar sign in the handwritten “Bonus $” callout.


BUILD 3.6.3
-----------
Desktop-only hero correction: on screens 1101px and wider, the hero image is constrained to the right 58% of the hero so the tractor is no longer positioned beneath the left-side messaging. Mobile and tablet hero rules are unchanged.

PRODUCTION BUILD 3.9.0 HERO UPDATE
----------------------------------
Based on Build 3.6.4 with the following approved hero changes:
- Replaced hero truck asset with the newly approved warehouse-background truck image with fender number removed.
- Removed the six-item hero bullet list.
- Added Traig Zeigler portrait and centered caption: Traig Zeigler / Driver & Trainer.
- Moved existing introductory paragraph beside the portrait and increased its readable size.
- Reduced hero headline size.
- Desktop hero uses a strict split layout: 32% text / 68% truck image, with no overlap.
- Mobile and tablet portrait keep image-first/content-below composition.
- Tablet landscape retains split text/image composition.
All other Build 3.6.4 sections, content, form handling, CAPTCHA, and styling remain unchanged.


BUILD 3.9.0 ADDITIONS
---------------------
Obfuscated prize page: JPFb6AGDQxWrkcw8RQ6Dm0F3lpz1.html
Main form confirmation: main-confirmation.html
Prize claim confirmation: prize-confirmation.html

IMPORTANT BEFORE DEPLOYMENT
---------------------------
Deployment root URL configured as:
https://redreferralcdl.com/

Per instruction, the Main Form does NOT include the future conditional _cc address yet.
Prize claims submit to redreferral1952@gmail.com.
