WOOP - Aptaclub AI Poop Checker Landing Page
=============================================

WHAT'S IN THIS FOLDER
----------------------
index.html            -> the landing page
assets/woop-poop-checker.png  -> the full page design (with updated final CTA)

HOW TO USE
----------
1. Unzip this folder anywhere.
2. Open index.html in a browser to preview it.
3. To publish it, upload the whole folder (index.html + assets/) to any web
   host (Netlify, Vercel, GitHub Pages, your own server, etc). No build step
   needed - it's plain HTML.

MAKING THE BUTTONS CLICKABLE TO YOUR REAL LINK
------------------------------------------------
The page design is a single image, so two invisible clickable areas ("hotspots")
have been placed on top of it, matching the position of:
  - the "TAKE THE HEALTH CHECK" button
  - the "TAKE THE TEST & ENTER THE LUCKY DRAW" button

Open index.html in a text editor and find this line near the bottom:

    window.location.href = 'https://your-health-check-url.com';

Replace 'https://your-health-check-url.com' with the real URL of your
health-check form / quiz / lucky draw page. Both buttons currently point to
the same destination - change the two hotspot hrefs separately in the HTML
if you want them to go to different pages.

CHECKING THE HOTSPOT POSITIONS
--------------------------------
The clickable zones are positioned using percentages so they stay aligned
with the buttons on any screen size. If you ever edit the image and the
buttons move, you can temporarily uncomment this line in the <style> block
to see the clickable areas highlighted in green:

    /* background: rgba(0,255,0,0.25); */

Then adjust the top / left / width / height percentages under .cta-primary
and .cta-final to match the new button positions, and re-comment that line.

NOTES
-----
- This is a single-image landing page (fast to ship), not a fully coded
  HTML page with live text/fonts. If you'd like a true coded version
  (real HTML text, editable copy, animations, form fields, etc. instead of
  one big image) just ask and it can be built out section by section.
