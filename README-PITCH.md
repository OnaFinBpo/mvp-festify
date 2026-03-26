# Festify Video Pitch - HTML Presentation

## Overview
Complete single-file HTML presentation for the Festify party planning platform. Vertical scrolling format with synchronized audio narration and auto-scroll transitions.

## File Details
- **Location**: `/sessions/laughing-busy-archimedes/mnt/Festa da Maitê/festify-video-pitch.html`
- **Size**: 5.3 MB (fully self-contained)
- **Format**: Single HTML file with all assets embedded as base64 data URIs
- **Browser Support**: Modern browsers (Chrome, Firefox, Safari, Edge)

## Key Features

### Content Structure (7 Sections)
1. **Section 0 - Gancho** (23.4s): The pain point - party planning chaos
2. **Section 1 - O Produto** (36.6s): Interactive invitations with 3 iPhone mockups
3. **Section 2 - Central de Gestão** (37.9s): Management dashboard with 2 iPhone mockups
4. **Section 3 - Integração** (28.0s): Supplier integration with 2 iPhone mockups
5. **Section 4 - Mercado** (32.1s): Market opportunity and competitive analysis
6. **Section 5 - Modelo de Negócio** (31.5s): Revenue streams with 2 iPhone mockups
7. **Section 6 - CTA** (64.7s): Call to action with login screen mockup

### Visual Design
- **Gradient Background**: Dark purple (#0F0524 to #1A0A3E)
- **Accent Colors**: Purple (#7C3AED), Pink (#EC4899), Amber (#F59E0B)
- **Typography**: Inter (body) + Playfair Display (headings) from Google Fonts
- **Layout**: Vertical scroll, max-width 800px, mobile responsive
- **iPhone Mockups**: CSS-only frames with rounded corners and notch

### Audio
- 7 MP3 audio tracks (one per section)
- Embedded as base64 data URIs
- Synced with section scrolling
- Auto-advances to next section when audio ends

### Controls
Fixed bottom control bar with:
- **Play/Pause**: Start/stop audio playback
- **Mute**: Toggle audio on/off
- **Progress Bar**: Visual indication of playback progress
- **Time Display**: Current time / Total duration
- **Speed Control**: 1x, 1.5x, 2x playback speeds
- **Keyboard Support**: Space bar to play/pause

### Screenshots Embedded (10 Total)
1. `01_convite_envelope` - Invitation envelope view
2. `02_convite_open` - Invitation opened
3. `03_convite_rsvp` - RSVP confirmation screen
4. `04_central_login` - Login screen
5. `05_dashboard` - Main dashboard
6. `06_dashboard_scroll` - Dashboard (alternate view)
7. `08_tarefas` - Task management
8. `09_orcamento` - Budget tracking
9. `10_convidados` - Guest list
10. `11_notas` - Notes section

## How to Use

### Opening the File
1. Double-click the HTML file to open in your default browser
2. Or drag the file into your browser window
3. Or use "Open File" from your browser (Ctrl+O / Cmd+O)

### Playback
1. Click anywhere on the splash screen to start
2. The first audio track will begin playing
3. The page automatically scrolls to match the audio narration
4. When audio ends, it automatically advances to the next section
5. Use the control bar to pause, adjust speed, or mute

### Manual Navigation
- Scroll manually at any time - the presentation continues to work
- Use play/pause button to control audio
- Adjust playback speed with the speed buttons
- Progress bar shows position in current section's audio

## Technical Details

### Embedded Assets
- **7 Audio Files**: Base64 encoded MP3s
- **10 Images**: Base64 encoded JPEGs
- **All Fonts**: Google Fonts (external CDN links)
- **No External Dependencies**: Except Google Fonts

### File Size Breakdown
- Images: ~2.8 MB
- Audio: ~2.2 MB
- HTML/CSS/JavaScript: ~0.3 MB

### Optimization
- Images optimized as JPEGs
- Audio at 128kbps quality
- Single file reduces HTTP requests
- Responsive design works on all screen sizes

## Browser Compatibility
- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Features

### IntersectionObserver
Automatically detects which section is visible for scroll-based navigation

### Smooth Scroll Behavior
CSS `scroll-behavior: smooth` for elegant transitions between sections

### Responsive Design
- Mobile: 220px iPhone frames, 70px control bar
- Desktop: 280px iPhone frames, 80px control bar
- Breakpoint: 600px width

## Notes

- All sections have `data-scene` attributes (0-6) for audio mapping
- Audio durations are defined in JavaScript for progress calculation
- Each section scrolls into view when its audio starts
- Manual scrolling doesn't interfere with audio playback
- Mobile-friendly vertical layout optimized for presentation on phone/tablet

## File Encoding
All files are embedded directly in the HTML using:
- `data:audio/mpeg;base64,` for MP3 audio
- `data:image/jpeg;base64,` for JPEG images

This makes the file completely self-contained and requires no external file access.
