# Du-Track Customization Guide

## Personalizing Your Installation

This guide will help you customize Du-Track to match your institution's branding.

### Branding Elements

#### Logos and Icons
Replace the following files in `static/assets/img/` with your own:

1. **logo.png** - Main logo (used in dashboard header)
   - Recommended size: 200x60 pixels
   - Format: PNG with transparent background

2. **logo-white.png** - White version of logo (used on login pages)
   - Recommended size: 200x60 pixels
   - Format: PNG with transparent background
   - Should be visible on dark backgrounds

3. **logo-small.png** - Small logo for mobile view
   - Recommended size: 30x30 pixels
   - Format: PNG with transparent background

4. **favicon.png** - Browser tab icon
   - Recommended size: 32x32 pixels
   - Format: PNG

#### Images to Customize

1. **login.jpg** - Background image for login page
   - Recommended size: 1920x1080 pixels
   - Should be a welcoming educational environment

2. **user.jpg** - Default user avatar
   - Recommended size: 200x200 pixels
   - Used when users don't have profile pictures

3. **img-01.jpg** - Default placeholder image
   - Recommended size: 800x600 pixels

### Color Scheme

The main colors are defined in `static/assets/css/style.css`. You can customize:
- Primary color
- Secondary color
- Background colors
- Text colors

### Title and Naming

All page titles have been updated to "Du-Track". You can further personalize by:
1. Editing template files in `templates/` directory
2. Modifying the `HOME_PAGE_TITLE` in settings if needed

### Application Settings

Edit `Home/settings.py` to customize:
- Time zone: `TIME_ZONE = 'Your/Timezone'`
- Language: `LANGUAGE_CODE = 'en-us'`
- Site name and other Django settings

### Footer Customization

Add your institution details and contact information in the base template.

## Quick Checklist

- [ ] Replace logo.png with your institution's logo
- [ ] Replace logo-white.png with white version
- [ ] Replace logo-small.png for mobile
- [ ] Update favicon.png
- [ ] Change login.jpg background
- [ ] Update user.jpg default avatar
- [ ] Customize color scheme in CSS
- [ ] Update footer with your contact info
- [ ] Set correct timezone in settings.py

---

**Note:** After making changes to static files, run:
```bash
python manage.py collectstatic
```

For personalized assistance, visit: https://github.com/Aliipou/du-track
