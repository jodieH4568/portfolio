# Jodie Hemsill — Portfolio website specification

**Status:** Initial specification, following the first interview round.  
**Updated:** 25 October 2026.  
**Purpose:** Establish the intent, design constraints, content structure and build requirements. Detailed case-study content and several personal details remain to be supplied. This document authorises no deployment; the current deliverable is the specification.

## 1. Sources and decision precedence

Read alongside:

- `context/handwritten-portfolio-notes.md` — original thinking, capabilities and candidate projects.
- `context/gptchat.md` — prior design brief, approved hero direction and proposed content.
- `context/granola.md` — planning discussion, web CV, maintenance preferences and contact requirements.
- `context/techrequirements.md` — static hosting, performance and agent maintenance requirements.
- `context/mockupUI.png` — primary visual reference for the homepage.
- The interview in this chat — the latest clarification of purpose, audience and desired work.

The latest direct interview answers take precedence where earlier documents differ. Preserve the established visual direction unless Jodie requests a change. Recommendations in this specification are implementation defaults, not additional decisions Jodie has personally confirmed.

Use **Jodie Hemsill** throughout. Name variants in the meeting notes are transcription inconsistencies.

## 2. Purpose and desired outcome

The website is an asset alongside Jodie's existing CV. Its primary purpose is to differentiate her skills and support applications for existing, part-time contract marketing opportunities.

Priority roles:

- Contract social media management.
- Contract marketing management.
- Marketing strategy work.

The primary audience is a potential employer or hiring manager assessing Jodie for one of these roles. Recruitment contacts are a secondary route to that audience. Direct freelance enquiries remain welcome, but should not drive the site towards agency-style sales language.

**Desired visitor conclusion:** Jodie understands complex subjects, can turn them into marketing that connects with the intended audience, and combines professional judgement with creative execution.

**Desired visitor action:** Review relevant work, understand Jodie's contribution and experience, then contact her about a suitable opportunity.

Success means stronger applications, more relevant conversations and ultimately suitable part-time contracts. No numerical conversion targets or tracking setup have been agreed.

## 3. Positioning and personality

### Confirmed direction

- Professional B2B is the strongest positioning context, particularly engineering and life science engineering.
- Experience also includes education and creative work, including Jodie's own artist rebrand.
- The site should remain relevant to opportunities outside B2B.
- The central capability is translating technical concepts into marketing material that resonates with its audience.
- Creative strengths include visual identity, brand voice and finding appropriate ways to bring humour and personality into professional B2B marketing.
- Jodie does not want to lead with hands-on sales. Advising on sales strategy and supporting conferences remain relevant supporting capabilities.

### Working narrative

**Connecting the dots between data, strategy and creativity.**

The scientific background explains a way of thinking: understanding evidence, identifying opportunities, making deliberate choices and improving the work. The creative background shows how that thinking becomes distinctive communications and campaigns.

Do not let molecular imagery imply that Jodie is offering scientific research services. The site must clearly present a marketer and an individual person.

### Voice

- First person, clear, confident and personable.
- Professional enough for technical employers, with room for warmth and restrained humour.
- Specific about decisions and contributions; avoid unsupported claims and generic growth promises.
- Explain technical work in language a hiring manager can understand.
- Use British English.

## 4. Visitor journey and content hierarchy

The site should support both a quick first assessment and a deeper review:

1. Recognise Jodie, her marketing identity and the central connecting-dots idea.
2. Find selected work relevant to the opportunity being considered.
3. Understand the challenge, her individual contribution, the reasoning and available evidence.
4. Read the professional background and experience that support the work.
5. Make contact about a role or contract.

The hero establishes identity and tone. The content immediately below it must make relevance to employers concrete without adding a paragraph to the approved hero.

Recommended emphasis: selected work first, supported by background and experience. Services should explain useful capabilities rather than read as a large menu of unrelated offerings.

## 5. Information architecture

**Recommended implementation:** A small static, multi-page website with dedicated, shareable case-study pages. This allows a relevant project to be linked directly from an application.

