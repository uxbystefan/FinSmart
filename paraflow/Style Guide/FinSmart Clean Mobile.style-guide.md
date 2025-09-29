# FinSmart Clean Mobile Style Guide

## Colors
### Primary Colors
- **primary-base**: `text-[#2563EB]` or `bg-[#2563EB]` - Professional trust-inspiring blue
- **primary-lighter**: `bg-[#3B82F6]` - Interactive states
- **primary-darker**: `text-[#1D4ED8]` or `bg-[#1D4ED8]` - Deep blue emphasis

### Secondary Colors
- **secondary-base**: `text-[#F97316]` or `bg-[#F97316]` - Vibrant orange accent
- **secondary-lighter**: `bg-[#FB923C]` - Hover states
- **secondary-darker**: `text-[#EA580C]` or `bg-[#EA580C]` - Active emphasis

### Background Colors
- **bg-page**: `bg-white` - Primary clean white background
- **bg-container-primary**: `bg-white` - Main cards, content containers
- **bg-container-secondary**: `bg-gray-50` - Secondary content areas
- **bg-container-inset**: `bg-gray-50` - Input fields, form elements
- **bg-container-accent**: `bg-blue-50` - Subtle blue highlighting
- **bg-bottom-navigation**: `bg-white` - Navigation bar background

### Text Colors
- **color-text-primary**: `text-gray-900` - Main headings and primary content
- **color-text-secondary**: `text-gray-700` - Subheadings and descriptions
- **color-text-tertiary**: `text-gray-500` - Supporting information
- **color-text-quaternary**: `text-gray-400` - Placeholder text
- **color-text-on-dark-primary**: `text-white` - Text on blue backgrounds
- **color-text-on-dark-secondary**: `text-blue-100` - Secondary text on blue backgrounds
- **color-text-link**: `text-[#2563EB]` - Links and interactive text elements

### Functional Colors
Used sparingly to maintain clean aesthetic while providing clear status indicators for financial data.
- **color-success-default**: `#10B981` - Positive financial indicators, gains
- **color-success-light**: `#D1FAE5` - Success notifications background
- **color-error-default**: `#EF4444` - Losses, alerts, errors
- **color-error-light**: `#FEE2E2` - Error notifications background
- **color-warning-default**: `#F59E0B` - Caution indicators
- **color-warning-light**: `#FEF3C7` - Warning notifications background
- **color-neutral-default**: `#6B7280` - Neutral financial data
- **color-neutral-light**: `#F3F4F6` - Neutral backgrounds

### Data Visualization Charts
Optimized for financial data clarity and accessibility.
- **Primary Data**: #2563EB (Primary Blue)
- **Secondary Data**: #F97316 (Orange)
- **Supporting Colors**: #10B981 (Green), #EF4444 (Red), #8B5CF6 (Purple), #06B6D4 (Cyan)
- **Neutral Tones**: #E5E7EB, #D1D5DB, #9CA3AF, #6B7280, #374151

