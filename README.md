# Swnata E-Commerce Design Guidelines

## Design Approach
**Reference-Based Approach**: Drawing inspiration from premium natural beauty e-commerce leaders (Aesop, Ritual, Goop) combined with tropical nature aesthetics. The design emphasizes purity, tranquility, and organic authenticity through generous whitespace, elegant typography, and nature-inspired visual elements.

## Core Design Principles
1. **Pureza Natural** - Clean, uncluttered layouts that breathe
2. **Conexão Orgânica** - Nature-inspired patterns and imagery throughout
3. **Elegância Minimalista** - Refined simplicity without sacrificing richness
4. **Frescor Tropical** - Light, airy feeling with tropical forest undertones

---

## Color Palette

### Primary Colors
- **Forest Green**: 152 49% 33% - Primary brand color for headers, CTAs, key elements
- **Soft Sage**: 123 38% 71% - Secondary actions, hover states, accents
- **Natural Wood**: 16 25% 38% - Warm grounding element for text, borders

### Neutrals & Backgrounds
- **Pure White**: 0 0% 100% - Primary backgrounds, cards
- **Cream**: 73 50% 97% - Alternative background, section dividers
- **Light Sage**: 100 30% 95% - Subtle section backgrounds

### Functional Colors
- **Success Green**: 140 60% 45% - Confirmations, availability
- **Alert Amber**: 45 100% 51% - Warnings, low stock
- **Error Red**: 0 70% 50% - Errors, out of stock

---

## Typography

### Font Families
- **Primary**: 'Poppins' (Google Fonts) - Body text, UI elements
- **Accent**: 'Playfair Display' (Google Fonts) - Headers, brand moments
- **System Fallback**: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif

### Type Scale
- **Hero Heading**: text-6xl (60px) / text-5xl mobile, font-light, tracking-tight
- **Section Heading**: text-4xl (36px) / text-3xl mobile, font-light
- **Card Title**: text-2xl (24px), font-normal
- **Product Name**: text-xl (20px), font-medium
- **Body**: text-base (16px), leading-relaxed
- **Small**: text-sm (14px), for metadata, labels
- **Tiny**: text-xs (12px), for footer, legal text

---

## Layout System

### Spacing Primitives
**Core Units**: 2, 4, 8, 12, 16, 24, 32 (Tailwind units)
- Component padding: p-4, p-6, p-8
- Section spacing: py-16 (desktop), py-12 (tablet), py-8 (mobile)
- Card gaps: gap-6 or gap-8
- Element margins: mb-4, mb-8, mb-12

### Container Strategy
- **Max Width**: max-w-7xl for main content areas
- **Product Grid**: max-w-6xl centered
- **Text Content**: max-w-4xl for readability
- **Full Bleed**: w-full for hero, banner sections

### Grid Systems
- **Product Cards**: grid-cols-1 md:grid-cols-2 lg:grid-cols-4
- **Info Cards**: grid-cols-1 md:grid-cols-2 lg:grid-cols-4
- **Admin Dashboard**: grid-cols-1 lg:grid-cols-3 (sidebar + content)

---

## Component Library

### Navigation
- **Fixed Header**: backdrop-blur-md bg-white/90, shadow-sm, h-20
- **Logo**: Playfair Display, text-3xl, forest green color
- **Menu Items**: Poppins medium, hover:text-forest-green transition
- **Mobile Menu**: Full-screen overlay with slide-in animation, hamburger icon (3 horizontal lines)

### Hero Section
- **Layout**: Full-width image background with centered overlay content
- **Height**: min-h-[600px] md:min-h-[700px]
- **Image Treatment**: Overlay with gradient (from transparent to cream at bottom)
- **Text**: Large Playfair heading in white or cream, centered
- **CTA**: Outlined button with blurred background (backdrop-blur-md bg-white/20)

