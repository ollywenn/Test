# Zolv Travel Technology Website

A Blazor Server application implementing the Zolv travel technology company website based on content specifications and design requirements.

## Project Overview

This project delivers a complete marketing and client engagement platform for Zolv, showcasing their expertise in travel platform development and integration.

### Key Features

- **Blazor Server Architecture**: Server-side rendering with interactive components
- **Multi-step Contact Wizard**: 3-step form with progress tracking and validation
- **FAQ Accordion**: Interactive expand/collapse Blazor component
- **Filter Tabs**: Category filtering for insights content
- **Responsive Design**: Mobile-friendly layouts using CSS Grid and Flexbox
- **Brand Design System**: Custom purple/yellow color scheme per specifications

## Pages Implemented

1. **Home** (`/`) - Hero section, partnership models, platform overview, solutions showcase
2. **About** (`/about`) - Company mission, history timeline, founder profile, careers
3. **Our Approach** (`/our-approach`) - Partnership models, client experience, testimonials
4. **Platform** (`/platform`) - WTP platform features, capabilities showcase
5. **Integrations** (`/integrations`) - Integration categories, FAQ accordion
6. **Case Studies** (`/case-studies`) - Client testimonials, partner logos
7. **Insights** (`/insights`) - Articles with category filtering
8. **Contact** (`/contact`) - Multi-step wizard, location information

## Blazor Interactive Components

### ContactWizard (`Components/Shared/ContactWizard.razor`)

Multi-step form wizard with:
- Step 1: Partnership type selection (6 options)
- Step 2: Contact information with validation
- Step 3: Project details and requirements
- Progress indicator
- Form validation using DataAnnotations
- Success confirmation

### FAQAccordion (`Components/Shared/FAQAccordion.razor`)

Interactive FAQ component with:
- Expand/collapse functionality
- Multiple items can be open simultaneously
- Smooth animations
- 5 travel technology FAQs

## Technology Stack

- **.NET 10**: Latest .NET framework
- **Blazor Server**: Server-side rendering with WebSocket communication
- **C#**: Application logic and components
- **Razor**: Component templates
- **CSS3**: Custom design system implementation
- **HTML5**: Semantic markup

## Getting Started

### Prerequisites

- .NET 10 SDK

### Running the Application

```bash
cd src/ZolvWeb
dotnet restore
dotnet run
```

The application will be available at `http://localhost:5214` (or the port specified in launchSettings.json).

### Building for Production

```bash
cd src/ZolvWeb
dotnet publish -c Release
```

## Project Structure

```
src/ZolvWeb/
├── Components/
│   ├── Layout/
│   │   ├── MainLayout.razor      # Main page layout
│   │   ├── NavMenu.razor          # Top navigation
│   │   └── Footer.razor           # Site footer
│   ├── Pages/
│   │   ├── Home.razor
│   │   ├── About.razor
│   │   ├── OurApproach.razor
│   │   ├── Platform.razor
│   │   ├── Integrations.razor
│   │   ├── CaseStudies.razor
│   │   ├── Insights.razor
│   │   └── Contact.razor
│   └── Shared/
│       ├── ContactWizard.razor    # Multi-step form wizard
│       └── FAQAccordion.razor     # FAQ accordion component
├── wwwroot/
│   ├── app.css                    # Main stylesheet
│   └── favicon.png
├── Program.cs                     # Application startup
└── ZolvWeb.csproj
```

## Design System

### Colors

- **Primary Purple**: `#35226E`
- **Yellow Accent**: `#FDD712`
- **Dark Gray Text**: `#595959`
- **Light Gray Background**: `#EAEBF3`

### Typography

- **Primary Font**: Plus Jakarta Sans (with fallbacks)
- **Hero Heading**: 64px, SemiBold
- **Section Headings**: 48px, SemiBold
- **Body Text**: 20px, Medium

## Content Source

All content is derived from the `/MATTER/Pages/` directory containing:
- Marketing documents
- Page content specifications
- Positioning and messaging materials

## Documentation

- **PRD**: Comprehensive Product Requirements Document at `/docs/PRD.md`
- 13 sections covering purpose, architecture, requirements, design system
- Detailed page specifications and interaction requirements

## Development Approach

Following the PRD requirements:
- **Blazor-first**: All interactivity implemented using Blazor components
- **No unnecessary JavaScript**: Only Blazor and HTML5 native features
- **Server-side rendering**: All state managed on the server
- **Form validation**: Using Blazor EditForm and DataAnnotations
- **Responsive**: CSS-based responsive design

## Future Enhancements

Potential improvements identified in PRD:
- CMS integration for content management
- Advanced filtering for case studies
- Real-time analytics dashboard
- Multi-language support
- Enhanced search functionality

## License

Copyright © 2025 Zolv Ltd. All Rights Reserved.
