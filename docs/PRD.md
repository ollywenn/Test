# Product Requirements Document (PRD)
## Zolv Travel Technology Website

**Version:** 1.0  
**Date:** January 31, 2026  
**Status:** Approved for Implementation

---

## 1. Purpose & Goals

### 1.1 What the Site Is For

The Zolv website is a marketing and client engagement platform designed to position Zolv as a specialized travel technology partner. The site serves to:

- Communicate Zolv's expertise in travel platform development and integration
- Demonstrate the value proposition of their Web Travel Platform (WTP)
- Showcase client success stories and project outcomes
- Facilitate client engagement through multiple partnership models
- Provide industry insights and thought leadership

### 1.2 Primary Business Objectives

1. **Lead Generation**: Convert visitors into qualified partnership inquiries through clear CTAs and an interactive contact wizard
2. **Brand Positioning**: Establish Zolv as a pragmatic, experienced travel technology partner (not a generic digital agency)
3. **Client Education**: Help prospects understand partnership models and integration capabilities
4. **Talent Acquisition**: Attract qualified technical candidates through career pages
5. **Thought Leadership**: Build credibility through insights and case study content

### 1.3 Success Criteria

- Clear differentiation from generic digital agencies
- Intuitive navigation through partnership options
- Effective showcasing of technical capabilities
- Reduced friction in the inquiry process
- Professional, modern presentation aligned with the travel technology sector

---

## 2. Target Audiences

### 2.1 Primary User Types

#### Travel Business Decision Makers
- **Profile**: CTOs, Product Managers, Digital Directors at travel companies
- **Needs**: 
  - Understand Zolv's integration capabilities
  - Evaluate partnership models
  - Assess technical expertise and credibility
  - View relevant case studies and outcomes
- **Goals**: Find a reliable technical partner to extend/improve existing systems

#### Travel Operations Teams
- **Profile**: Technical leads, product owners evaluating implementation partners
- **Needs**:
  - Deep-dive into platform capabilities
  - Understand integration approach and supported systems
  - Review technical depth through insights
- **Goals**: Validate technical fit and approach

#### Prospective Employees
- **Profile**: Software engineers, tech leads seeking travel technology roles
- **Needs**:
  - Understand company culture and values
  - Review available positions
  - Learn about the types of projects and technologies used
- **Goals**: Determine if Zolv is the right career fit

#### Existing Clients
- **Profile**: Current Zolv clients accessing portals or resources
- **Needs**:
  - Quick access to client login
  - Platform updates and insights
- **Goals**: Access client-specific resources efficiently

---

## 3. Information Architecture

### 3.1 Sitemap

```
Home
├── Our Approach (Services)
│   ├── Integration and Development
│   ├── Design, Build and Support
│   └── Strategic Consultancy
├── Platform
│   ├── WTP Platform Overview
│   ├── Platform Features (8 features)
│   └── Integration Capabilities
├── Integrations
│   ├── Integration Categories
│   │   ├── Booking Engines
│   │   ├── CRM Systems
│   │   ├── Payment Gateways
│   │   ├── Hotel & Flight APIs
│   │   ├── Customer Management
│   │   └── Third-party Tools
│   └── FAQ Section
├── Case Studies
│   ├── Case Studies List
│   └── Case Study Detail (template)
│       ├── Client Overview
│       ├── The Opportunity
│       ├── The Outcome
│       └── Results/Metrics
├── Insights
│   ├── Insights List (with filters)
│   │   ├── All
│   │   ├── Journal
│   │   ├── Industry News
│   │   └── Resources
│   └── Insight Detail (template)
│       ├── Article Meta
│       ├── Article Content
│       └── Related Insights
├── About
│   ├── Company Overview
│   ├── Mission Statement
│   ├── Company Story (Timeline)
│   ├── What Makes Us Different
│   ├── Meet the Founder
│   └── Careers
│       └── Career Detail (template)
│           ├── Role Overview
│           ├── Responsibilities
│           ├── Benefits
│           ├── Candidate Profile
│           └── Application Form
├── Contact
│   ├── Partnership Selection Wizard (3 steps)
│   ├── Location Information
│   └── Contact Form
└── Client Login (External Link)
```

### 3.2 Page Relationships

- **Navigation**: Persistent top navigation across all pages
- **CTAs**: Strategic placement of partnership CTAs throughout content pages
- **Cross-linking**: Case studies link to insights; insights link to case studies; all pages can link to contact
- **Footer**: Consistent footer navigation on all pages

---

## 4. Page-Level Requirements

### 4.1 Home Page

**Purpose**: Primary entry point that communicates value proposition and guides users to key sections

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "WE ARE YOUR DEVELOPMENT PARTNER"
   - Subheading: "Unlocking better customer experiences from the travel systems you already use"
   - Value proposition paragraph
   - Client logo strip (Virgin Holidays, HF Holidays, CV Villas, Monarch, Kuoni, Ramble Worldwide)

