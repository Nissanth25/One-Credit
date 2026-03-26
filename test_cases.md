# Test Cases for Nissanth Portfolio Website

## Test Suite Overview
This document outlines comprehensive test cases for the portfolio website (nissanth-portfolio.html). Tests are organized by functionality and user scenarios.

---

## 1. Navigation & Header Tests

### TC-001: Navigation Links Functionality
**Description:** Verify all navigation links work correctly  
**Steps:**
1. Load the website
2. Click on each navigation link (About, Skills, Projects, Achievements, Contact)
3. Observe page scroll behavior

**Expected Result:** 
- Each link scrolls smoothly to corresponding section
- Correct section is highlighted in view

**Status:** ⏳ To Be Tested

---

### TC-002: Logo Click Navigation
**Description:** Verify logo redirects to home section  
**Steps:**
1. Scroll to middle of page
2. Click on "nissanth.sp" logo
3. Observe page behavior

**Expected Result:** 
- Page scrolls smoothly to hero section
- Logo link works as home anchor

**Status:** ⏳ To Be Tested

---

### TC-003: Navigation Bar Visibility
**Description:** Verify navigation bar remains fixed at top  
**Steps:**
1. Load website
2. Scroll down multiple times
3. Observe navigation bar position

**Expected Result:** 
- Navigation bar stays fixed at top
- Content scrolls behind it
- Backdrop blur effect visible

**Status:** ⏳ To Be Tested

---

## 2. Hero Section Tests

### TC-004: Hero Text Animation
**Description:** Verify hero title and text animations work  
**Steps:**
1. Load website
2. Observe hero section text
3. Check for fade-in animations

**Expected Result:** 
- "Nissanth S P" title animates in smoothly
- Role text changes dynamically with typing effect
- CTA buttons appear with animation

**Status:** ⏳ To Be Tested

---

### TC-005: Dynamic Role Text
**Description:** Verify role text cycles through different roles  
**Steps:**
1. Load website
2. Wait for 3+ seconds
3. Observe role text changes

**Expected Result:** 
- Role text cycles through: "Building intelligent ML systems", "Detecting patterns in data", etc.
- Typing animation is smooth
- Text changes every ~3 seconds

**Status:** ⏳ To Be Tested

---

### TC-006: Hero CTA Buttons
**Description:** Verify call-to-action buttons work  
**Steps:**
1. Click "View Projects →" button
2. Click "LinkedIn ↗" button
3. Click "Codolio ↗" button

**Expected Result:** 
- View Projects scrolls to projects section
- LinkedIn opens in new tab
- Codolio opens in new tab
- External links have correct hrefs

**Status:** ⏳ To Be Tested

---

### TC-007: Scroll Cue Animation
**Description:** Verify scroll indication animation  
**Steps:**
1. Load website on hero section
2. Observe bottom-left corner

**Expected Result:** 
- Scroll cue appears with animated track
- Animation indicates scrolling is possible

**Status:** ⏳ To Be Tested

---

## 3. About Section Tests

### TC-008: About Card Display
**Description:** Verify about section card displays correctly  
**Steps:**
1. Scroll to about section
2. Check card content visibility

**Expected Result:** 
- Profile info card shows avatar (🧠 emoji)
- Name: Nissanth S P displays
- All contact info visible (email, phone, LinkedIn, etc.)

**Status:** ⏳ To Be Tested

---

### TC-009: Contact Links in About
**Description:** Verify contact links in about section work  
**Steps:**
1. Click on email link in about section
2. Click on phone link
3. Click on LinkedIn link

**Expected Result:** 
- Email link opens mail client
- Phone link initiates call/SMS
- LinkedIn opens in new tab

**Status:** ⏳ To Be Tested

---

### TC-010: Statistics Display
**Description:** Verify stats counter display  
**Steps:**
1. Scroll to about section stats
2. Observe numbers

**Expected Result:** 
- Shows "6 Projects"
- Shows "2 Internships"
- Shows "10+ Certs"
- All aligned in 3-column grid

**Status:** ⏳ To Be Tested

---

## 4. Skills Section Tests

