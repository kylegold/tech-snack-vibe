---
description: >
  Comprehensive UI/UX design system generator that creates style guides from
  image analysis, transforms app concepts into production-ready design
  specifications with component libraries, and generates complete product
  specifications following SaaS best practices.
allowed_tools:
  - mcp__filesystem          # File operations for design specs
  - mcp__frame0-mcp-server   # Visual design and component creation
---

## Arguments

```
/ui-style-guide-generator 
[task=<analyze-images|create-from-concept|generate-ui|product-spec|full-workflow>]
[design_source=<image-analysis|app-concept|existing-guide>]
[output_format=<style-guide|ui-components|html-prototype|product-spec|full-system>]
[app_name="<your app name>"]
[app_description="<brief description>"]
[target_platform=<ios|android|web|cross-platform>]
[design_style=<modern|minimal|playful|professional|custom>]
[include_pondering=<yes|no>]
```
*Defaults → `task=analyze-images  design_source=image-analysis  output_format=style-guide  target_platform=cross-platform  design_style=modern  include_pondering=yes`*

### Example

```
/ui-style-guide-generator 
task=full-workflow
app_name="FocusLock"
app_description="Productivity app that blocks distracting apps with educational unlocks"
target_platform=ios
design_style=minimal
include_pondering=yes
```

---

## Context – what the AI should do

### Phase 1: Design Analysis & Style Guide Creation

1. **Image Analysis Mode** (if task includes analyze-images)
   * Expert UX/UI designer approach:
     ```
     <pondering>
     Looking at these images, I'm seeing a design language that speaks to...
     - The app's aesthetics and principles it conforms to
     - How the visual choices make users feel
     - The emotional journey through color and typography
     - Design patterns that reinforce the app's purpose
     </pondering>
     ```
   * Extract and document:
     - Color palette with exact hex codes
     - Typography hierarchy and usage
     - Component patterns
     - Spacing systems
     - Motion principles

2. **Style Guide Format** (comprehensive output)
   ```
   Color Palette
   Primary Colors
   * Primary White - #F8F9FA (Used for backgrounds and clean surfaces)
   * Primary Dark [Color] - #HEXCODE (Primary brand color for buttons, icons, and emphasis)
   
   Secondary Colors
   * Secondary [Color] Light - #HEXCODE (For hover states and secondary elements)
   * Secondary [Color] Pale - #HEXCODE (For backgrounds, selected states, and highlights)
   
   Accent Colors
   * Accent [Color] - #HEXCODE (For important actions and notifications)
   * Accent [Color] - #HEXCODE (For warnings and highlights)
   
   Functional Colors
   * Success Green - #HEXCODE (For success states and confirmations)
   * Error Red - #HEXCODE (For errors and destructive actions)
   * Neutral Gray - #HEXCODE (For secondary text and disabled states)
   * Dark Gray - #HEXCODE (For primary text)
   
   Background Colors
   * Background White - #FFFFFF (Pure white for cards and content areas)
   * Background Light - #HEXCODE (Subtle off-white for app background)
   * Background Dark - #HEXCODE (For dark mode primary background)
   
   Typography
   Font Family
   * Primary Font: SF Pro Text (iOS) / Roboto (Android)
   * Alternative Font: Inter (Web fallback)
   
   Font Weights
   * Regular: 400
   * Medium: 500
   * Semibold: 600
   * Bold: 700
   
   Text Styles
   Headings
   * H1: 28px/32px, Bold, Letter spacing -0.2px
      * Used for screen titles and major headers
   * H2: 24px/28px, Bold, Letter spacing -0.2px
      * Used for section headers and card titles
   * H3: 20px/24px, Semibold, Letter spacing -0.1px
      * Used for subsection headers and important text
   
   Body Text
   * Body Large: 17px/24px, Regular, Letter spacing 0px
      * Primary reading text for content
   * Body: 15px/20px, Regular, Letter spacing 0px
      * Standard text for most UI elements
   * Body Small: 13px/18px, Regular, Letter spacing 0.1px
      * Secondary information and supporting text
   
   Special Text
   * Caption: 12px/16px, Medium, Letter spacing 0.2px
      * Used for timestamps, metadata, and labels
   * Button Text: 16px/24px, Medium, Letter spacing 0.1px
      * Used specifically for buttons and interactive elements
   * Link Text: 15px/20px, Medium, Letter spacing 0px, Primary Color
      * Clickable text throughout the application
   
   Component Styling
   [Complete component specifications...]
   
   Spacing System
   * 4dp - Micro spacing (between related elements)
   * 8dp - Small spacing (internal padding)
   * 16dp - Default spacing (standard margins)
   * 24dp - Medium spacing (between sections)
   * 32dp - Large spacing (major sections separation)
   * 48dp - Extra large spacing (screen padding top/bottom)
   
   Motion & Animation
   * Standard Transition: 200ms, Ease-out curve
   * Emphasis Transition: 300ms, Spring curve (tension: 300, friction: 35)
   * Microinteractions: 150ms, Ease-in-out
   * Page Transitions: 350ms, Custom cubic-bezier(0.2, 0.8, 0.2, 1)
   
   Dark Mode Variants
   * Dark Background: #121212 (primary dark background)
   * Dark Surface: #1E1E1E (card backgrounds)
   * Dark Primary: #HEXCODE (adjusted for contrast)
   * Dark Text Primary: #EEEEEE
   * Dark Text Secondary: #B0BEC5
   ```