| Destination | Purpose | Initial content |
| --- | --- | --- |
| Home | Establish identity and guide assessment | Approved hero, selected work, concise professional context, contact invitation |
| About | Explain the person and approach | Scientific and creative background, portrait, working style, link to experience |
| Work | Make relevant evidence easy to find | Project index with short summaries and links to case studies |
| Individual case studies | Demonstrate judgement and contribution | Challenge, audience, role, approach, work and evidenced outcomes |
| Services | Explain contract capabilities | A few coherent capability groups with links to relevant work |
| Experience | Provide a readable web CV | Career history, responsibilities, education and relevant skills |
| Contact | Start a relevant conversation | Contact form with clear submission states |

Keep the established main navigation: **Home, About, Work, Services, Contact**, with a separate outlined **Let's connect →** button. Recommended placement for Experience is a prominent link from About and an accessible footer link, preserving the existing navigation composition. Final placement remains open.

The earlier notes request a web CV rather than a downloadable PDF. Do not make a PDF download a launch requirement.

## 6. Homepage and visual design

### Primary reference

Use `context/mockupUI.png` as the primary visual reference. The earlier design brief records the hero composition, messaging, navigation and molecular treatment as approved. Build from this direction rather than redesigning it.

### Hero content

- Eyebrow: **FREELANCE MARKETER**.
- H1: **Jodie Hemsill**.
- Tagline: **Connecting the dots between data, strategy and creativity.**
- Primary button: **Explore my work →**.
- Secondary button: **About me**.
- No additional descriptive paragraph beneath the tagline.
- No JH monogram, initials or logo in the navigation.

Retain the established eyebrow for the initial build. Whether to change it to make contract availability more explicit is a later content decision; do not silently replace it.

### Colour and typography

| Role | Starting colour |
| --- | --- |
| Primary background | Black, `#000000` |
| Background depth and molecular shadows | Deep navy, `#07182E` |
| Molecular surfaces and secondary accents | Blue, `#254E83` |
| Buttons and highlights | Ice blue, `#B9D4FF` |
| Main text | Off-white, `#F5F7FA` |

These are starting values from the brief, not exact samples from the mockup. Refine them as needed for visual fidelity and legibility.

Use a modern sans-serif such as Inter or Manrope, with a suitable fallback. Keep the name oversized, with Jodie in off-white and Hemsill in soft ice blue or a subtle gradient. Use generous space, a clear hierarchy and restrained font weights. Avoid decorative fonts and excessive letter spacing in body text.

### Molecular visual

- Realistic ball-and-stick structure, with opaque, matte dark-blue spheres and thin bonds.
- Subtle texture, restrained blue lighting, soft shadows and controlled depth of field.
- Follow the diagonal from the upper right towards the lower left, with scale and fade informed by the mockup.
- Keep the text on the left readable and the right-hand structure visually dominant.
- Avoid glassy spheres, neon, strong reflections, bright white highlights and a disco-ball appearance.

Earlier notes suggest trying SVG first and comparing static and gently moving versions. **Recommendation:** Test an SVG treatment against the reference before committing. If it cannot capture the material and depth convincingly, use an optimised dedicated image asset. Do not use the complete mockup as a flattened webpage or embed its text inside the background.

Use a static version as the baseline. Optional movement should be subtle, inexpensive and removable for reduced-motion preferences. Do not require live 3D rendering for launch.

### Responsive behaviour

- Preserve the name, tagline and button hierarchy on narrow screens.
- Reposition or crop the molecular artwork to support the text rather than compete with it.
- Use a compact navigation with an accessible open/close control.
- Prevent text clipping, horizontal overflow and awkward button wrapping.
- Lower-page layouts must retain the same visual restraint as the hero.

## 7. Content requirements

### About and experience

The source brief states that Jodie holds a BSc in Biomedical Science. Include this background with its relevance to her approach; confirm the precise qualification wording before final publication.

Explain experience across technical B2B, education and creative industries. Show a real person through a professional portrait and specific, natural writing. The circular portrait inside a grey panel is an earlier idea, not a fixed layout requirement.