### TC-011: Skills Grid Layout
**Description:** Verify skills section displays in grid  
**Steps:**
1. Scroll to skills section
2. Observe grid layout

**Expected Result:** 
- 7 skill cards displayed
- Auto-fit responsive grid
- Cards have proper spacing

**Status:** ⏳ To Be Tested

---

### TC-012: Skill Card Hover Effect
**Description:** Verify skill cards have hover animation  
**Steps:**
1. Scroll to skills section
2. Hover over a skill card
3. Observe animation

**Expected Result:** 
- Background color changes on hover
- Bottom border animates from left to right
- Smooth transition effect

**Status:** ⏳ To Be Tested

---

### TC-013: Progress Bar Animation
**Description:** Verify skill progress bars animate  
**Steps:**
1. Scroll into skills section view
2. Observe progress bars

**Expected Result:** 
- Progress bars fill from 0 to set percentage
- Animation triggers when card enters viewport
- Smooth easing animation

**Status:** ⏳ To Be Tested

---

### TC-014: Skill Tags Display
**Description:** Verify technology tags display correctly  
**Steps:**
1. View skills section
2. Check tag styling

**Expected Result:** 
- Tags show related technologies
- Proper color coding (accent vs cyan)
- Tags fit within card

**Status:** ⏳ To Be Tested

---

## 5. Projects Section Tests

### TC-015: Projects Grid Display
**Description:** Verify projects display in proper grid  
**Steps:**
1. Scroll to projects section
2. Observe layout

**Expected Result:** 
- 6 project cards displayed
- Auto-fit responsive grid
- Cards have consistent styling

**Status:** ⏳ To Be Tested

---

### TC-016: Project Card Hover Effect
**Description:** Verify project cards have hover animation  
**Steps:**
1. Scroll to projects
2. Hover over project card
3. Observe animation

**Expected Result:** 
- Card moves up slightly (translateY)
- Border color changes to accent color
- Top gradient line animates in
- Smooth transition

**Status:** ⏳ To Be Tested

---

### TC-017: Project Information Display
**Description:** Verify each project shows required info  
**Steps:**
1. View each of 6 projects
2. Check information completeness

**Expected Result:** 
- Project number (01-06) displays
- Project title with emoji displays
- 3-4 bullet points display
- Technology tags display

**Status:** ⏳ To Be Tested

---

### TC-018: Hospital Notification System Project
**Description:** Verify new hospital project displays correctly  
**Steps:**
1. Scroll to projects
2. Look for 6th project card

**Expected Result:** 
- Project 06 displays "🏥 Hospital Trip Notification System"
- Description mentions notifications and alerts
- Tags include: Python, Database, Notifications, Healthcare Tech

**Status:** ⏳ To Be Tested

---

## 6. Achievements Section Tests

### TC-019: Achievements Grid Display
**Description:** Verify achievements section displays  
**Steps:**
1. Scroll to achievements section
2. Observe layout

**Expected Result:** 
- 6 achievement items displayed
- Grid layout with auto-fit columns
- Proper spacing and borders

**Status:** ⏳ To Be Tested

---

### TC-020: Achievement Item Hover
**Description:** Verify achievement item hover effect  
**Steps:**
1. Hover over achievement item
2. Observe background change

**Expected Result:** 
- Background color changes slightly
- Icon and text remain readable
- Smooth transition

**Status:** ⏳ To Be Tested

---

### TC-021: Achievement Icons and Text
**Description:** Verify each achievement displays correctly  
**Steps:**
1. View all 6 achievements
2. Check icon and text display

**Expected Result:** 
- Icons display (🏆 📐 🚀 🖥️ ⚡ 🗄️)
- Title and description text visible
- Content is clear and readable

**Status:** ⏳ To Be Tested

---

## 7. Experience & Education Section Tests

### TC-022: Experience Cards Display
**Description:** Verify experience section layout  
**Steps:**
1. Scroll to experience section
2. Check card display

**Expected Result:** 
- 2 experience cards shown (Google Internship, Nexyuga)
- Cards in 2-column grid
- Proper styling with left border

