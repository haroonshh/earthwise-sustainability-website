# EarthWise — Sustainability & Climate Action Website

A group website built for the Web Design and Development module (University of Westminster), focused on SDG 13: Climate Action. Built as a 4-person team ("Team Green") sharing a common template and design system, with each member responsible for specific pages.

## My contribution (Student 3)

I was responsible for three pages plus their supporting documentation:

- **Feedback page** — a scrollable directory of sustainability programmes, a ratings/reviews grid, and a feedback form with JavaScript validation
- **Team page** — an interactive grid of team member cards with hover/focus-triggered expanding detail panels
- **Content page** — an SDG 13 climate action article with an in-page anchor navigation menu and a fixed "go to top" button

## Feedback page — what it does

- Displays a scrollable list of sustainability programmes (community clean-ups, tree planting, green travel, campus sustainability club) using a max-height container with `overflow-y: scroll`
- Shows a ratings summary and a responsive grid of user reviews using CSS Grid (`repeat(auto-fit, minmax(...))`) so it reflows without media queries
- Includes a feedback form (name, email, phone, address, topic, comment, visit date/time) built with semantic `fieldset`/`legend` grouping for accessibility
- JavaScript live character counter on the comment field, updating as the user types
- JavaScript validation on submit — checks name, email format, and comment aren't empty, shows inline error messages, and displays a confirmation box on success (all client-side, no page reload)

## Team page — what it does

- CSS Grid layout of team member cards, each showing a photo and role
- Hover and keyboard-focus (`tabindex`) triggered detail panels that expand via `max-height` transitions — accessible to keyboard users, not just mouse hover
- Documents each team member's role and contribution (template/home/gallery, splash screen/simulator, feedback/team/content, profile/sitemap)

## Content page — what it does

- An article on SDG 13 (Climate Action) split into five sections: introduction, why it matters, what students can do, real-world examples, and further resources
- In-page anchor navigation lets users jump directly to any section
- A fixed "go to top" button (pure CSS/HTML, no JavaScript) using `position: fixed` and an anchor link back to the top of the page
- Card-style content sections with consistent shadow/radius styling matching the site's design system

## Tech used

- HTML5 (semantic elements: `section`, `fieldset`, `legend`, `nav`)
- CSS3 — Flexbox, CSS Grid, `position: fixed`, hover/focus transitions, responsive layout without media queries where possible
- Vanilla JavaScript — DOM manipulation, event listeners, form validation
- Shared global stylesheet (`styles.css`) and shared page template built by another team member, extended with page-specific embedded styles

## Notes

- All pages share a common header, navigation, and footer from the team's shared template
- Validation and page-editor documentation pages (`validation_ST3.html`, `pageEditor_ST3.html`) contain before/after accessibility and validation screenshots and a technical write-up of each page's implementation
