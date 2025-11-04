# Changelog - Mural de Testemunhos

## Features Added

### 1. ✅ Vercel Analytics Integration
- Added Vercel Analytics via CDN (works when deployed to Vercel)
- Tracks page views and user interactions
- Custom events tracked:
  - Page views
  - Testimonial submissions
  - Prayer clicks
  - Social shares
  - Filter usage
  - Newsletter subscriptions
  - Welcome popup interactions
  - FAB (Floating Action Button) clicks

**Note:** When deployed to Vercel, the analytics will automatically track visitors per day. For local development, the analytics script is included via CDN.

### 2. 🎉 Welcome Popup for New Visitors
- Beautiful welcome modal that appears for first-time visitors
- Stored in localStorage to avoid showing again
- Encourages engagement and explains the purpose of the site
- Tracks when users close the popup

### 3. 📧 Newsletter Subscription Popup
- Appears after 5 seconds (non-intrusive)
- Allows visitors to subscribe for daily testimonies and verses
- Stores subscription in localStorage
- Toast notification confirms successful subscription
- Tracks subscription events

### 4. 📱 Social Sharing Functionality
- Added social sharing buttons to each testimony card:
  - Facebook sharing
  - WhatsApp sharing
  - Twitter sharing
  - Copy link to clipboard
- Makes it easy for visitors to share testimonies
- Tracks which platforms are used most

### 5. ✨ Daily Verse Feature
- Beautiful animated banner showing a daily verse
- Different verse each day (rotates based on date)
- Includes inspirational Bible verses
- Encourages daily engagement

### 6. 🎯 Floating Action Button (FAB)
- Quick access button to share a testimony
- Smooth scroll to the share form
- Animated hover effects
- Tracks FAB clicks

### 7. 🔔 Toast Notifications
- Non-intrusive notifications for user actions
- Confirms prayer submissions
- Confirms newsletter subscriptions
- Confirms link copying

### 8. 📊 Enhanced Analytics Tracking
All user interactions are tracked:
- Page views
- Testimonial submissions (with category)
- Prayer clicks (with testimonial ID)
- Social shares (with platform and testimonial ID)
- Filter usage (with category)
- Newsletter subscriptions (with email)
- Welcome popup interactions
- FAB clicks

## UX Improvements

1. **Better Visual Feedback**: Toast notifications for actions
2. **Smoother Animations**: Enhanced CSS animations throughout
3. **Mobile Responsive**: All new features work on mobile devices
4. **Accessibility**: Proper ARIA labels and keyboard navigation
5. **User Guidance**: Welcome popup helps new users understand the site

## Technical Details

- **Package**: `@vercel/analytics` installed via npm
- **Analytics Method**: CDN script for plain HTML (works with Vercel deployment)
- **Storage**: Uses localStorage for user preferences
- **Compatibility**: Works in all modern browsers

## Deployment Notes

When deploying to Vercel:
1. Vercel will automatically detect and enhance analytics
2. Visitor tracking will be available in the Vercel dashboard
3. Daily visitor counts will be tracked automatically
4. Custom events will appear in analytics

## Next Steps (Optional Enhancements)

1. Connect newsletter to an email service (Mailchimp, SendGrid, etc.)
2. Add backend API for persistent testimonial storage
3. Add user authentication for personalized experience
4. Add more daily verses to the rotation
5. Add email verification for newsletter
6. Add share buttons for more platforms (Instagram, LinkedIn)