## Typography
- **Font Stack**:
  - **font-family-base**: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif` — Clean, professional sans-serif optimized for mobile readability

- **Font Size & Weight**:
  - **Caption**: 10px / 400 - Navigation labels, fine print
  - **Body small**: 12px / 400 - Supporting details, metadata
  - **Body default**: 14px / 400 - Main content, descriptions
  - **Card Title / Emphasized Text**: 14px / 600 - Card headings, important labels
  - **Page Title**: 20px / 600 - Screen titles, main headings
  - **Financial Values**: 18px / 700 - Currency amounts, key metrics
  - **Headline**: 28px / 600 - Welcome messages, major sections
  - **Display**: 36px / 700 - Hero numbers, prominent financial figures

- **Line Height**: 1.4 - Optimized for mobile reading comfort

## Border Radius
- **Small**: 8px — Small elements, tags, badges
- **Medium**: 12px — Input fields, buttons, cards
- **Large**: 16px — Major containers, modal dialogs
- **Full**: full — Profile avatars, toggle switches, circular elements

## Layout & Spacing
- **Spacing Scale**:
  - **Base Unit**: 4px
  - **Tight**: 8px - Closely related elements, icon spacing
  - **Compact**: 12px - List items, form element spacing
  - **Standard**: 16px - General padding, section spacing
  - **Comfortable**: 24px - Major section breaks, card spacing

## Create Boundaries
Clean separation using subtle shadows and surface contrast for professional financial interface.

### Borders
- **case 1**: Minimal borders for clean aesthetic
- **case 2**: When needed for form inputs and active states
  - **Default**: 1px solid #E5E7EB - Form inputs, inactive states
  - **Focus**: 2px solid #2563EB - Active input fields, focused elements
  - **Error**: 1px solid #EF4444 - Error states

### Dividers
- **case 1**: Subtle separation using background color contrast
- **case 2**: When explicit division needed: `border-t border-gray-100` or `border-b border-gray-100`

### Shadows & Effects
Professional depth hierarchy for trustworthy financial interface.
- **case 1**: Clean flat design for most elements
- **case 2 (subtle)**: `shadow-[0_1px_3px_rgba(0,0,0,0.1)]` - Input fields, small cards
- **case 3 (moderate)**: `shadow-[0_4px_6px_rgba(0,0,0,0.05)]` - Main cards, containers
- **case 4 (prominent)**: `shadow-[0_8px_25px_rgba(0,0,0,0.08)]` - Modal dialogs, floating elements

## Assets
### Image
- For normal `<img>`: `object-cover`
- For `<img>` with overlay: `object-cover brightness-95`
- For background images: `object-cover brightness-90`

### Logo
- **Icon-based**: Use a clean, professional FontAwesome icon relevant to finance
- **Graphic**: `fa-chart-line` for investment focus, `fa-wallet` for personal finance, `fa-brain` for AI features

### Icon
- Use Lucide icons from Iconify for consistent, clean aesthetic
- Each icon centered in square container matching icon size
- Use Tailwind font size classes for consistent scaling
- Example:
  ```html
  <div class="flex items-center justify-center bg-transparent w-5 h-5">
    <iconify-icon icon="lucide:dollar-sign" class="text-lg"></iconify-icon>
  </div>
  ```

## Page Layout - Mobile
```html
<!-- Mobile Layout Template: FinSmart AI optimized for 390px width -->
<body class="w-[390px] min-h-[844px] bg-white font-['-apple-system','BlinkMacSystemFont','Segoe_UI','Roboto','Helvetica_Neue','Arial',sans-serif] leading-[1.4]">

  <!-- Top Fixed Header: Status bar and navigation -->
  <div class="z-10 fixed top-0 w-full bg-white border-b border-gray-100">
    <!-- Default Top Safe Area -->
    <div class="h-[env(safe-area-inset-top,0px)]"></div>
    <!-- Top Navigation Bar: 56px height for comfortable touch targets -->
    <header class="h-14 flex items-center justify-between px-4">
      <!-- Navigation content goes here -->
    </header>
  </div>

  <!-- Top Spacer: Prevents content overlap -->
  <div>
    <div class="h-[env(safe-area-inset-top,0px)]"></div>
    <div class="h-14"></div>
  </div>
  
  <!-- Main Scrollable Content Area -->
  <main class="pb-4 space-y-4">
    <!-- Main content with standard horizontal padding -->
    <section class="px-4">
      <!-- Financial content goes here -->
    </section>
  </main>

  <!-- Bottom Spacer: Account for fixed bottom elements -->
  <div>
    <div class="mt-4 h-[72px]"></div>
    <div class="h-[env(safe-area-inset-bottom,0px)]"></div>
    <!-- FAB space if needed -->
    <div class="h-14"></div>
  </div>

  <!-- Bottom Fixed Area: Navigation and FAB -->
  <div class="z-10 fixed bottom-0 w-full flex flex-col">

    <!-- Floating Action Button (Optional) -->
    <div class="flex flex-col gap-4 px-4 pb-4 items-end">
      <button class="w-14 h-14 bg-[#F97316] hover:bg-[#EA580C] rounded-full flex items-center justify-center shadow-[0_8px_25px_rgba(0,0,0,0.15)]">
        <iconify-icon icon="lucide:plus" class="text-white text-xl"></iconify-icon>
      </button>
    </div>

    <!-- Bottom Navigation -->
    <div class="bg-white border-t border-gray-100">
      <nav class="flex justify-around py-3 px-2">
        <!-- Navigation Item: Active state -->
        <div class="flex flex-1 flex-col items-center gap-1">
          <div class="w-6 h-6 flex items-center justify-center">
            <iconify-icon icon="lucide:home" class="text-[#2563EB] text-lg"></iconify-icon>
          </div>
          <span class="text-[10px] font-medium text-[#2563EB]">Home</span>
        </div>
        <!-- Navigation Item: Default state -->
        <div class="flex flex-1 flex-col items-center gap-1">
          <div class="w-6 h-6 flex items-center justify-center">
            <iconify-icon icon="lucide:trending-up" class="text-gray-400 text-lg"></iconify-icon>
          </div>
          <span class="text-[10px] font-normal text-gray-400">Invest</span>
        </div>
      </nav>
      <!-- Bottom Safe Area -->
      <div class="h-[env(safe-area-inset-bottom,0px)]"></div>
    </div>
  </div>
