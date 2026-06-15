Build a flip-card testimonial component with the following exact specifications:

Card Dimensions & Container

Card size: 430 × 448px
Card background color: #1C1D21 (dark charcoal)
Border radius: 20px on all corners
No box shadow
Page/section background: #000000
When showing multiple cards side by side, use a 32px gap between them


Front Side

A full-bleed portrait photo covering the entire card (object-fit: cover, centered)
On top of the photo, apply a gradient overlay: linear-gradient(transparent 0%, rgba(0,0,0,0.4) 100%) — transparent at the top, darkening at the bottom
At the bottom-left of the card, inside 44px padding, display two lines of text stacked vertically (gap: 0px):

Name — font: Poppins, 16px, weight 600, color white (#ffffff), line-height 19.2px
Title/Role — font: Poppins, 16px, weight 400, color white (#ffffff), line-height 19.2px




Back Side (revealed on flip)

Same dark card background (#1C1D21), same 20px border radius
Content padding: 44px on all sides
Layout: flex column, justify-content: flex-end, align-items: flex-start, gap: 12px between all elements
Elements from top to bottom:

Company logo — displayed top-left, max size ~141 × 50px, object-fit: contain, left-aligned
Quote icon — a double open-quotation mark SVG (42 × 42 viewBox), filled with a diagonal linear gradient from #D9D9D9 (0%) to #FFFFFF (89%), giving a soft grey-to-white shimmer effect
Quote text — font: Poppins, 24px, weight 400, color #ffffff, line-height 28.8px (1.2×), width ~342px
Name — font: Poppins, 16px, weight 600, color #ffffff, line-height 19.2px
Title/Role — font: Poppins, 16px, weight 400, color #ffffff, line-height 19.2px


Avatar photo — positioned in the top-right corner of the card, size 142 × 148px, object-fit: cover, with an asymmetric border radius of 0px 20px 0px 80px (top-left: 0, top-right: 20px, bottom-right: 0, bottom-left: 80px) — this creates a curved cutout shape anchored to the top-right corner


Flip Interaction

On desktop: hovering the card triggers a 3D flip (rotateY 180°) to reveal the back side
On mobile/touch: tapping the card triggers the flip
Use CSS transform-style: preserve-3d and backface-visibility: hidden on both faces
Apply a smooth CSS transition on the flip (e.g. transition: transform 0.5s ease)
The card should flip around the vertical Y axis


Overall Design Language

Strictly dark-mode: black background, dark charcoal cards, all-white text
Font: Poppins (Google Fonts) throughout
No borders, no external box shadows on the card
Minimalist — no decorative elements other than the gradient quote icon and the asymmetric avatar cutout