**Status:** ⏳ To Be Tested

---

### TC-023: Experience Card Hover
**Description:** Verify experience card hover effect  
**Steps:**
1. Hover over experience card
2. Observe change

**Expected Result:** 
- Border color changes to accent
- Smooth color transition
- Left colored border visible

**Status:** ⏳ To Be Tested

---

### TC-024: Education Cards Display
**Description:** Verify education section displays  
**Steps:**
1. Scroll to education area
2. Check cards

**Expected Result:** 
- 2 education cards shown
- "B.E. — AI & ML" program displays
- "Interests & Hobbies" card displays
- Hobbies shown with badges

**Status:** ⏳ To Be Tested

---

### TC-025: Hobbies Display
**Description:** Verify hobbies badges display correctly  
**Steps:**
1. Find hobbies section
2. Check badge display

**Expected Result:** 
- 4 hobby badges visible
- Proper styling and spacing
- Hover effect on each badge

**Status:** ⏳ To Be Tested

---

## 8. Contact Section Tests

### TC-026: Contact Form Elements
**Description:** Verify contact form elements are present  
**Steps:**
1. Scroll to contact section
2. Check form elements

**Expected Result:** 
- Name input field visible
- Email input field visible
- Subject input field visible
- Message textarea visible
- Send button visible

**Status:** ⏳ To Be Tested

---

### TC-027: Contact Form Input Focus
**Description:** Verify form inputs have focus styles  
**Steps:**
1. Click on each form input
2. Observe focus state

**Expected Result:** 
- Border color changes to accent on focus
- Clear visual feedback
- Placeholder text visible

**Status:** ⏳ To Be Tested

---

### TC-028: Contact Info Links
**Description:** Verify contact info section links work  
**Steps:**
1. Click email link in contact info
2. Click phone link
3. Click LinkedIn link
4. Click Codolio link

**Expected Result:** 
- Email opens mail client
- Phone initiates call
- LinkedIn opens in new tab
- Codolio opens in new tab

**Status:** ⏳ To Be Tested

---

### TC-029: Send Button Styling
**Description:** Verify send button has proper styling  
**Steps:**
1. View send button
2. Hover over button

**Expected Result:** 
- Button has accent background color
- Hover effect: background changes
- Smooth transition
- Proper cursor appearance

**Status:** ⏳ To Be Tested

---

## 9. Custom Cursor Tests

### TC-030: Custom Cursor Display
**Description:** Verify custom cursor appears  
**Steps:**
1. Load website
2. Move mouse around
3. Observe cursor

**Expected Result:** 
- Custom cursor dot visible
- Cursor ring visible around cursor
- Both move smoothly with mouse

**Status:** ⏳ To Be Tested

---

### TC-031: Cursor Interaction on Interactive Elements
**Description:** Verify cursor scales on interactive elements  
**Steps:**
1. Move cursor over buttons
2. Move cursor over project cards
3. Move cursor over achievement items

**Expected Result:** 
- Cursor ring scales up (1.7x) on hover
- Ring color changes to accent
- Smooth animation

**Status:** ⏳ To Be Tested

---

## 10. Scroll & Animation Tests

### TC-032: Scroll Animation on Hero Elements
**Description:** Verify hero elements animate in on load  
**Steps:**
1. Load website
2. Observe hero section

**Expected Result:** 
- Eyebrow text fades in with slide up
- Hero name fades in with slide up
- Role text fades in with slide up
- CTA buttons fade in with slide up

**Status:** ⏳ To Be Tested

---

### TC-033: Intersection Observer Animation
**Description:** Verify elements animate in on scroll  
**Steps:**
1. Scroll page
2. Observe elements coming into view

**Expected Result:** 
- Elements fade and slide up as they enter viewport
- Different animation delays for .r, .r2, .r3, .r4 classes
- Smooth animations throughout

**Status:** ⏳ To Be Tested

---

### TC-034: Smooth Scroll Behavior
**Description:** Verify smooth scrolling works  
**Steps:**
1. Click navigation links
2. Observe scroll behavior

