# Portfolio Site Test Cases

Date: 2026-03-27
Scope: `nissanth-portfolio.html`

## Execution Summary
- Total test cases: 10
- Passed: 10
- Failed: 0

## Test Cases

### TC-01 Page load
- Steps:
  1. Open `nissanth-portfolio.html` in browser.
- Expected:
  - Page loads without blank screen or broken layout.
- Result: PASS

### TC-02 HTML document structure
- Steps:
  1. Check file contains doctype and closing `head`, `body`, `html` tags.
- Expected:
  - All required structural tags are present.
- Result: PASS

### TC-03 Internal navigation targets
- Steps:
  1. Collect all nav links with `href="#..."`.
  2. Confirm each target ID exists in page.
- Expected:
  - No missing section IDs.
- Result: PASS

### TC-04 Local asset availability
- Steps:
  1. Collect local `src`/`href` references.
  2. Verify each file exists in workspace.
- Expected:
  - No missing local assets.
- Result: PASS

### TC-05 Hero section visibility
- Steps:
  1. Open top of page.
  2. Check name, role line, and intro text are visible.
- Expected:
  - Hero content readable on dark background.
- Result: PASS

### TC-06 About section readability
- Steps:
  1. Scroll to About section.
  2. Verify paragraph text and highlighted bold words are readable.
- Expected:
  - Paragraphs are white; bold highlights use accent color.
- Result: PASS

### TC-07 Projects section text contrast
- Steps:
  1. Scroll to Projects cards.
  2. Verify heading and body text color contrast.
- Expected:
  - Headings are accent color; other text is white and readable.
- Result: PASS

### TC-08 Achievements section text contrast
- Steps:
  1. Open Certifications and related cards.
  2. Check headings and list text readability.
- Expected:
  - Headings are accent color; list text is white.
- Result: PASS

### TC-09 Background section text contrast
- Steps:
  1. Scroll to Background cards.
  2. Verify heading and supporting text readability.
- Expected:
  - Headings are accent color; other text is white.
- Result: PASS

### TC-10 Contact section readability
- Steps:
  1. Scroll to Contact section.
  2. Verify heading, description, contact links, and icons are visible.
- Expected:
  - Heading in accent color; remaining text in white.
- Result: PASS

## Risk/Limitations
- External CDN resources (fonts/Tailwind) depend on internet connectivity.
- Functional form submission is not validated because no backend endpoint is configured.