### Phase 2: Product Specification Development

3. **SaaS Founder Mode** (if task includes product-spec)
   * Take collaborative/consultative approach:
     ```
     As an experienced SaaS Founder who obsesses about product and solving 
     people's problems, I'll help transform this idea into a detailed project 
     specification focusing on the PROBLEM first.
     ```
   
   * Generate complete product specification:
     ```
     ## Elevator Pitch
     [Concise 1-2 sentence value proposition]
     
     ## Problem Statement
     [Clear articulation of the problem, backed by data if possible]
     
     ## Target Audience
     Primary: [Specific demographic with pain points]
     Secondary: [Additional user segment]
     
     ## USP (Unique Selling Proposition)
     [What makes this solution different and better]
     
     ## Target Platforms
     [iOS, Android, Web, etc.]
     
     ## Features List
     
     ### Core Functionality
     [] As a user, I want to [action] so that [benefit]
        [] [Sub-requirement or acceptance criteria]
        [] [Technical implementation note]
     
     ### User Account & Settings
     [] As a user, I want to [action] so that [benefit]
        [] [Sub-requirement]
     
     ### UX/UI Considerations
     [] [Screen or Interaction]
        [] [Description of different "states" of that screen]
        [] [How it handles state changes visually]
        [] [Animations, information architecture, visual hierarchy]
     
     ### Non-Functional Requirements
     [] Performance: [Specific metrics]
     [] Scalability: [Growth considerations]
     [] Security: [Data protection measures]
     [] Accessibility: [WCAG compliance level]
     
     ## Monetization
     [Detailed revenue model with pricing tiers]
     
     ## Critical Questions or Clarifications
     [Important decisions that need stakeholder input]
     ```

### Phase 3: Design Philosophy Development

4. **Concept Fusion** (when creating from app concept)
   * Process through design thinking:
     ```
     <pondering>
     This app needs to embody [core values]...
     The core challenge is creating a visual language that reinforces the app's purpose.
     This means the design itself should be:
     - [Design principle 1] - [Explanation]
     - [Design principle 2] - [Explanation]
     - [Design principle 3] - [Explanation]
     
     The color psychology is crucial here. We want colors that promote [emotion]...
     The typography should feel [quality]...
     The interaction design needs to embody [philosophy]...
     </pondering>
     ```
   
   * Generate design rationale:
     ```
     <pontificating>
     Fusing the design analysis with the app concept:
     - Visual metaphors that reinforce the app's purpose
     - Color choices that evoke intended emotions
     - Typography that supports content consumption
     - Interaction patterns that guide user behavior
     </pontificating>
     ```

### Phase 4: UI Implementation

5. **Design Guidelines Application**
   * Follow industry-veteran principles:
     ```
     <aesthetics>
     - Bold simplicity with intuitive navigation
     - Breathable whitespace for visual hierarchy
     - Strategic negative space for cognitive breathing room
     - Systematic color theory with purposeful accents
     - Typography hierarchy for information architecture
     - Visual density optimization
     - Motion choreography for spatial continuity
     - Accessibility-driven contrast ratios
     - Feedback responsiveness via state transitions
     - Content-first layouts prioritizing objectives
     </aesthetics>
     
     <practicalities>
     - Simulate iPhone device frame
     - Use lucide react icons
     - Use Tailwind for CSS
     - No scroll bars for simulated phone
     - Focus on UI/UX examples over functionality
     </practicalities>
     ```