**Expected Result:** 
- Smooth scroll animation
- No jank or jumpy behavior
- Clean transition to target section

**Status:** ⏳ To Be Tested

---

## 11. Responsive Design Tests

### TC-035: Mobile Layout (< 600px)
**Description:** Verify mobile layout displays correctly  
**Steps:**
1. Set viewport to 375px width
2. Check layout

**Expected Result:** 
- Single column layout
- Navigation links stack or shrink
- Readable on mobile screen
- No horizontal scroll

**Status:** ⏳ To Be Tested

---

### TC-036: Tablet Layout (600-900px)
**Description:** Verify tablet layout displays correctly  
**Steps:**
1. Set viewport to 768px width
2. Check layout

**Expected Result:** 
- Grids adjust to single column
- Text sizes readable
- Proper padding and margins

**Status:** ⏳ To Be Tested

---

### TC-037: Desktop Layout (> 900px)
**Description:** Verify desktop layout displays correctly  
**Steps:**
1. Set viewport to 1920px width
2. Check layout

**Expected Result:** 
- Multi-column grids display
- Proper spacing on all sides
- Typography scales correctly

**Status:** ⏳ To Be Tested

---

### TC-038: Font Scaling
**Description:** Verify fonts scale with viewport  
**Steps:**
1. Test on different viewport sizes
2. Check font sizes

**Expected Result:** 
- Text uses clamp() for responsive sizing
- Text readable on all screen sizes
- No overflow or truncation

**Status:** ⏳ To Be Tested

---

## 12. CSS & Styling Tests

### TC-039: Color Scheme Consistency
**Description:** Verify color scheme is consistent  
**Steps:**
1. View entire page
2. Check color usage

