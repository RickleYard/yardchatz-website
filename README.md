# Yard Chatz Website

A modern, responsive website for the Yard Chatz app featuring AI-powered social media capabilities, iOS download options, and Android pre-order functionality.

## 🚀 Features

- **Responsive Design**: Works perfectly on all devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **iOS Download Section**: QR code and App Store links
- **Android Pre-order System**: Crowdfunding-style waitlist with $50,000 goal
- **iPhone Purchase Section**: For Android users who want immediate access
- **Contact Forms**: User engagement and feedback collection
- **Mobile-First Navigation**: Hamburger menu for mobile devices

## 📁 File Structure

```
yardchatz-website/
├── index.html          # Main HTML file
├── styles.css          # CSS styling and responsive design
├── script.js           # JavaScript functionality
├── README.md           # This file
└── assets/             # Images and media files (create this folder)
    ├── logo.png        # Yard Chatz logo
    ├── hero-app.png    # Hero section app preview
    ├── screenshot1.png # App screenshots
    ├── screenshot2.png
    ├── screenshot3.png
    ├── screenshot4.png
    └── qr-code.png     # Download QR code
```

## 🛠️ Setup Instructions

### 1. Create Assets Folder
Create an `assets` folder in the `yardchatz-website` directory and add the following images:

- **logo.png**: Your Yard Chatz app logo (40x40px recommended)
- **hero-app.png**: App preview image for hero section
- **screenshot1.png** through **screenshot4.png**: App screenshots
- **qr-code.png**: QR code that links to your App Store page

### 2. Customize Content
Edit the following in `index.html`:

- **App Store Links**: Replace `#` with actual App Store URLs
- **Contact Information**: Update email, social media handles
- **iPhone Purchase Links**: Add affiliate links to iPhone sales pages
- **Company Information**: Update copyright, legal links

### 3. Customize Styling
Modify `styles.css` to match your brand:

- **Colors**: Update CSS variables in `:root` section
- **Fonts**: Change Google Fonts import and font-family
- **Logo**: Adjust logo dimensions and styling

### 4. Customize Functionality
Update `script.js` for:

- **Form Handling**: Connect forms to your backend/email service
- **Progress Bar**: Update with real funding data
- **Analytics**: Add Google Analytics or other tracking

## 🌐 Deployment

### Option 1: GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source branch (usually `main`)

### Option 2: Netlify
1. Drag and drop the folder to Netlify
2. Configure custom domain if needed
3. Set up form handling

### Option 3: Vercel
1. Connect GitHub repository to Vercel
2. Deploy automatically on push
3. Configure custom domain

## 📱 Customization Guide

### Colors
Update these CSS variables in `styles.css`:

```css
:root {
    --primary-color: #007AFF;      /* Main brand color */
    --secondary-color: #5856D6;    /* Secondary brand color */
    --accent-color: #FF2D92;       /* Accent/highlight color */
    --success-color: #34C759;      /* Success/green color */
    --warning-color: #FF9500;      /* Warning/orange color */
    --error-color: #FF3B30;        /* Error/red color */
}
```

### Typography
Change fonts by updating the Google Fonts import:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

Then update the font-family in CSS:

```css
body {
    font-family: 'YourFont', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

### Content Updates
Key areas to customize:

1. **Hero Section**: Main headline and description
2. **Features**: Update feature descriptions and icons
3. **Screenshots**: Replace with actual app screenshots
4. **Funding Goal**: Adjust the $50,000 target if needed
5. **Pledge Tiers**: Modify reward descriptions and amounts

## 🔧 Technical Features

- **CSS Grid & Flexbox**: Modern layout system
- **CSS Variables**: Easy theming and customization
- **Intersection Observer**: Scroll-triggered animations
- **Form Validation**: Client-side form validation
- **Responsive Images**: Optimized for all screen sizes
- **Progressive Enhancement**: Works without JavaScript

## 📊 Form Integration

### Android Signup Form
The Android pre-order form includes:
- Name, email, phone, pledge amount
- Form validation
- Success/error notifications
- Progress bar updates

### Contact Form
General contact form with:
- Name, email, message fields
- Form validation
- Success notifications

### Backend Integration
To connect forms to your backend:

1. **Replace form action URLs** in HTML
2. **Update JavaScript form handlers** to send data to your API
3. **Add CSRF tokens** if using frameworks like Django/Rails
4. **Implement email notifications** for form submissions

## 🎨 Design System

The website uses a consistent design system:

- **Spacing**: 8px grid system (8px, 16px, 24px, 32px, 48px, 64px, 80px)
- **Border Radius**: 8px, 12px, 20px for different component sizes
- **Shadows**: Subtle shadows for depth and hierarchy
- **Transitions**: 0.3s cubic-bezier for smooth animations
- **Breakpoints**: 768px and 480px for responsive design

## 🚀 Performance Optimization

- **Minified CSS/JS**: Consider minifying for production
- **Image Optimization**: Compress images for web
- **Lazy Loading**: Implement for images if needed
- **CDN**: Use CDN for external resources
- **Caching**: Set appropriate cache headers

## 🔒 Security Considerations

- **HTTPS**: Always use HTTPS in production
- **Form Validation**: Server-side validation required
- **CSRF Protection**: Implement if using server-side forms
- **Input Sanitization**: Sanitize all user inputs
- **Rate Limiting**: Prevent form spam

## 📈 Analytics & Tracking

Add these to track website performance:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>

<!-- Facebook Pixel -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'YOUR_PIXEL_ID');
  fbq('track', 'PageView');
</script>
```

## 🆘 Support

For questions or issues:
- Check the code comments for guidance
- Review browser console for JavaScript errors
- Test on different devices and browsers
- Validate HTML/CSS using online validators

## 📄 License

This website template is provided as-is for the Yard Chatz app. Customize as needed for your specific requirements.
