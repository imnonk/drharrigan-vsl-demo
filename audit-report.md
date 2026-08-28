# Opt-In Page Audit Report
## Dr. Tim Harrigan — Signature Blueprint Protocol VSL Page
**Page URL:** https://drtim.drharrigan.ai/optin-page-5094-6518-9619-6275
**Audit Date:** August 29, 2026
**Prepared by:** BizEx

---

## EXECUTIVE SUMMARY

The opt-in page is a functional GHL-hosted landing page that communicates the core message well. It has a clear headline, reasonable copy structure, and the Synergy Wellness branding is visible. However, several critical technical and conversion issues were found, including placeholder content visible on the live page, missing alt text across all images, broken heading hierarchy, an unlinked Terms of Service, and copy inconsistencies with the VSL script. A demo rebuild has been prepared addressing all findings.

---

## SECTION 1: TECHNICAL AUDIT

### 1.1 Page Title
- **Current:** `Opt-in |` (incomplete, cuts off)
- **Issue:** Title tag is truncated. Missing the practice name and keyword context.
- **Recommended:** `Watch Free: The Signature Blueprint Protocol | Dr. Tim Harrigan`

### 1.2 Meta Description
- **Current:** `Helping Entrepreneurs and Parents Revitalize Health, End Fatigue and Brain Fog`
- **Issue:** This is a copy of the H1, not a purpose-built meta description. No call to action. No mention of the video or consultation offer.
- **Recommended:** `Discover why conventional labs miss the real cause of your fatigue, brain fog, and hormonal struggles. Watch Dr. Harrigan's free video and book your Blueprint Consultation.`

### 1.3 Open Graph Tags
- **Current:** Not detected on the page.
- **Issue:** No OG title, description, or image. Social shares will render poorly with no preview image or description.
- **Action:** Add `og:title`, `og:description`, `og:image`, `og:type`, and `og:url` to the page `<head>`.

### 1.4 Heading Structure (Critical)
The page has a broken heading hierarchy. Multiple H1 tags are in use simultaneously, and there are H1s appearing below H2s, which is semantically incorrect and hurts SEO.

**Findings:**
- `H2: BEYOND THE STREETLIGHT:` (appears before any H1 — wrong order)
- `H1: Helping Entrepreneurs and Parents...` (correct main H1)
- `H1: If you've ever:` (should be H3 or a styled list intro, not H1)
- `H1: ...it's time to look beyond the streetlight` (should be paragraph text)
- `H1: and find real answers.` (same — paragraph text, not a heading)
- `H1: Your breakthrough begins right here.` (should be H2 or H3)
- `H1: What You'll Learn In This Video` (duplicate section — hidden section below the fold with Lorem Ipsum content)
- `H1: Lorem ipsum odor amet,` (six instances — live placeholder text on production page)
- `H1: - Best name ever` / `H1: - Name ipsum` (placeholder testimonial names visible to real visitors)

**Rule:** One H1 per page. Heading order must be H1 then H2 then H3. Headings are not for styling — use CSS classes instead.

### 1.5 Placeholder / Lorem Ipsum Content (Critical)
Live production page has visible Lorem Ipsum content and placeholder testimonials:
- 6x `Lorem ipsum odor amet,` blocks in the "What You'll Learn In This Video" section
- Testimonial names: "Best name ever" and "Name ipsum" visible to real visitors
- These are unfilled GHL template elements that should be removed or filled before the page is used in campaigns

### 1.6 Image Alt Text
- **Current:** All 11 images have empty `alt=""` attributes.
- **Issue:** Meaningful images (Dr. Harrigan photo, Synergy Wellness logo) must have descriptive alt text. Only decorative images should have empty alt. This affects accessibility and image SEO.
- **Action:** Add descriptive alt text to all meaningful images.

### 1.7 Terms of Service Link
- **Current:** `Terms of Service` button in the footer links to `#` (the current page, no destination).
- **Issue:** Broken link. Visitors clicking Terms of Service get no page.
- **Action:** Link to the actual Terms of Service document or remove the link.

### 1.8 Copyright Year
- **Current:** `Copyright 2026. Synergy Wellness.`
- **Status:** Correct for 2026.

---

## SECTION 2: CONVERSION AUDIT

### 2.1 CTA Clarity
- **Current CTAs:** "REGISTER AND WATCH," "Watch the Video Now," "WATCH NOW!," "Click to get instant access!"
- **Issue:** Four different CTA button labels for what appears to be the same action. Inconsistent messaging creates decision friction and reduces click-through rate. The page should use one primary CTA phrase consistently.
- **Recommended primary CTA:** "Watch the Free Video" or "Watch Now" (consistent throughout)
- **Secondary CTA (below video):** "Book My Free Blueprint Consultation" pointing to the booking link

### 2.2 CTA Destination
- **Current:** The main CTA buttons do not visibly link to the VSL or an opt-in form. No GHL form is embedded and no booking URL is active on the page.
- **Issue:** Visitors who click the CTA have no clear next step presented.
- **Action:** Embed the GHL opt-in form above the fold, or point CTAs directly to `https://l.bttr.to/dSSt6` (the booking link from the VSL script).

### 2.3 Above-the-Fold Experience
- The hero has a strong headline and clear subheadline.
- The CTA button is visible without scrolling on desktop.
- The hero does not show the video or a video thumbnail above the fold. Adding a video thumbnail with a play button above the fold would increase engagement.

