# Film Strip Scroll Gallery

A single-page website featuring a horizontal film strip that scrolls as you scroll vertically. The design mimics a real 35mm Kodak film roll with photos displayed inside film frames.

## Features

- Horizontal film strip that moves as you scroll vertically
- Kodak film canister with film emerging from it
- Realistic film frame design with sprocket holes
- Frame numbers like real Kodak film (1, 1A, 2, 2A, etc.)
- Vintage/warm photo filter
- Hover effects on photos
- Progress bar indicator
- Smooth scroll animations
- Responsive design for mobile

## Files

- `index.html` - Main website (HTML/CSS/JS all-in-one)
- `film-roll.png` - Kodak 400 film canister image
- `film-frame.svg` - Repeating film strip segment with sprocket holes
- `film-end-frame.svg` - End cap of the film strip

## Usage

1. Open `index.html` in a web browser
2. Scroll down to see the film strip slide through
3. Photos move into the canister as you scroll

## Customization

### Adding Your Own Photos

Edit the `photos` array in the JavaScript section of `index.html`:

```javascript
const photos = [
    'path/to/photo1.jpg',
    'path/to/photo2.jpg',
    'path/to/photo3.jpg',
    // ... add more photos
];
```

Or use URLs:

```javascript
const photos = [
    'https://example.com/photo1.jpg',
    'https://example.com/photo2.jpg',
    // ...
];
```

### Changing Number of Frames

Update the `NUM_FRAMES` constant:

```javascript
const NUM_FRAMES = 12; // Change to desired number
```

### Adjusting Scroll Speed

Modify the `body` height in CSS (higher = slower scroll):

```css
body {
    height: 300vh; /* Increase for slower, decrease for faster */
}
```

### Changing Photo Filter

Edit the `.photo-slot img` CSS:

```css
.photo-slot img {
    filter: sepia(15%) saturate(110%) brightness(95%) contrast(105%);
}
```

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge).

## License

MIT
