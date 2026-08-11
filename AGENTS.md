# WUFFWERK — Codex / Agent Instructions

## 1. Project goal

WUFFWERK is a German premium-style online shop for dog accessories.

The project should remain:
- simple to maintain
- fast
- mobile-friendly
- visually premium
- suitable for GitHub Pages
- as cost-efficient as possible

The current business model is intended to use dropshipping rather than holding inventory.

## 2. Repository

Repository:
`OrdinaryOnonas/wuffwerk-shop`

Default branch:
`main`

The site is intended to run as a static GitHub Pages website.

Do not introduce a server, database, build system, framework, or paid service unless explicitly requested.

## 3. Technology rules

Prefer:
- HTML5
- CSS3
- vanilla JavaScript

Avoid adding React, Vue, Next.js, Node build tooling, Tailwind, Bootstrap, or other frameworks unless explicitly requested.

Keep the project usable by simply opening/deploying `index.html`.

If additional files are necessary, keep the structure simple and explain why they are needed.

## 4. Design language

WUFFWERK should have a premium, clean aesthetic inspired by modern Apple-style product presentation.

Design principles:
- generous whitespace
- strong typography hierarchy
- rounded cards
- subtle shadows
- restrained use of color
- large product imagery
- smooth but lightweight animations
- excellent mobile layout
- clear calls to action

Do not turn the site into a generic template or marketplace.

Brand name:
**WUFFWERK**

Tone:
- modern
- trustworthy
- friendly
- premium
- dog-focused

## 5. Product presentation

Products should have:
- clear German names
- concise benefit-focused descriptions
- realistic pricing
- high-quality product imagery
- useful product highlights
- clear CTA buttons
- mobile-friendly layouts

Never invent:
- supplier prices
- delivery times
- reviews
- certifications
- product specifications
- guarantees
- stock levels

If information is unknown, leave it configurable or clearly mark it as needing confirmation.

Supplier/product data must be treated as external data and verified before being presented as fact.

## 6. Images

Use realistic product photography where possible.

Do not use obviously fake placeholder images in the finished storefront.

If AI-generated imagery is used:
- it should look realistic
- it must fit the WUFFWERK visual identity
- it should not falsely imply a specific supplier's exact product unless the image actually represents that product
- do not create fake customer reviews or fake user testimonials using AI imagery

## 7. Shopping cart

The cart should:
- allow adding products
- allow changing quantities
- allow removing products
- show subtotal/total
- work on mobile
- persist locally where appropriate

Use `localStorage` for a simple static-site cart unless a real backend is explicitly introduced.

Do not collect or store sensitive payment information in localStorage.

## 8. Checkout

The current checkout is a frontend/demo checkout.

Until a real payment/backend system is explicitly implemented:
- do not claim that payment was processed
- do not claim that an order was actually submitted
- do not transmit customer data to third parties
- do not store payment credentials

When implementing a real checkout, use a proper payment provider and server-side order handling.

Never implement raw credit-card handling in frontend JavaScript.

## 9. Legal pages

The project may contain:
- Impressum
- Datenschutz
- Widerrufsbelehrung
- AGB

These are placeholders until the owner's actual business details and legal requirements are supplied.

Never invent company details, addresses, VAT IDs, registration numbers, or legal claims.

Before the store goes live, clearly indicate that the legal texts need to be finalized.

## 10. Dropshipping rules

The intended model is dropshipping.

Preferred suppliers:
- Germany
- EU

Prioritize:
- short delivery times to Germany
- reliable suppliers
- transparent product data
- reasonable shipping costs
- good supplier ratings
- low return risk
- products with sufficient margin

Do not publish a product merely because the wholesale price looks cheap.

Always evaluate:

`selling price - product cost - shipping - payment fees - expected returns - taxes = realistic contribution`

Never present an estimated margin as guaranteed profit.

## 11. Current product direction

The current product strategy focuses on a small selection of dog accessories.

Ideas previously considered:
- snuffle mats
- travel water bottles
- interactive dog toys
- LED collars/leashes
- car protection covers

The current preference is to find German/EU suppliers before using expensive overseas suppliers.

ZooDrop / Pet-Star was identified as a German supplier candidate. Its actual merchant prices must be verified through the merchant account before using them in calculations.

## 12. Zero-budget constraint

The project is being developed with a target of approximately 0 € upfront investment.

Therefore:
- prefer free hosting such as GitHub Pages
- avoid unnecessary SaaS subscriptions
- avoid paid plugins unless explicitly approved
- do not recommend buying a domain until the user decides to do so
- prefer free/open-source tooling

Do not sacrifice security or legal compliance merely to save money.

## 13. Code quality

Keep code:
- readable
- well structured
- reasonably commented
- accessible
- responsive
- lightweight

Avoid unnecessary duplication.

Do not break existing functionality when changing the design.

Before replacing a working component, understand its existing behavior.

## 14. Accessibility

Use:
- semantic HTML
- labels for form fields
- keyboard-accessible controls
- useful alt text
- sufficient contrast
- visible focus states

Do not rely on color alone to communicate important information.

## 15. Security and privacy

Never:
- hard-code API keys
- commit passwords or secrets
- expose private credentials
- collect payment credentials in frontend code
- send customer data to unknown services

If an API or secret is required, stop and explain the required secure architecture instead of putting the secret into `index.html`.

## 16. Change policy

When modifying the project:
1. Inspect the existing code first.
2. Preserve working functionality.
3. Make the smallest sensible change.
4. Test the affected behavior.
5. Check desktop and mobile layouts.
6. Explain what changed.

Do not rewrite the entire site unnecessarily.

## 17. Git workflow

Use clear commit messages.

Examples:
- `feat: add snuffle mat product`
- `fix: repair mobile cart`
- `style: improve product cards`
- `docs: update agent instructions`

Do not force-push or overwrite history unless explicitly requested.

Prefer small, understandable commits.

## 18. Future development priorities

Recommended order:

1. Verify German/EU suppliers
2. Select 3–5 profitable products
3. Add real product information and images
4. Improve product detail pages
5. Implement a real order backend
6. Add a legitimate payment provider
7. Add order confirmation emails
8. Finalize legal pages
9. Test checkout thoroughly
10. Connect a domain
11. Launch marketing/social content

## 19. Important rule for Codex

When asked to modify WUFFWERK, treat this file as the project-specific source of truth.

Do not:
- change the brand name
- remove existing core shop functionality
- introduce unnecessary frameworks
- invent business information
- invent supplier information
- claim that demo checkout functionality is a real payment system
- add paid services without approval

When requirements conflict, prioritize the user's newest explicit request while preserving security, privacy, legal compliance, and existing functionality.

## 20. GitHub operations

Codex handles GitHub operations for the project on the owner's behalf, including inspecting repository state, creating branches, committing, pushing, opening and updating pull requests, and managing issues when requested.

Before irreversible or high-impact actions — deleting remote branches or files, force-pushing, merging pull requests, changing repository settings, or publishing releases — Codex must state the exact target and obtain the owner's explicit confirmation.

Codex must keep the owner informed about each completed GitHub action, including the affected branch, commit, pull request, issue, or file.