**Expected Result:** 
- Dark blue background (#080810)
- Accent purple (#6c63ff) for highlights
- Cyan (#38bdf8) for secondary accents
- Light text (#e2e2f0) for readability

**Status:** ⏳ To Be Tested

---

### TC-040: Background Gradient Mesh
**Description:** Verify mesh background displays  
**Steps:**
1. Load page
2. Observe background

**Expected Result:** 
- Gradient mesh background visible
- Subtle animations
- Doesn't interfere with content readability

**Status:** ⏳ To Be Tested

---

### TC-041: Border Styling
**Description:** Verify borders display correctly  
**Steps:**
1. View all sections
2. Check border colors

**Expected Result:** 
- Borders use accent color with transparency
- Consistent border-radius (2px)
- Grid borders divide sections properly

**Status:** ⏳ To Be Tested

---

### TC-042: Shadow Effects
**Description:** Verify box shadows display correctly  
**Steps:**
1. View projects and skill cards
2. Check shadow effects

**Expected Result:** 
- Buttons have glow shadow effect
- Cards have subtle shadows
- Shadows change on hover

**Status:** ⏳ To Be Tested

---

## 13. Accessibility Tests

### TC-043: Keyboard Navigation
**Description:** Verify keyboard navigation works  
**Steps:**
1. Press Tab repeatedly
2. Navigate through all links
3. Press Enter on links

**Expected Result:** 
- All links are keyboard accessible
- Tab order is logical
- Focus visible on all interactive elements

**Status:** ⏳ To Be Tested

---

### TC-044: Color Contrast
**Description:** Verify text has sufficient contrast  
**Steps:**
1. Check text vs background contrast
2. Use contrast checker tool

**Expected Result:** 
- All text has WCAG AA contrast ratio
- Text is readable for color-blind users

**Status:** ⏳ To Be Tested

---

### TC-045: Link Identification
**Description:** Verify links are identifiable  
**Steps:**
1. View all links
2. Check styling differences

**Expected Result:** 
- Links are clearly identifiable
- Not just distinguished by color
- Hover states visible

**Status:** ⏳ To Be Tested

---

## 14. Cross-Browser Tests

### TC-046: Chrome Browser
**Description:** Verify site works in Chrome  
**Steps:**
1. Open in Chrome latest version
2. Test all functionality

**Expected Result:** 
- All features work correctly
- No console errors
- Animations smooth

**Status:** ⏳ To Be Tested

---

### TC-047: Firefox Browser
**Description:** Verify site works in Firefox  
**Steps:**
1. Open in Firefox latest version
2. Test all functionality

**Expected Result:** 
- All features work correctly
- No console errors
- Styling matches Chrome

**Status:** ⏳ To Be Tested

---

### TC-048: Safari Browser
**Description:** Verify site works in Safari  
**Steps:**
1. Open in Safari latest version
2. Test all functionality

**Expected Result:** 
- All features work correctly
- Animations work properly
- Layout correct

**Status:** ⏳ To Be Tested

---

### TC-049: Edge Browser
**Description:** Verify site works in Edge  
**Steps:**
1. Open in Edge latest version
2. Test all functionality

**Expected Result:** 
- All features work correctly
- Performance good
- Styling consistent

**Status:** ⏳ To Be Tested

---

## 15. Performance Tests

### TC-050: Page Load Speed
**Description:** Verify page loads quickly  
**Steps:**
1. Measure initial load time
2. Check Core Web Vitals

**Expected Result:** 
- First Contentful Paint < 1.8s
- Largest Contentful Paint < 2.5s
- Cumulative Layout Shift < 0.1

**Status:** ⏳ To Be Tested

---

### TC-051: Smooth Animations
**Description:** Verify animations perform well  
**Steps:**
1. Scroll through page
2. Check for any jank

**Expected Result:** 
- 60 FPS animations
- No stuttering or lag
- Smooth transitions

**Status:** ⏳ To Be Tested

---

### TC-052: Large Dataset Rendering
**Description:** Verify page handles many elements  
**Steps:**
1. Load full page with all content
2. Check rendering performance

**Expected Result:** 
- Page renders smoothly
- No memory leaks
- Efficient DOM updates

**Status:** ⏳ To Be Tested

---

## Bug Report Template

```
Bug ID: [Auto-assigned]
Title: 
Severity: [Critical | High | Medium | Low]
Browser: 
OS: 
Device: 
Steps to Reproduce:
1. 
2. 
3. 

Expected Result: 

Actual Result: 

Screenshots/Videos: 

Notes:
```

---

## Test Execution Summary

| Test Category | Total Tests | Passed | Failed | Status |
|--------------|------------|--------|--------|--------|
| Navigation | 3 | 0 | 0 | ⏳ Pending |
| Hero Section | 4 | 0 | 0 | ⏳ Pending |
| About Section | 3 | 0 | 0 | ⏳ Pending |
| Skills Section | 4 | 0 | 0 | ⏳ Pending |
| Projects Section | 4 | 0 | 0 | ⏳ Pending |
| Achievements | 3 | 0 | 0 | ⏳ Pending |
| Experience & Education | 4 | 0 | 0 | ⏳ Pending |
| Contact Section | 4 | 0 | 0 | ⏳ Pending |
| Custom Cursor | 2 | 0 | 0 | ⏳ Pending |
| Scroll & Animation | 3 | 0 | 0 | ⏳ Pending |
| Responsive Design | 4 | 0 | 0 | ⏳ Pending |
| CSS & Styling | 4 | 0 | 0 | ⏳ Pending |
| Accessibility | 3 | 0 | 0 | ⏳ Pending |
| Cross-Browser | 4 | 0 | 0 | ⏳ Pending |
| Performance | 3 | 0 | 0 | ⏳ Pending |
| **TOTAL** | **52** | **0** | **0** | **⏳ Pending** |

---

## Test Execution Notes

- All tests should be executed on latest browser versions
- Mobile testing requires actual devices or reliable emulators
- Performance tests should use DevTools
- Document any deviations from expected results
- Update status as tests are completed

**Test Date:** March 26, 2026  
**Tested By:** [Your Name]  
**Approved By:** [Reviewer Name]

---

## Recommendations

After completing tests:
1. Fix any critical or high-severity bugs immediately
2. Create GitHub issues for outstanding bugs
3. Document browser/device-specific workarounds
4. Plan performance optimization if needed
5. Schedule regression testing before major updates