2. **Partnership Models Section**
   - Section heading: "How we partner"
   - Introduction paragraph
   - 5 partnership model cards:
     - Integration and development
     - Design, build and support
     - Development partner
     - Strategic partner
     - Strategic consultancy

3. **Design, Build and Support Section**
   - Process flow visualization: Research → Strategy → Design → Build → Integration → Production support
   - Description paragraph
   - CTA: "More about our approach"

4. **WTP Platform Section**
   - Heading: "Web Travel Platform"
   - Description of WTP capabilities
   - Highlight: "90% of what we deliver is bespoke"
   - CTA: "More about the WTP platform"

5. **What We Build Section**
   - 6 solution types:
     - B2C transactional websites
     - B2B agent portals
     - Booking management systems
     - Post-booking portals
     - Travel agent dashboards
     - Booking and integration APIs
   - CTA: "Explore integrations"

6. **Brand Statement**
   - "Tailored, tech-driven solutions for **travel companies**"

7. **Latest Case Studies Section**
   - Heading and description
   - Featured case study cards (3-4)
   - CTA: "View all case studies"

8. **Insights Section**
   - Heading: "Industry insight from people who build this stuff for a living"
   - Description
   - CTA: "Explore our insights"

**Required Interactions**:
- Smooth scrolling navigation (Blazor)
- Hover effects on cards and CTAs (CSS + Blazor)
- Client logo carousel (Blazor component)

**Dependencies**:
- Shared: Header, Footer, CTA Button components
- Card components for partnership models, case studies

---

### 4.2 Our Approach (Services) Page

**Purpose**: Detail the partnership models and service offerings

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Our approach"
   - Subheading: "We partner with travel companies at every stage of their journey"
   - Introduction text

2. **Partnership Models Detail**
   - Section heading with context
   - 3 detailed partnership model sections:
     
     **a. Integration and development**
     - Description
     - Services include list
     - CTA: "Partner with us"
     
     **b. Design, build and support**
     - Description highlighting it as most common engagement
     - Services include list (5 items)
     - CTA: "Partner with us"
     
     **c. Strategic consultancy**
     - Description
     - Services include list
     - CTA: "Partner with us"

3. **Effectiveness Section**
   - Heading: "Effectiveness of our approach"
   - Subheading
   - 3 value points:
     - Integration without friction
     - Unlocking real potential
     - A trusted delivery partner (50+ travel clients)

4. **Client Testimonial**
   - Quote from CEO, Virgin Holidays
   - Formatted quote block

5. **Platform CTA Section**
   - Description of WTP
   - CTA: "Find out more about the platform"

**Required Interactions**:
- Expandable/collapsible sections (Blazor)
- CTA button tracking and navigation (Blazor)

**Dependencies**:
- Shared: Header, Footer, Quote component, CTA Button

---

### 4.3 Platform Page

**Purpose**: Showcase the Web Travel Platform capabilities and features

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Web Travel Platform"
   - Subheading: "Our Web platform seamlessly connects with your existing travel systems"
   - Purple theme with video background

2. **Platform Overview**
   - Section label: "WTP PLATFORM"
   - Heading: "Our platform reveals the possibilities for your online travel services"
   - Description paragraph
   - Interactive platform diagram showing WTP connections:
     - Your travel platform
     - Book flow
     - CRM
     - API
     - Systems
     - Support

3. **Platform Features**
   - Section heading: "Web Travel Platform features"
   - Subheading
   - Central feature hub visual (Design, Infrastructure, AI)
   - Feature grid (2 rows × 4 columns = 8 features):
     1. Customisable Design
     2. Seamless Integration
     3. AI-Driven Capabilities
     4. Multi-Channel Support
     5. Staging Environments
     6. Language Translations
     7. Managed Infrastructure
     8. Multi Concurrent Users

4. **Testimonial Section**
   - Quote from Product Manager at HF Holidays
   - CTA button

5. **Client Philosophy**
   - Statement: "We believe in delivering tailored solutions that align with each client's specific needs and objectives"

6. **Integrations CTA**
   - Heading: "Integrations"
   - Description
   - CTA: "Find out more"

**Required Interactions**:
- Interactive platform diagram with hover states (Blazor)
- Feature card animations on scroll (Blazor)
- Video background control (HTML5 video)

**Dependencies**:
- Shared: Header, Footer, Feature Card, Testimonial Card
- Platform Diagram component (custom Blazor component)

---

### 4.4 Integrations Page

**Purpose**: Explain integration capabilities and supported systems

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Integrations"
   - Subheading: "Connecting the systems your business already depends on"
   - Introduction paragraphs

2. **Why Integrations Matter**
   - Section heading
   - Description paragraphs
   - "What good integrations unlock" list (6 benefits)