### Product Cards
- **Container**: Rounded-xl, overflow-hidden, bg-white, shadow-md hover:shadow-xl transition
- **Image**: aspect-[3/4], object-cover, smooth hover scale (scale-105)
- **Content Padding**: p-6
- **Button**: Full-width, rounded-lg, forest green background
- **Spacing**: gap-2 for internal elements

### Information Cards
- **Style**: Horizontal layout, bg-cream/white, rounded-2xl, p-8
- **Icon**: Large circular icon (w-16 h-16) in soft sage background
- **Text**: Centered, title in text-lg font-medium, description in text-sm

### Shopping Cart
- **Overlay**: Fixed right sidebar, backdrop-blur with semi-transparent background
- **Items**: List with product thumbnail, name, quantity controls (+/- buttons), remove icon
- **Footer**: Sticky total and checkout button at bottom

### Admin Dashboard
- **Sidebar**: Fixed left, bg-forest-green, white text, w-64
- **Main Area**: bg-light-sage, rounded cards for each section
- **Forms**: Clean inputs with rounded-lg borders, focus:ring-sage
- **Data Tables**: Alternating row colors, hover:bg-sage-light

### Footer
- **Layout**: Three-column grid on desktop, stacked on mobile
- **Background**: bg-forest-green, text-white/cream
- **Links**: Hover underline effect
- **Social Icons**: Circular, hover:bg-sage transition
- **Tagline**: Italic Playfair text, text-xl, centered below columns

---

## Animations & Interactions

### Subtle Animations Only
- **Hover Effects**: scale-105 on product images (duration-300)
- **Button Hover**: Slight brightness increase, no dramatic color changes
- **Scroll**: Smooth scroll behavior enabled
- **Page Transitions**: Simple fade-in for new content
- **Cart**: Slide-in from right (translate-x-full to translate-x-0)

**Avoid**: Parallax, complex scroll-triggered animations, spinning elements

---

## Images

### Hero Section
**Large Background Image**: Full-width, immersive tropical nature scene
- Suggested imagery: Lush green leaves with water droplets, soft sunlight filtering through forest canopy, or aerial view of tropical botanical garden
- Overlay: Subtle gradient to ensure text readability
- Placement: Top of homepage, 600-700px height

### Product Images
**High-Quality Photos**: Square aspect ratio (1:1 or 3:4) on white/cream background
- Suggested imagery: Close-up product shots, styled with natural elements (leaves, stones, water)
- Consistency: All products should have similar lighting and background treatment

### Informational Sections
**Decorative Nature Elements**: Subtle leaf patterns or botanical illustrations as section backgrounds
- Suggested imagery: Watercolor botanical illustrations, minimalist line drawings of leaves/plants
- Treatment: Low opacity (20-30%), positioned as decorative accents

### Category/Banner Images
**Lifestyle Photography**: Products in natural settings
- Suggested imagery: Products on wooden surfaces, surrounded by plants, in spa-like environments
- Mood: Serene, clean, aspirational

---

## Responsive Behavior

### Breakpoints
- **Mobile**: < 768px (single column, stacked navigation)
- **Tablet**: 768px - 1024px (2 columns for products/info cards)
- **Desktop**: > 1024px (4 columns for products, full layout)

### Mobile-Specific
- Hamburger menu replaces horizontal nav
- Product cards stack to single column
- Footer columns stack vertically
- Reduce heading sizes by 1-2 levels
- Increase touch target sizes (min 44x44px)

---

## Accessibility & Dark Mode

### Contrast
- Maintain WCAG AA standard (4.5:1 for normal text, 3:1 for large text)
- Forest green on white: ✓ Passes
- Wood brown on cream: ✓ Passes

### Focus States
- Visible focus rings on all interactive elements (ring-2 ring-sage)
- Skip to content link for keyboard navigation

### Dark Mode
**Not Implemented** - The brand identity centers on lightness, purity, and natural brightness. Maintain light theme throughout for consistency with brand values.