</body>
```

## Tailwind Component Examples
### Basic
- **Progress bars**: `h-2 bg-gray-200 rounded-full overflow-hidden`
- **Button**:
  - Primary: `bg-[#2563EB] hover:bg-[#1D4ED8] text-white px-6 py-3 rounded-xl font-medium flex items-center justify-center`
  - Secondary: `bg-[#F97316] hover:bg-[#EA580C] text-white px-6 py-3 rounded-xl font-medium flex items-center justify-center`
  - Text: `text-[#2563EB] hover:text-[#1D4ED8] font-medium flex items-center`

- **Label/Tag/Badge**:
  - Success: `bg-[#D1FAE5] text-[#047857] px-3 py-1 rounded-full text-xs font-medium flex items-center`
  - Error: `bg-[#FEE2E2] text-[#DC2626] px-3 py-1 rounded-full text-xs font-medium flex items-center`
  - Neutral: `bg-gray-100 text-gray-700 px-3 py-1 rounded-full text-xs font-medium flex items-center`

### Data Entry
- **Input Field**: `w-full px-4 py-3 bg-gray-50 border border-gray-200 rounded-xl focus:ring-2 focus:ring-[#2563EB] focus:border-[#2563EB] outline-none`
- **Select**: `w-full px-4 py-3 bg-gray-50 border border-gray-200 rounded-xl focus:ring-2 focus:ring-[#2563EB] appearance-none`

### Container
- **Main Card**: `bg-white rounded-xl shadow-[0_4px_6px_rgba(0,0,0,0.05)] p-4`
- **Financial Metric Card**: `bg-white rounded-xl shadow-[0_4px_6px_rgba(0,0,0,0.05)] p-6 border-l-4 border-[#2563EB]`

## Additional Notes
This style guide prioritizes trust, clarity, and accessibility essential for financial applications. The color palette balances professional credibility with engaging visual hierarchy. Typography and spacing are optimized for mobile financial data consumption and interaction.

<colors_extraction>
#2563EB
#3B82F6
#1D4ED8
#F97316
#FB923C
#EA580C
#FFFFFF
#F9FAFB
#F3F4F6
#EFF6FF
#111827
#374151
#6B7280
#9CA3AF
#E0F2FE
#DBEAFE
#2563EB
#10B981
#D1FAE5
#EF4444
#FEE2E2
#F59E0B
#FEF3C7
#6B7280
#F3F4F6
#8B5CF6
#06B6D4
#E5E7EB
#D1D5DB
#9CA3AF
#6B7280
#374151
#E5E7EB
#EF4444
#F3F4F6
rgba(0,0,0,0.1)
rgba(0,0,0,0.05)
rgba(0,0,0,0.08)
#047857
#DC2626
rgba(0,0,0,0.15)
</colors_extraction>