### 2.4 Opt-In Form
- **Current:** No opt-in form is visible on the page.
- **Issue:** The page is labeled an "opt-in page" but captures no contact information. If the goal is to collect leads, a name and email form must be present, ideally above the fold.
- **Action:** Embed GHL form or link to GHL form page. Confirm with Dr. Tim whether this is a direct-to-video page or a lead capture page.

### 2.5 VSL Integration
- **Current:** No video is embedded on the page. The Vimeo VSL link (vimeo.com/1078021215) from the script is not shown.
- **Issue:** The page is titled an opt-in page for a video but the video is not on the page.
- **Action:** Embed the Vimeo video directly on the page. The CTA should appear below the video and scroll the user down to the booking form.

### 2.6 Urgency and Scarcity
- **Current:** No urgency or scarcity element present.
- **Note:** Do not add false urgency ("limited seats," "offer expires tonight") for a recorded video. Any urgency used must be factually accurate.
- **Acceptable option:** "Limited consultation slots available each week" if Dr. Tim confirms this is true.

### 2.7 Social Proof
- **Current:** Client Success Stories section exists on the page but the testimonial placeholders are not filled ("Best name ever," "Name ipsum").
- **VSL script confirms real patient stories:** Keith (entrepreneur, lost 30 lbs in 90 days), Tish (75 years old, better than her 40s), Sarah (son's health transformation).
- **Action:** Replace placeholder testimonials with the real stories from the VSL script. Dr. Tim to confirm written consent to publish these publicly.

---

## SECTION 3: BRAND CONSISTENCY

| Element | Current Page | Brand Standard |
|---|---|---|
| Primary color | Blue (#teal) | Navy #003B5C |
| Accent color | Blue/teal buttons | Gold #C9A84C |
| Font (headings) | System serif | Georgia or equivalent |
| Logo shown | Yes (Synergy Wellness) | Correct |
| Dr. Tim name format | "Dr. Tim Harrigan, D.C., B.Sc." | Correct |
| Credentials label | "Root-Cause Health Pioneer" | Acceptable |

**Finding:** The page uses a teal/blue color scheme rather than the confirmed navy and gold brand colors. While not a blocking issue, it creates visual inconsistency compared to the naturalhealthtucson.com site and the other demo pages prepared for this campaign.

---

## SECTION 4: COPY AUDIT

### Strengths
- Strong hook: "Helping Entrepreneurs and Parents Revitalize Health, End Fatigue and Brain Fog"
- Clear avatar identification (entrepreneurs, busy parents, hormone patients)
- The "if you've ever" symptom list is effective and matches the VSL script
- Dr. Tim's credentials and bio are present and accurate
- The three root causes (Deficiency, Toxicity, Imbalance) are clearly stated
- Disclaimer / results-vary language is present in the success stories section

### Issues Found
- Em dashes present in body copy: "one-size-fits-all health solutions fail—and how Dr. Harrigan's protocol" and similar instances. Remove all em dashes per brand writing rules.
- "Life-Changing Video" in a subheading is a superlative claim without factual basis. Rephrase to something specific.
- "helped thousands" appears without a source or qualifier. Either confirm this number or soften to "has helped patients across the country."
- The "Beyond the Streetlight" concept is mentioned in the headline but not explained anywhere on the page. A one-sentence explanation would anchor the metaphor.

---

## SECTION 5: SUMMARY OF FINDINGS

**Critical (fix before running traffic):**
1. Remove all Lorem Ipsum placeholder content
2. Replace "Best name ever" and "Name ipsum" testimonial placeholders with real patient stories
3. Fix the Terms of Service link (currently points to `#`)
4. Embed the VSL video on the page
5. Add or connect an opt-in form if this is a lead capture page

**High Priority:**
6. Fix heading hierarchy (multiple H1s, wrong order)
7. Add descriptive alt text to all meaningful images
8. Unify CTA label to one consistent phrase
9. Add Open Graph meta tags for social sharing
10. Fix the page title tag

**Recommended:**
11. Switch button and accent colors to brand gold (#C9A84C)
12. Add booking link (l.bttr.to/dSSt6) as the post-video CTA
13. Remove em dashes from body copy
14. Soften unqualified superlatives ("thousands," "life-changing")

---

## WHAT WAS BUILT

A full demo replacement page has been prepared at:
`/vsl-optin-demo/index.html`

The demo addresses all critical and high-priority findings:
- Correct Navy + Gold brand colors
- Single clear H1, proper heading hierarchy
- Real patient testimonials from the VSL script (Keith, Tish, Sarah)
- Video embed placeholder with correct Vimeo link noted
- Booking CTA pointing to `https://l.bttr.to/dSSt6`
- Pain points, root cause framework, and bio sections in proper reading order
- All em dashes removed
- Alt text placeholders marked for Dr. Tim's actual photos
- Copyright 2026, correct practice address and phone number in footer
- Disclaimer language included below testimonials
- No Lorem Ipsum or placeholder content visible

**Still needed from Dr. Tim to finalize:**
- Headshot photo file (for bio section)
- Actual logo file (PNG with transparent background)
- Vimeo embed approval (currently linked but commented out pending confirmation)
- Confirmation of GHL opt-in form embed code (if lead capture is the goal)
- Written consent confirmation for patient testimonial names published publicly

---

*Prepared by BizEx | August 29, 2026*
