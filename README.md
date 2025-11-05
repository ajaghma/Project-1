I organized the site around a simple top-nav plus “Modules” list on the home page so 
users can jump in two ways: browse linearly or go straight to a task. Each page keeps a 
clean heading hierarchy (site title → page title → section headings) and uses lightweight 
components—<aside> for tips/definitions and <figure> for screenshots with real alt 
text—so content stays scannable. One shared CSS file handles spacing, type scale, 
and card/aside styling to signal hierarchy without heavy decoration. The structure is 
intentionally boring: predictable folders, relative links, and a template page, which should 
make new modules easy to add later.

Trade-offs: I chose longer single pages with an on-page TOC instead of splitting into many 
subpages; that keeps context together but can feel scroll-heavy. With more time, I’d add a 
breadcrumbs pattern, print styles, dark mode, and a11y refinements (focus states, 
reduced-motion). Current accessibility steps include a skip link, consistent headings, 
keyboard-friendly nav, and descriptive alt text.