6. **HTML Prototype Generation**
   * Create multiple screen variations:
     ```html
     <!DOCTYPE html>
     <html lang="en">
     <head>
       <meta charset="UTF-8">
       <title>[App Name] - [Screen Name]</title>
       <script src="https://cdn.tailwindcss.com"></script>
       <link href="https://unpkg.com/lucide@latest/dist/lucide.css" rel="stylesheet">
       <style>
         /* Design tokens from style guide */
         :root {
           --primary-deep-blue: #1E3A8A;
           --focus-green: #10B981;
           /* ... all color variables ... */
         }
       </style>
     </head>
     <body class="bg-gray-50">
       <!-- iPhone Frame -->
       <div class="mx-auto max-w-[375px] h-[812px] bg-black rounded-[3rem] p-3">
         <div class="bg-white h-full rounded-[2.5rem] overflow-hidden">
           <!-- Status Bar -->
           <div class="bg-white px-6 py-2 flex justify-between items-center text-xs">
             <span>9:41</span>
             <div class="flex gap-1">
               <i data-lucide="wifi" class="w-4 h-4"></i>
               <i data-lucide="signal" class="w-4 h-4"></i>
               <i data-lucide="battery" class="w-4 h-4"></i>
             </div>
           </div>
           
           <!-- Screen Content -->
           <div class="px-6 pb-6 h-full">
             <!-- Implementation based on screen type -->
           </div>
         </div>
       </div>
       
       <script src="https://unpkg.com/lucide@latest"></script>
       <script>lucide.createIcons();</script>
     </body>
     </html>
     ```

### Phase 5: Advanced Scenarios

7. **Complex UI Challenges**
   * For each design problem, generate 3 unique solutions:
     ```
     Example Problem: When a user has run out of free "emergency unlocks", 
     the only way they can unlock is to withdraw money from their account. 
     Account is pre-loaded with $25, costs $5 to unlock during block period.
     
     Solution 1: [Approach focused on deterrence]
     - Visual design emphasizing consequence
     - Clear display of account balance ($25) and cost ($5)
     - Red/warning colors for financial impact
     - Multi-step confirmation with friction
     
     Solution 2: [Approach focused on alternatives]
     - Prominent display of free unlock options
     - Visual hierarchy de-emphasizing paid unlock
     - Account balance shown subtly
     - Gamification of earning free unlocks
     
     Solution 3: [Approach focused on reflection]
     - Mindfulness prompt before payment
     - Visual breathing exercise
     - Show impact: "This $5 could buy..."
     - Progress visualization of money saved
     ```

### Phase 6: Evaluation & Optimization

8. **Design Quality Assurance**
   * Evaluate output against standards:
     ```
     EVALUATOR-OPTIMIZER CHECKLIST:
     □ Adheres to established design system
     □ Maintains consistency across all screens
     □ Follows accessibility guidelines
     □ Implements proper visual hierarchy
     □ Uses appropriate motion and transitions
     □ Optimizes for target platform conventions
     □ Validates color contrast ratios
     □ Ensures touch target sizes (min 44x44)
     ```

### Special Workflows

#### FocusLock Example Implementation
When app_name="FocusLock" or similar productivity apps:
- Implement mindful design principles
- Use calming color palette (deep blues, greens)
- Create intentional friction in UI
- Design reward-oriented feedback
- Implement deliberate interaction patterns
- 3-second press for unlock actions
- Progress visualization prominently displayed

#### Financial/Payment Flows
For apps with monetary transactions:
- Clear display of account balance
- Multiple confirmation steps
- Visual emphasis on consequences
- Alternative options prominently shown
- Undo/refund information visible
- Trust signals and security indicators

#### Educational Content Integration
For apps with learning components:
- Readable typography optimization
- Progress tracking visualization
- Completion celebration animations
- Content categorization UI
- Bookmark/favorite functionality
- Offline availability indicators

### Output Structure

Generate complete design package:
```
/ui-style-guide-generator/
├── style-guide.md (comprehensive guide)
├── product-spec.md (full specification)
├── design-tokens.json (programmatic values)
├── design-rationale.md (pondering/pontificating)
├── components/
│   ├── buttons.html
│   ├── cards.html
│   ├── forms.html
│   └── navigation.html
├── screens/
│   ├── onboarding/
│   │   ├── solution-1.html
│   │   ├── solution-2.html
│   │   └── solution-3.html
│   ├── dashboard.html
│   ├── settings.html
│   └── special-scenarios/
│       └── emergency-unlock.html
├── assets/
│   ├── colors.css
│   ├── typography.css
│   └── animations.css
└── evaluation-report.md

```

> Focus on creating cohesive, accessible, and psychologically-informed design systems that solve real user problems while maintaining beauty and usability. Every design decision should be intentional and serve both business goals and user needs.