# Raymond Website

A luxury real estate website built with React and Tailwind CSS.

## Features

- Responsive design for all devices
- Smooth animations with Framer Motion
- Enquiry popup form (appears after 4-5 seconds)
- Floating WhatsApp and Call buttons
- Image gallery with lightbox
- Floor plans section
- Location map
- Contact form with validation

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Navigate to the project directory:
   ```bash
   cd experion-website
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Configuration

### Contact Information

Edit `src/config/contact.js` to update:
- Phone numbers
- Email addresses
- WhatsApp number
- Social media links
- Address
- Company details

### Images and Media

Edit `src/config/media.js` to update:
- Logo images
- Hero slider images
- Gallery images
- Floor plan images
- Location map

### Adding Images

1. Place your images in the `public/images/` folder
2. Update the paths in `src/config/media.js`

Folder structure for images:
```
public/
  images/
    logo.png
    logo-white.png
    hero/
      hero-1.jpg
      hero-2.jpg
      hero-3.jpg
    about/
      about-main.jpg
      about-secondary.jpg
    highlights/
      location.jpg
      design.jpg
      amenities.jpg
      lifestyle.jpg
    floorplans/
      3bhk-type-a.jpg
      3bhk-type-b.jpg
      4bhk-type-a.jpg
      4bhk-type-b.jpg
    gallery/
      gallery-1.jpg
      gallery-2.jpg
      ...
    location/
      map.jpg
    amenities/
      pool.svg
      gym.svg
      ...
    decorative/
      cherry-blossom.png
```

## Color Scheme

The website uses these primary colors (from the original design):

- Primary Red: `#BA1E2C`, `#DC0B2A`
- Brown Accent: `#B7602F`, `#824218`
- Dark Text: `#222222`, `#262626`, `#333333`
- Gray Text: `#707070`, `#7C7C7C`
- Light Gray: `#D7D7D7`, `#DDDDDD`
- WhatsApp Green: `#42DB87`

## Build for Production

```bash
npm run build
```

This creates an optimized build in the `build` folder.

## Tech Stack

- React 18
- Tailwind CSS 3
- Framer Motion
- React Icons
- Swiper.js
- React Intersection Observer

## Project Structure

```
src/
  components/       # React components
    Header.jsx
    Hero.jsx
    About.jsx
    Highlights.jsx
    Amenities.jsx
    FloorPlans.jsx
    Gallery.jsx
    Location.jsx
    Footer.jsx
    EnquiryPopup.jsx
    FloatingButtons.jsx
  config/           # Configuration files
    contact.js      # Contact information
    media.js        # Image/video paths
  hooks/            # Custom React hooks
  App.js            # Main app component
  index.js          # Entry point
  index.css         # Global styles
```

## Customization

### Changing Colors

Update `tailwind.config.js` to modify the color palette:

```javascript
colors: {
  primary: {
    DEFAULT: '#BA1E2C',
    dark: '#DC0B2A',
  },
  // ... other colors
}
```

### Changing Fonts

Update the Google Fonts link in `public/index.html` and the font families in `tailwind.config.js`.

### Adding New Sections

1. Create a new component in `src/components/`
2. Import and add it to `App.js`
3. Add navigation link in `Header.jsx`

## License

This project is for personal/educational use.