3. **Our Integrations**
   - Section heading
   - Description
   - Integration categories (6 types):
     - Booking engines
     - CRM systems
     - Payment gateways
     - Hotel & flight APIs
     - Customer management systems
     - Third-party tools

4. **FAQ Section**
   - 5 Q&A pairs:
     - What do integrations mean in a travel technology context?
     - Why are integrations so important for travel businesses?
     - What systems can Zolv integrate with?
     - How do integrations improve customer experience?
     - Do you use AI in integrations?

5. **Case Studies CTA**
   - Section heading: "Integration in practice"
   - Description
   - CTA: "View case studies"

**Required Interactions**:
- Expandable FAQ accordion (Blazor)
- Integration category cards with icons (Blazor)

**Dependencies**:
- Shared: Header, Footer, FAQ Accordion component, Category Card

---

### 4.5 Case Studies List Page

**Purpose**: Showcase client work and outcomes

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Case studies"
   - Subheading: "Delivery that stands up in real environments"
   - Introduction text

2. **Philosophy Statement**
   - Heading: "We empower our clients to stay ahead — by fixing what actually holds them back"
   - Description paragraph

3. **Client Partners**
   - Section heading: "A few of our travel partners"
   - Client logos grid: Virgin Holidays, HF Holidays, CV Villas, Monarch, Kuoni, Ramble Worldwide

4. **Client Testimonials**
   - Section heading: "What our clients say"
   - Subheading: "Proof from people who have to live with the outcome"
   - 3 featured testimonials:
     - CEO, Virgin Holidays
     - Product Manager, HF Holidays
     - Product Manager, Monarch
   - Each links to corresponding case study detail

5. **Insights CTA**
   - Description
   - CTA: "Explore our insights"

**Required Interactions**:
- Case study card hover effects (CSS + Blazor)
- Filter/sort functionality (Blazor - future enhancement)
- Testimonial cards linking to case study details (Blazor routing)

**Dependencies**:
- Shared: Header, Footer, Case Study Card, Testimonial Card

---

### 4.6 Case Study Detail Page (Template)

**Purpose**: Provide detailed view of specific client engagement

**Core Content Blocks**:
1. **Hero Section**
   - Client hero image
   - Client logo overlay

2. **Client Perspective**
   - Quote from client
   - Project overview paragraph

3. **The Opportunity**
   - Section heading
   - Challenge description
   - Key challenges list (3-4 bullets)
   - Goal statement

4. **The Outcome**
   - Section heading
   - Solution description
   - Results list (4 benefits)

5. **Results/Metrics**
   - Section heading: "The result"
   - 3 key metrics:
     - 80% increase in bookings
     - 90% uplift in sales
     - 12 new integrations delivered
   - Note: Metrics adapted per client

6. **More Case Studies CTA**
   - Description
   - CTA: "View all case studies"

7. **About Zolv CTA**
   - Section heading
   - Description
   - CTA: "Learn more"

**Required Interactions**:
- None specific (content-focused page)

**Dependencies**:
- Shared: Header, Footer, Quote component, Metric Card
- Dynamic content loading (Blazor parameter routing)

---

### 4.7 Insights List Page

**Purpose**: Present thought leadership and industry insights

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Insights"
   - Subheading: "Thinking from inside real travel platforms"
   - Introduction text (2 paragraphs)

2. **Filter Section**
   - Filter tabs:
     - All (default)
     - Journal
     - Industry news
     - Resources

3. **Article Grid**
   - Article cards with:
     - Featured image
     - Category tags
     - Article title
     - Excerpt
     - Read time/date
   - Grid layout (responsive)

4. **About Zolv CTA**
   - Section heading
   - Description
   - CTA: "Learn more"

**Required Interactions**:
- Filter tabs with active state (Blazor)
- Article list filtering based on selected category (Blazor)
- Pagination or infinite scroll (Blazor)

**Dependencies**:
- Shared: Header, Footer, Article Card, Filter Tabs component

---

### 4.8 Insight Detail Page (Template)

**Purpose**: Display full article content

**Core Content Blocks**:
1. **Article Meta**
   - Publication date
   - Category tags (Industry news · Resources)

2. **Article Title**
   - Main heading (specific, not poetic)

3. **Intro Section**
   - Introduction paragraph
   - Hero image

4. **Section 1**
   - Section heading: "Context before conclusion"
   - Image + text layout
   - Download link (if applicable)

5. **Section 2**
   - Section heading: "What we've learned in practice"
   - Text + image layout
   - Bullet points (3 learnings)

6. **Brand Statement**
   - "Tailored, tech-driven solutions for **travel companies**"

7. **More Insights**
   - Section heading: "Related thinking"
   - Description
   - Related article cards (3-4)

**Required Interactions**:
- None specific (content-focused)
- Download button functionality (Blazor)

