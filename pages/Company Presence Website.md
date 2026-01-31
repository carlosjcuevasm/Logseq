## Don’t build a “GUI toolkit” first — build 3 templates first

This is the most important advice.

If you start by building a generic toolkit, you’ll spend weeks polishing buttons.

Instead:
- Build **Template 1** (most common business type)
- Extract reusable blocks into your kit
- Build **Template 2**
- Extract more blocks
- Build **Template 3**
  
  Your toolkit will naturally become the right toolkit — driven by real needs.
-
- ## What to include in your toolkit (MVP)
- ### Components / blocks
- Navbar (3 variants)
- Hero (5 variants)
- Feature list (3)
- Service cards (2)
- Product grid + product detail
- CTA (3)
- Testimonials (2)
- FAQ accordion
- Contact section + map embed
- Footer (2)
-
- ### System pieces (more important than components)
- Typography scale
- Spacing scale
- Responsive rules
- SEO defaults (OG tags, sitemap)
- Analytics hook
- Form handling + spam protection
- Image optimization pipeline
  
  These are what make delivery fast and consistent.
-
- ## One warning (so you don’t get burned)
  
  If you host Strapi per client, you’ll end up doing ops forever.
  
  Two good approaches:
- **Hosted CMS per client (Sanity, etc.)**
- **One “multi-tenant” CMS** (more complex, but scalable)
  
  Early stage: keep it simple. Just price maintenance.