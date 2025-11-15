# Travel Website Design Guidelines

## Design Approach
**Reference-Based Design** inspired by Airbnb's visual language with elements from Booking.com's information hierarchy. This approach emphasizes aspirational imagery, clean layouts, and seamless browsing experiences that inspire wanderlust while maintaining usability.

## Typography System

**Font Families:**
- Primary: Inter (via Google Fonts) - for headings and UI elements
- Secondary: Open Sans (via Google Fonts) - for body text and descriptions

**Type Scale:**
- Hero Headlines: text-5xl to text-7xl, font-bold
- Section Headers: text-3xl to text-4xl, font-semibold
- Card Titles: text-xl to text-2xl, font-semibold
- Body Text: text-base to text-lg, font-normal
- Captions/Meta: text-sm, font-medium

## Layout System

**Spacing Primitives:** Use Tailwind units of 4, 6, 8, 12, 16, 20, 24 (e.g., p-4, gap-8, mt-12, py-20)

**Container Strategy:**
- Full-width sections with inner max-w-7xl for content
- Cards and content blocks: max-w-6xl
- Text-heavy sections: max-w-4xl

**Grid Patterns:**
- Destination cards: grid-cols-1 md:grid-cols-2 lg:grid-cols-3
- Package listings: grid-cols-1 lg:grid-cols-2
- Feature highlights: grid-cols-1 md:grid-cols-3
- Testimonials: grid-cols-1 md:grid-cols-2 lg:grid-cols-3

## Component Library

**Navigation:**
- Sticky header with logo left, navigation center, CTA button right
- Mobile: Hamburger menu with full-screen overlay
- Include search icon and user account icons
- Subtle shadow on scroll for depth

**Hero Sections:**
- Home: Full-viewport (min-h-screen) with large background image, centered headline, search bar overlay
- Inner pages: Half-viewport (h-96 to h-[32rem]) with page title and breadcrumb
- Buttons on images: Use backdrop-blur-sm with semi-transparent backgrounds

**Destination Cards:**
- Image-first design with 4:3 aspect ratio
- Hover effect: subtle scale transform and shadow increase
- Location badge overlay on image (top-left)
- Title, brief description, "Explore" link below image
- Price indicator for packages

**Package Cards:**
- Horizontal layout on desktop (image left, content right)
- Vertical stack on mobile
- Include: Featured image, title, duration badge, highlights list, price, "View Details" CTA
- Use border and subtle shadow for card elevation

**Search/Filter Component:**
- Prominent search bar with destination input, date pickers, guest selector
- Filter sidebar for Destinations page: categories, price range, duration sliders
- Pill-style active filter tags

**Contact Form:**
- Two-column layout: form left (name, email, subject, message), contact info/map right
- Form fields with floating labels
- Include office hours, phone, email, social media links

**Footer:**
- Three-column layout: Company info, Quick Links, Newsletter signup
- Social media icons row
- Copyright and legal links bottom bar
- Include trust badges (secure booking, customer support indicators)

**About Page Components:**
- Mission statement section with large typography
- Team grid with photos and bios (circular avatars)
- Timeline/milestone visualization
- Stats counter section (destinations served, happy travelers, years of experience)

## Images

**Hero Images:**
- Home: Breathtaking travel destination (mountain landscape, beach sunset, or iconic cityscape) - full-width, high-quality
- Destinations: Aerial view of diverse landscapes
- Packages: Collage of adventure activities
- About: Team photo or authentic travel moment
- Contact: World map or travel montage

**Content Images:**
- Destination cards: High-quality photos of each location (landmarks, culture, nature)
- Package thumbnails: Activity-focused imagery (hiking, beaches, cultural sites)
- About page: Authentic team photos, office culture shots
- Testimonial avatars: Circular customer photos

**Image Treatment:**
- Consistent aspect ratios (4:3 for cards, 16:9 for headers)
- Subtle gradient overlays on hero images for text legibility
- Rounded corners: rounded-lg for cards, rounded-xl for featured content

## Interaction Patterns

**Page Transitions:**
- Smooth React Router transitions between pages
- Scroll restoration on navigation

**Micro-interactions:**
- Card hover: transform scale-105 with transition-transform duration-300
- Button hover: Native button states (no custom implementations)
- Image loading: Skeleton placeholders with pulse animation

**Forms:**
- Inline validation with clear error messages
- Success states with checkmark icons
- Disabled state during submission

## Accessibility Standards
- Semantic HTML throughout (nav, main, article, aside)
- ARIA labels for icons and interactive elements
- Focus states with visible outlines (ring-2 ring-offset-2)
- Alt text for all images with descriptive context
- Keyboard navigation support for all interactive elements
- Minimum touch target size of 44x44px for mobile