**Dependencies**:
- Shared: Header, Footer, Article Card
- Dynamic content loading (Blazor parameter routing)

---

### 4.9 About Page

**Purpose**: Communicate company background, mission, and team

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "About"
   - Subheading: "A travel technology partner, not a generic digital agency"
   - Introduction paragraphs

2. **Mission Section**
   - Section heading: "Our mission"
   - Subheading: "Bridging technology and travel — properly"
   - Description paragraphs

3. **Company Story**
   - Section heading: "Our story"
   - Subheading: "Built in travel, shaped by delivery"
   - Timeline:
     - 2002: Foundation
     - 2003: Expansion
     - 2004: Growth
     - Present day focus

4. **Differentiators**
   - Section heading: "What makes us different"
   - Subheading: "Deep travel experience, end-to-end responsibility"
   - Description paragraphs

5. **Founder Profile**
   - Section heading: "Meet the founder"
   - Subheading: "Olly Wenn – Founder & Managing Director"
   - Biography
   - Photo

6. **Careers Section**
   - Section heading: "Careers"
   - Subheading: "Work on platforms that matter"
   - Description
   - Current opportunities list (3 roles):
     - Principal Software Engineer / Tech Lead
     - Web Developer
     - Graduate Developer

7. **Brand Statement**
   - "Tailored, tech-driven solutions for **travel companies**"

8. **Contact CTA**
   - Section heading: "Get in touch"
   - Subheading: "A partner you can rely on, not just a supplier"
   - Description
   - CTA: "Partner with us"

**Required Interactions**:
- Timeline visualization (Blazor component)
- Career opportunities as clickable cards (Blazor routing)

**Dependencies**:
- Shared: Header, Footer, Timeline component, Job Card

---

### 4.10 Career Detail Page (Template)

**Purpose**: Provide detailed job description and application path

**Core Content Blocks**:
1. **Job Header**
   - Job title: "Principal Software Engineer / Tech Lead"
   - Job details: Location, Type, Salary

2. **Overview Section**
   - Description of role and expectations

3. **Responsibilities**
   - Section heading
   - Responsibilities list (7 items)
   - Additional context paragraph

4. **Benefits**
   - Section heading
   - Introduction paragraph
   - Benefits list (6 items)
   - Tone note about company culture

5. **Candidate Profile**
   - Section heading
   - Introduction line
   - Profile requirements list (6 items)
   - Additional context

6. **Apply Now**
   - Section heading
   - Instructions
   - Application form or CTA

**Required Interactions**:
- Application form (Blazor)
- File upload for CV (Blazor InputFile)

**Dependencies**:
- Shared: Header, Footer, Form components

---

### 4.11 Contact Page

**Purpose**: Facilitate partnership inquiries through guided wizard and provide contact information

**Core Content Blocks**:
1. **Hero Section**
   - Main heading: "Contact"
   - Subheading: "We are your dedicated travel tech partner"
   - Purple background with decorative elements

2. **Partnership Statement**
   - Main heading: "We are more than just a service provider, we are your new dedicated travel tech partner"
   - White background with decorative shapes

3. **Partnership Selection Wizard**
   - Progress indicator (3 steps)
   - **Step 1: Partnership Type Selection**
     - Question: "How do you want to partner with us?"
     - 6 options (radio button style):
       1. Integration and development
       2. Design build and support
       3. Development partner (shown as selected in design)
       4. Strategic development partner
       5. Integration and development
       6. Strategic consultancy
     - "Next" button
   - **Step 2**: (To be defined - likely contact details)
   - **Step 3**: (To be defined - likely additional information/message)

4. **Location Information**
   - Section heading: "Where to find us"
   - Address: Avenue HQ, 10-12 East Parade, Leeds, LS1 2BH
   - Email: enquiries@zolv.com (clickable link)
   - Phone: +44 (0)113 3800 950
   - Interactive map with office location

5. **Brand Statement**
   - "Tailored, tech-driven solutions for **travel companies**"

6. **Insights CTA**
   - Title: "Insights"
   - Subtitle: "90% of what we create is bespoke to you"
   - CTA: "Find out more"

**Required Interactions**:
- **Multi-step wizard with progress tracking (Blazor)**
- **Partnership option selection with visual feedback (Blazor)**
- **Form validation and submission (Blazor)**
- **Next/Previous navigation through wizard steps (Blazor)**
- Email link (mailto:)
- Phone link (tel:)
- Interactive map (embedded iframe or Blazor map component)

**Dependencies**:
- Shared: Header, Footer
- **Wizard component (custom Blazor component - key feature)**
- **Form components with validation**
- Map integration component

---

## 5. Interactivity & Behaviour

### 5.1 Interactive Elements Overview

