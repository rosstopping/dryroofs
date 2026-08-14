# Copilot website build

Create a production-quality marketing website for **Dry Roofs**, operating in the **Roofing** sector.

## Business brief

With over 30 years of expertise, Dry Roofs is dedicated to providing top-quality roofing solutions for homes and businesses in South Yorkshire. No matter the size of the project, we bring focus, skill, and attention to detail to deliver exceptional results every time.

Our comprehensive services include everything from complete roof replacements and flat roof installations, such as GRP, fibreglass, and felt, to minor roof repairs and maintenance. Whether you’re planning a major roofing project or need assistance with smaller repairs, Dry Roofs has you covered.

We pride ourselves on delivering reliable, professional service, with all work carried out to the highest standards and backed by a guarantee for your peace of mind. For all your roofing needs, trust Dry Roofs to provide a solution tailored to you.

Replacement Roofing

We specialise in professional roof replacement services, offering durable and high-quality solutions to suit your needs. Whether replacing a worn-out roof or upgrading to a modern design, our experienced team ensures a seamless and reliable service from start to finish.
Flat Roofing

We offer expert flat roof replacement services, tailored to your needs. Whether you require firestone, rubber, GRP, fibreglass, or felt roofing, our skilled team delivers durable and professional results. Trust us for a seamless and reliable flat roof upgrade.
Roofing Repairs

We provide expert roofing repair services to keep your roof in top condition. From minor leaks to more extensive damage, our skilled team ensures quick, reliable, and cost-effective solutions to protect your home and restore your roof’s integrity.

Required pages: Home, About, Services, Blog, Gallery, Contact.

## Creative direction

- Design a distinctive, fully fledged visual identity specifically informed by the Roofing industry. Do not produce a generic SaaS landing page.
- Establish an intentional colour system, typography hierarchy, spacing rhythm, imagery direction, and reusable component language.
- Use strong art direction, considered responsive composition, polished navigation and footer, meaningful page transitions or restrained interaction where helpful, and varied editorial layouts.
- Write useful British-English page copy based only on the supplied brief. Do not invent awards, certifications, locations, people, prices, statistics, testimonials, clients, or guarantees.
- Every requested page must have substantial, differentiated content and a clear conversion path.

## Required implementation

- Keep Eleventy as the static-site generator and Tailwind CSS v4 as the styling system.
- Use the existing CSS-first Tailwind setup with `@import "tailwindcss"`; do not add a legacy `tailwind.config.js` or deprecated v3 utilities.
- Build reusable Nunjucks layouts/components and data-driven navigation. Use clean semantic HTML.
- Make the result responsive from small phones through large screens, keyboard accessible, WCAG-conscious, and respectful of reduced-motion preferences.
- Add unique page titles, meta descriptions, canonical-ready URLs, Open Graph metadata, favicon treatment, and appropriate structured data supported by the brief.
- Optimise image dimensions/loading and avoid layout shift. Use properly licensed remote imagery only when the source and licence are clear; otherwise use art-directed CSS/SVG treatments.

## Lead form — mandatory

The Contact page must contain this functional form contract exactly:

```html
<form method="POST" action="https://sitewell.digizu.co.uk/submit">
  <input type="hidden" name="_form_name" value="Contact form">
  <div class="..." style="position:absolute;left:-9999px;width:1px;height:1px;overflow:hidden" aria-hidden="true">
    <label>Leave this field empty<input type="text" name="_honeypot" tabindex="-1" autocomplete="off"></label>
  </div>
  <label>Name<input type="text" name="name" required></label>
  <label>Email<input type="email" name="email" required></label>
  <label>Message<textarea name="message" required></textarea></label>
  <button type="submit">Send enquiry</button>
</form>
```

The fields may be visually composed with Tailwind classes, but do not change the action, method, hidden field, honeypot name, or public field names.

## Completion checklist

1. Implement every requested page and all shared components.
2. Run `npm install`, `npm run build`, and `npm run check`.
3. Resolve all build errors, broken internal links, missing assets, overflow, and obvious accessibility issues.
4. Keep generated `_site` output uncommitted.
5. Open a pull request summarising the visual concept, page structure, form integration, and verification performed.