The experience page needs real job titles, organisations, dates, responsibilities and qualifications supplied or confirmed by Jodie. Current title, career chronology and the relative prominence of the degree remain open.

### Portfolio

Candidate inventory from the source material:

| Candidate project | Evidence to request | Status |
| --- | --- | --- |
| SEO strategy and website redesign | Analytics, Search Console, screenshots, decisions and results | Candidate; details pending |
| Marketing-material design | Brochures, graphics, photographs and relevant designs | Candidate; details pending |
| Engineering-company social media | Content, articles, social or website analytics | Candidate; details pending |
| Emerging-artist social media | Instagram content and analytics, including 2023–2024 if relevant | Candidate; details pending |
| Artist rebrand and EP campaign | Identity, website, music video and festival evidence | Candidate; details pending |
| Education/careers social media | Channel content, audience context and outcomes | Candidate; organisation name needs confirmation |
| AI workflow and data aggregation | Workflow explanation, diagrams and examples | Candidate; details pending |
| CRM implementation | Process changes, implementation scope and examples | Candidate; platform and details need confirmation |

The meeting notes mention seven projects; other notes list eight candidates. Treat this as an inventory, not a commitment to publish every project. Select and order the strongest examples after the next interview. A small number of convincing case studies is the recommended launch scope.

For each published case study, capture:

1. Organisation or anonymised context, sector and intended audience.
2. The challenge and what needed to change.
3. Jodie's role, scope and collaborators, distinguishing individual contribution from team work.
4. The reasoning, approach and important decisions.
5. Selected deliverables with explanatory captions.
6. Outcomes supported by available evidence; include timeframe and context for figures.
7. A short reflection where it adds useful insight.

Do not invent metrics, testimonials, client names, responsibilities or results. The handwritten suggestion about tripling client bases is an unverified idea and must not become a published claim without evidence. Qualitative outcomes are acceptable when clearly described. Confirm permission and remove sensitive material before using client assets or analytics.

### Services / capabilities

Recommended grouping, retaining the established Services label:

| Group | Supporting capabilities |
| --- | --- |
| Strategy and direction | Marketing strategy, SEO strategy, consultancy and coaching |
| Content and creative delivery | Social media management, brand voice, marketing materials, brochure and website design |
| Systems and implementation | CRM implementation and optimisation, AI workflows, data aggregation |

Conference support and advice on business development or sales strategy can appear as supporting experience. Do not present hands-on sales as a priority offer.

Keep social media, marketing management and strategy easy to identify, since these are the priority contract opportunities. Avoid pricing packages or a productised agency offering unless requested later.

### Contact

The earlier notes request a form whose submissions reach Gmail, preferably using a free solution.

Recommended initial fields: name, email and message. Any additional fields should have a clear purpose. Invite enquiries about roles and contracts using natural, employer-friendly wording.

Required behaviour:

- Clear labels and validation.
- Visible sending, success and failure states.
- Preserve entered information if submission fails.
- Appropriate spam protection without unnecessary friction.
- Only report success after the submission service confirms receipt.

The provider, destination address and privacy wording are unresolved. Verify provider suitability, current free-tier limits and data handling during implementation. Recommend a service then explain meaningful tradeoffs in plain language. A static website requires a submission service or equivalent endpoint to deliver the form; keep secrets out of public site files. An unconnected form may be demonstrated locally but is not launch-ready.

## 8. Technical and maintenance requirements

### Confirmed constraints

- Host on **GitHub Pages**.
- Build a **static** site.
- Target **100 Lighthouse scores**.
- Structure the project so an agent can maintain it through instructions from a non-technical owner.
- Explain decisions with significant technical implications in plain language and make a recommendation.
- Support adding projects and potentially a blog later.

### Recommended implementation default

Use plain HTML, CSS and minimal JavaScript. A small static generator is an option only if its benefit for shared layouts and project content outweighs the extra setup. Do not add a framework, database, CMS or server application without an actual requirement.