All interactive elements should be implemented using **Blazor** to maintain consistency and leverage server-side rendering capabilities. JavaScript should be avoided unless absolutely necessary for third-party integrations.

### 5.2 Blazor Interactive Components

#### 5.2.1 Navigation
- **Implementation**: Blazor NavLink components
- **Behavior**: 
  - Active state highlighting
  - Smooth scroll to sections on single-page layouts
  - Responsive mobile menu toggle
- **State Management**: Active route tracking via Blazor routing

#### 5.2.2 Contact Wizard (Primary Interactive Feature)
- **Implementation**: Custom Blazor component with state management
- **Behavior**:
  - Multi-step form with 3 distinct steps
  - Progress indicator updates automatically
  - Previous/Next navigation
  - Form state preservation between steps
  - Validation at each step before proceeding
  - Final submission with server-side processing
- **Data Flow**:
  - Step 1: Partnership type selection
  - Step 2: Contact information collection
  - Step 3: Additional details/message
  - Submit: Send to server/email endpoint
- **State Management**: Blazor component state with form model
- **Validation**: Blazor validation attributes and error messaging

#### 5.2.3 Filter Tabs (Insights Page)
- **Implementation**: Blazor component with event callbacks
- **Behavior**:
  - Tab selection updates active state
  - Filter articles based on selected category
  - Maintain state during navigation
- **State Management**: Component parameter and event callback pattern

#### 5.2.4 FAQ Accordion (Integrations Page)
- **Implementation**: Blazor accordion component
- **Behavior**:
  - Click to expand/collapse individual questions
  - Single or multiple items can be open (configurable)
  - Smooth animation transitions
- **State Management**: Array of boolean states for each FAQ item

#### 5.2.5 Platform Diagram
- **Implementation**: Custom Blazor component with SVG or HTML/CSS
- **Behavior**:
  - Interactive hover states showing connections
  - Click to highlight specific integration paths
  - Tooltips on hover explaining each connection
- **State Management**: Hover and click state tracking

#### 5.2.6 Feature Cards
- **Implementation**: Blazor component with hover effects
- **Behavior**:
  - Scale/elevation effect on hover
  - Smooth transitions
  - Click to expand for more details (optional)
- **State Management**: CSS-based with optional Blazor state for expansion

#### 5.2.7 Client Logo Carousel (Home Page)
- **Implementation**: Blazor carousel component
- **Behavior**:
  - Auto-rotate through client logos
  - Manual navigation controls
  - Pause on hover
  - Responsive layout
- **State Management**: Timer-based with Blazor component lifecycle

#### 5.2.8 Application Form (Career Pages)
- **Implementation**: Blazor EditForm with validation
- **Behavior**:
  - Input validation on blur and submit
  - File upload for CV (Blazor InputFile)
  - Success/error messaging
  - Form submission to server endpoint
- **State Management**: Blazor form model with validation
- **File Handling**: Server-side processing of uploaded files

#### 5.2.9 Timeline Component (About Page)
- **Implementation**: Blazor component with CSS styling
- **Behavior**:
  - Scroll-based animations revealing timeline items
  - Interactive year markers
- **State Management**: Visibility state based on scroll position (using Blazor JS interop if needed)

### 5.3 Non-Blazor Interactions (Minimal)

#### 5.3.1 Video Background
- **Implementation**: HTML5 video element
- **Behavior**: Auto-play, loop, muted
- **Justification**: Standard HTML capability, no JavaScript needed

#### 5.3.2 Map Integration
- **Implementation**: Embedded iframe (Google Maps) or Blazor map library
- **Behavior**: Display office location, basic zoom/pan
- **Justification**: Third-party service, standard iframe embed acceptable

#### 5.3.3 External Links
- **Implementation**: Standard anchor tags
- **Behavior**: Open client login in new tab, email/phone links
- **Justification**: Browser native behavior

### 5.4 Animation & Transitions

All animations should be implemented using:
1. **CSS Transitions**: For simple hover effects, opacity changes
2. **Blazor State Changes**: For component visibility and content updates
3. **CSS Animations**: For scroll-based reveals and loading states

**Avoid**: JavaScript animation libraries (GSAP, Anime.js, etc.)

### 5.5 Form Handling

All forms must use **Blazor EditForm** components with:
- Server-side validation
- Blazor validation attributes
- Error message display
- Success confirmation
- Email submission via server-side code

### 5.6 Responsive Behavior

Responsive design should be implemented through:
- CSS Grid and Flexbox
- Blazor conditional rendering for mobile vs desktop layouts
- Media queries for breakpoints
- No JavaScript-based resize detection

### 5.7 State Management Strategy

- **Page-level state**: Blazor component parameters and cascading values
- **Application state**: Blazor state container service (if needed for user preferences)
- **Form state**: Blazor EditForm model binding
- **Navigation state**: Blazor NavigationManager

### 5.8 Performance Considerations

- **Lazy loading**: Images and components loaded on demand
- **Debouncing**: Search and filter inputs (Blazor-based)
- **Caching**: Static content and API responses
- **Prerendering**: Enable Blazor Server prerendering for SEO

---

## 6. Design System

### 6.1 Color Palette

**Primary Colors**:
- Primary Purple: `#35226E`
- Yellow Accent: `#FDD712`
- White: `#FFFFFF`
- Black: `#000000`

**Secondary Colors**:
- Dark Gray Text: `#595959`
- Light Purple Text: `#C8C3D7`
- Light Gray Background: `#EAEBF3`

**Accent Colors** (for features/decorative elements):
- Pink: `#FFADC9`
- Light Blue: `#B7E9FF`
- Orange: `#FFAD76`
- Cyan: `#99E4E5`
- Green: `#1BAA91`

### 6.2 Typography

**Primary Font**: Plus Jakarta Sans  
**Secondary Font**: SF Pro Display

**Hierarchy**:
- Hero Heading: 64px, SemiBold, White on purple backgrounds
- Section Headings: 48px, SemiBold, Black
- Section Labels: 16px, ExtraBold, Primary Purple
- Card Headings: 24px, SemiBold, Black
- Body Text: 20px, Medium, Dark Gray (#595959)
- Navigation: 16px, Bold, White (on purple background)
- Button Text: 16px, Bold

### 6.3 Spacing & Layout

- **Container Max Width**: 1400px
- **Content Padding**: 110px horizontal for desktop
- **Section Spacing**: 80-120px vertical between major sections
- **Card Spacing**: 24-32px gaps in grids

### 6.4 Components

**Buttons**:
- Primary: Yellow background (#FDD712), black text, rounded corners
- Secondary: Black background, white text, rounded corners
- CTA: Consistent sizing and hover states

**Cards**:
- White background
- Rounded corners (8-12px border radius)
- Subtle shadow on hover
- Clean typography hierarchy

**Forms**:
- White input fields
- Purple focus states
- Clear error messaging in red
- Success states in green

### 6.5 Visual Elements

- Geometric backgrounds and decorative shapes
- Hand-drawn annotations and playful labels (where appropriate)
- Travel photography frames
- Abstract patterns in feature sections
- Consistent use of brand colors

---

## 7. Technical Requirements

### 7.1 Framework & Stack

- **Framework**: Blazor Server (ASP.NET Core)
- **Language**: C# for server-side, Razor syntax for components
- **Styling**: CSS (consider Tailwind CSS or custom CSS)
- **Hosting**: IIS or Azure App Service (based on existing .gitignore patterns)

### 7.2 Project Structure

```
/src
  /ZolvWeb
    /Pages
      Index.razor (Home)
      OurApproach.razor
      Platform.razor
      Integrations.razor
      CaseStudies.razor
      CaseStudyDetail.razor
      Insights.razor
      InsightDetail.razor
      About.razor
      CareerDetail.razor
      Contact.razor
    /Shared
      MainLayout.razor
      NavMenu.razor
      Footer.razor
    /Components
      ContactWizard.razor
      FeatureCard.razor
      TestimonialCard.razor
      CaseStudyCard.razor
      ArticleCard.razor
      FAQAccordion.razor
      PlatformDiagram.razor
      Timeline.razor
      JobCard.razor
    /Models
      ContactWizardModel.cs
      CaseStudy.cs
      Article.cs
      Job.cs
    /Services
      EmailService.cs
      ContentService.cs
    /wwwroot
      /css
      /images
      /fonts
    Program.cs
    _Imports.razor
```

### 7.3 Data Management

- **Static Content**: Content can be stored in JSON files or a simple CMS
- **Case Studies**: Data models with properties for client, outcome, metrics
- **Articles**: Data models with category, date, content sections
- **Jobs**: Data models with role details, requirements, benefits

### 7.4 Routing

- Clean URLs using Blazor routing
- Dynamic routes for detail pages: `/case-studies/{id}`, `/insights/{id}`, `/careers/{id}`
- 404 handling for invalid routes

### 7.5 SEO Considerations

- Meta tags and descriptions for each page
- OpenGraph tags for social sharing
- Structured data for organization and articles
- Sitemap.xml generation
- Prerendering support in Blazor Server

### 7.6 Accessibility

- ARIA labels for interactive elements
- Keyboard navigation support
- Sufficient color contrast (WCAG AA minimum)
- Alt text for all images
- Form labels and error associations

### 7.7 Performance

- Image optimization and lazy loading
- CSS and JS minification
- Gzip compression
- Browser caching headers
- Blazor component virtualization for long lists

---

## 8. Non-Goals / Out-of-Scope

### 8.1 Explicitly Excluded

1. **E-commerce Functionality**: No shopping cart, payment processing, or transactions
2. **User Authentication/Registration**: Client login is external link only
3. **Client Portal**: No logged-in client area or dashboard
4. **Real-time Chat**: No live chat or messaging features
5. **Blog Comments**: Articles are read-only, no commenting system
6. **Multi-language Support**: English only (though platform content mentions translation capabilities)
7. **Mobile App**: Web-only, no native mobile applications
8. **Complex CMS**: No admin panel for content editing (content updates via code/config)
9. **Analytics Dashboard**: No built-in analytics UI (use Google Analytics externally)
10. **Search Functionality**: No site-wide search (can be added later)
11. **Job Application Portal**: Applications handled via form submission/email, no applicant tracking system
12. **Newsletter Management**: Email capture may link to external service (Mailchimp, etc.)

### 8.2 Deferred Features (Future Enhancements)

1. **Advanced Filtering**: Case studies and insights filtering beyond basic categories
2. **Related Content Algorithms**: Automated related articles/case studies matching
3. **Performance Metrics Dashboard**: Visual analytics within the site
4. **Chatbot/AI Assistant**: Automated inquiry handling
5. **Video Content**: Beyond background videos (e.g., client testimonials, platform demos)
6. **Interactive Platform Demos**: Sandbox or trial environments
7. **Resource Downloads**: Beyond individual article downloads
8. **Event Calendar**: For webinars, conferences, etc.

---

## 9. Assumptions & Open Questions

### 9.1 Assumptions

1. **Content Volume**:
   - Assume 3-6 case studies initially
   - Assume 10-20 insights articles initially
   - Assume 3-5 active job listings

2. **Third-party Services**:
   - Email sending will use SMTP or a service like SendGrid
   - Map integration will use Google Maps embed
   - Client login links to external system (URL to be provided)

3. **Browser Support**:
   - Modern browsers: Chrome, Firefox, Safari, Edge (last 2 versions)
   - No IE11 support required

4. **Hosting**:
   - Hosted on Windows Server with IIS or Azure App Service
   - HTTPS/SSL certificate in place
   - Domain: zolv.com (or similar)

5. **Content Updates**:
   - Content updated infrequently (monthly or quarterly)
   - Updates made via code deployment, not real-time CMS

6. **Form Submissions**:
   - Contact wizard and application forms send email notifications
   - No database storage of submissions required initially

### 9.2 Open Questions

1. **Figma Design Access**:
   - ❓ Are Figma design files accessible for detailed measurements and asset export?
   - **Status**: Figma links provided but not accessible during PRD creation
   - **Resolution Needed**: Request access or export design assets (images, icons, exact spacing)

2. **Content Data Source**:
   - ❓ Where will actual case study content, images, and metrics come from?
   - **Current**: Template content available in MATTER directory
   - **Resolution Needed**: Final content approval and real client data/images

3. **Client Login Destination**:
   - ❓ What is the URL for the client login link in navigation?
   - **Resolution Needed**: Provide external portal URL

4. **Email Configuration**:
   - ❓ What email service should be used for form submissions?
   - ❓ What is the destination email address for inquiries?
   - **Assumption**: enquiries@zolv.com based on contact page content

5. **Video Assets**:
   - ❓ Are actual video files available for background videos on hero sections?
   - **Resolution Needed**: Provide video files or approve placeholder/stock footage

6. **Logo Assets**:
   - ❓ Are high-resolution client logos available for display?
   - **Resolution Needed**: Provide logo files for Virgin Holidays, HF Holidays, CV Villas, Monarch, Kuoni, Ramble Worldwide

7. **Photography**:
   - ❓ Are professional photography assets available for decorative elements?
   - **Resolution Needed**: Provide image library or approve stock photography usage

8. **Contact Wizard Steps 2 & 3**:
   - ❓ What specific information should be collected in wizard steps 2 and 3?
   - **Assumption**: 
     - Step 2: Name, Email, Phone, Company
     - Step 3: Project details/message
   - **Resolution Needed**: Confirm required fields and validation rules

9. **Analytics Integration**:
   - ❓ Should Google Analytics or other tracking be integrated?
   - **Resolution Needed**: Provide GA tracking ID if required

10. **Microsoft Partner Badge**:
    - ❓ Is the Microsoft Partner badge in the footer linked, and to where?
    - **Resolution Needed**: Provide badge image and link URL

11. **Social Media Links**:
    - ❓ What are the URLs for Facebook, Instagram, Twitter social media profiles?
    - **Resolution Needed**: Provide social media profile URLs

12. **Job Application Processing**:
    - ❓ Should CV files be emailed or stored on server?
    - ❓ What file types and size limits for CV uploads?
    - **Resolution Needed**: Define file handling requirements

### 9.3 Clarifications Needed

1. **Timeline Component**: Exact visual design for company story timeline needs confirmation from Figma
2. **Platform Diagram**: Interactive behavior and exact connection visualization needs Figma reference
3. **Feature Icons**: Icon set for platform features needs to be identified or designed
4. **Responsive Breakpoints**: Specific breakpoints for tablet and mobile layouts
5. **Animation Timing**: Specific duration and easing for transitions and animations

---

## 10. Success Metrics (Post-Launch)

While not part of the build, these metrics will validate success:

1. **Engagement**:
   - Time on site
   - Pages per session
   - Bounce rate by landing page

2. **Conversion**:
   - Contact wizard completion rate
   - Step drop-off analysis in wizard
   - Form submission to response ratio

3. **Content Performance**:
   - Most viewed case studies
   - Most read insights
   - CTA click-through rates

4. **Technical Performance**:
   - Page load time (target: < 3 seconds)
   - Lighthouse scores (target: 90+ on Performance, Accessibility, Best Practices, SEO)
   - Error rate (target: < 1%)

5. **Recruitment**:
   - Career page visits
   - Job application submissions per role

---

## 11. Implementation Phases

### Phase 1: Foundation (Week 1)
- Set up Blazor Server project structure
- Implement shared layout (header, footer, navigation)
- Set up routing infrastructure
- Implement design system (colors, typography, base components)

### Phase 2: Core Pages (Weeks 2-3)
- Implement Home page
- Implement About page
- Implement Our Approach page
- Implement Platform page

### Phase 3: Content Pages (Week 4)
- Implement Integrations page
- Implement Case Studies list and detail pages
- Implement Insights list and detail pages
- Set up data models and content loading

### Phase 4: Interactive Features (Week 5)
- Implement Contact Wizard component
- Implement FAQ Accordion
- Implement Filter Tabs
- Implement Platform Diagram
- Implement Application Form

### Phase 5: Refinement (Week 6)
- Implement Career detail page
- Polish animations and transitions
- Optimize performance
- Complete responsive design
- Testing and bug fixes

### Phase 6: Launch Prep (Week 7)
- SEO optimization
- Accessibility audit
- Browser testing
- Content population
- Deployment preparation

---

## 12. Appendix

### 12.1 Content Page Mapping

| MATTER File | Website Page |
|-------------|--------------|
| home-content.md | Home (Index) |
| about-page-content.md | About |
| services-page-content.md | Our Approach |
| platform-page-content.md | Platform |
| integrations-page-content.md | Integrations |
| case-studies-page-content.md | Case Studies List |
| case-study-detail-page-content.md | Case Study Detail (template) |
| insights-page-content.md | Insights List |
| insights-detail-page-content.md | Insight Detail (template) |
| contact-page-content.md | Contact |
| career-detail-page-content.md | Career Detail (template) |

### 12.2 Figma Links Reference

- Node 2-1440: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-1440&m=dev)
- Node 2-1688: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-1688&m=dev)
- Node 2-2150: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2150&m=dev)
- Node 2-2261: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2261&m=dev)
- Node 2-2407: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2407&m=dev)
- Node 2-2842: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2842&m=dev)
- Node 2-2521: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2521&m=dev)
- Node 2-2659: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2659&m=dev)
- Node 2-2772: [Link](https://www.figma.com/design/ZxWFmkKVkp0oWyazSVP4xx/Untitled?node-id=2-2772&m=dev)

**Note**: Figma links were not accessible during PRD creation. Design system specifications were extracted from platform-page-content.md which includes detailed design specifications.

### 12.3 Key Component Specifications

#### Contact Wizard Component
- **Type**: Multi-step form
- **Steps**: 3
- **Step 1**: Partnership type selection (6 radio options)
- **Step 2**: Contact information (name, email, phone, company)
- **Step 3**: Project details and message
- **Validation**: Required fields at each step
- **State**: Preserves data across steps
- **Submission**: Email to enquiries@zolv.com

#### Platform Diagram Component
- **Type**: Interactive visualization
- **Elements**: Central WTP hub with 6 connections
- **Connections**: Your travel platform, Book flow, CRM, API, Systems, Support
- **Interactions**: Hover to highlight, tooltips
- **Style**: Purple theme with connecting lines

#### FAQ Accordion Component
- **Type**: Expandable Q&A list
- **Items**: 5 questions on Integrations page
- **Behavior**: Click to expand/collapse
- **Multiple**: Multiple items can be open simultaneously
- **Animation**: Smooth height transition

---

## 13. Document Control

**Author**: GitHub Copilot  
**Reviewers**: TBD  
**Approval**: TBD  
**Version History**:
- v1.0 - January 31, 2026 - Initial PRD created from MATTER content and issue requirements

**Next Steps**:
1. Review and approval of this PRD
2. Resolution of open questions (Section 9.2)
3. Obtain design assets from Figma
4. Begin Phase 1 implementation

---

**END OF DOCUMENT**