Maintain a shared visual system for colours, spacing, typography and components. Keep content and asset naming predictable. Document how to preview the site, change text, add a case study and publish an update. Avoid duplicating case-study data across multiple unrelated files where practical.

Support the selected GitHub Pages base path so navigation, images and direct links work both locally and when hosted. The repository URL, deployment setup and any custom domain are not yet known.

### Performance, accessibility and discovery

- Treat 100 in each applicable Lighthouse category as a target to measure, not a result already guaranteed.
- Run production checks on representative pages at mobile and desktop settings; record scores and material limitations.
- Keep the hero asset efficient, reserve image dimensions and avoid unnecessary scripts or third-party embeds.
- Use semantic page structure, logical headings, keyboard access, visible focus and readable contrast.
- Supply meaningful image alternatives; keep purely decorative molecular imagery out of the reading order.
- Respect reduced-motion preferences and ensure interactions work without hover.
- Use page-specific titles, descriptions and useful sharing metadata. Configure canonical URLs once the public address is known.
- Make content readable without relying on JavaScript for basic navigation or text.

Analytics, cookie tools and tracking integrations are not launch requirements. Decide on them only if there is a concrete measurement need.

## 9. Scope and delivery sequence

### Initial build scope

- Shared visual styles and responsive navigation.
- Homepage matching the established hero direction.
- About, Work, Services, Experience and Contact structure.
- Reusable case-study presentation with real content as it becomes available.
- Static hosting preparation, accessibility and performance verification.
- Short owner-facing maintenance instructions.

### Later options

- More projects and richer case-study evidence.
- Blog or articles.
- Additional restrained motion if it improves the experience.

Do not add a blog, CMS, booking system, login, chatbot or elaborate interactive visualisation to the initial scope by default.

### Recommended sequence

1. Build the homepage hero and shared styles against the supplied mockup.
2. Establish navigation, responsive layouts and case-study structure.
3. Add confirmed professional content and the strongest available projects.
4. Connect and test the contact form after its provider and destination are selected.
5. Verify content, accessibility, performance and hosted-path behaviour; prepare deployment and maintenance documentation.

Build structure can begin from this specification. A publication-ready portfolio depends on real content and working contact delivery. Clearly marked draft content may be used during local development; do not publish invented case studies or unfinished claims as real work.

## 10. Acceptance criteria

- A hiring manager can quickly identify Jodie as a marketer and find work relevant to contract opportunities.
- The site supports part-time contract applications while remaining open to other relevant work.
- The desktop hero follows the supplied composition, copy, colour direction and molecular treatment.
- Mobile layouts remain readable and usable without horizontal scrolling.
- Every navigation item, project link and contact action leads to a working destination.
- Published case studies distinguish Jodie's contribution and substantiate outcome claims.
- Professional background and experience contain confirmed details.
- The form is tested end to end, including failure handling and delivery to the intended inbox.
- Keyboard operation, focus, contrast, alternatives and reduced-motion behaviour are checked.
- Lighthouse results are recorded against the target of 100, with any remaining gaps explained.
- The site works as a static GitHub Pages deployment, including direct access to individual pages.
- Maintenance instructions allow an agent to update content consistently for a non-technical owner.

## 11. Open decisions for the next interview / build phase

These remain unanswered; do not present them as agreed requirements:

1. Which two or three projects lead the portfolio, and what evidence supports them?
2. What is the strongest example of translating a technical concept for an audience?
3. What may be named or shown publicly, and what requires anonymisation?
4. What are Jodie's current professional title, career history and exact qualification details?
5. Should the established freelance eyebrow change to communicate contract work more directly?
6. How much availability information should be public: days per week, remote/location preferences and start date?
7. Which portrait, project assets, testimonials and professional links are available?
8. Should Experience have a main-navigation position or remain linked through About and the footer?
9. Which Gmail address and form provider will receive enquiries?
10. Which GitHub repository, public URL and any custom domain will be used?
11. Does an SVG reproduce the approved hero convincingly, or is an optimised image needed?

Next interview priority: project evidence and career details. These will turn the site's central positioning from a promise into a convincing hiring case.
