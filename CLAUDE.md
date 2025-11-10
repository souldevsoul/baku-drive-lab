# BAKU DRIVE LAB - Brand Identity & Implementation Guide

## Brand Overview
**Market:** Azerbaijan - Performance/Tuning Culture
**Tone:** Performance / Tuning / Lab Research
**Positioning:** Technical performance lab for modified cars and tuning enthusiasts in Azerbaijan

## Brand Identity

### Color Palette
- **Primary:** Cyber Blue `#00D9FF`
- **Secondary:** Steel `#8B95A5`
- **Accent:** Black `#0A0A0A`
- **Background:** Dark Steel `#1A1F2E`
- **Surface:** Deep Blue Black `#0F1419`
- **Neon Accent:** Electric Blue `#00FFFF`

### Typography
- **Headlines:** Inter (Black, Extra Bold)
- **Body:** Inter (Regular, Medium)
- **Code/Lab:** Space Mono (for technical specs, dyno numbers)
- **Azeri:** Inter (supports Azeri Latin)

### Visual Style
- Cyber blue neon aesthetic
- Motion streak performance photography
- Lab research environment
- Performance tuning culture
- Dynamic, animated
- Tech-forward, futuristic
- Baku Flame Towers cyber context

## Image Generation Prompts

### Hero Image Prompt
```
"Performance coupe frozen motion shot at night with cyber blue neon lab motion streaks, medium format Phase One IQ4 modern high detail editorial, Zeiss Supreme crisp microcontrast, no branding, no plates, no text, subtle Flame Towers silhouette hint, cinematic 16:9."
```

### Report Card Image Prompt
```
"Top-down performance coupe on dark surface with cyber blue neon grid overlay, motion blur streaks, technical lab aesthetic, dark background with electric blue accents, suitable for 1200×800."
```

### Landing Page Banner Prompt
```
"Abstract motion streaks in cyber blue (#00D9FF) on dark background, performance energy, technical grid overlay, sized for 1920×400."
```

### Global Negative Prompt
```
"no logos, no license plates, no people, no cartoon style, no toy plastic look, no unrealistic CG lighting, no text overlays, no watermark"
```

## Design Modifications from Boxcar Base

### Layout Changes
1. **Dynamic motion** - animated hero sections
2. **Cyber blue neon accents** throughout
3. **Grid overlays** - technical/lab aesthetic
4. **Motion blur effects** - performance energy
5. **Dark theme** - futuristic lab environment
6. **Animated elements** - more dynamic than other brands

### Component Adjustments
- **Cards:** Dark with neon blue borders, subtle glow
- **Buttons:** Cyber blue with glow effects on hover
- **Forms:** Futuristic with neon focus states
- **Hero:** Motion streaks, animated background
- **Icons:** Outlined style with neon glow
- **Badges:** Performance stats (HP, 0-100, etc.)
- **Charts:** Dyno curves, performance graphs

### Cyber Theme
```css
:root {
  --cyber-blue: #00D9FF;
  --steel: #8B95A5;
  --black: #0A0A0A;
  --bg-dark: #1A1F2E;
  --surface: #0F1419;
  --neon: #00FFFF;
  --glow: rgba(0, 217, 255, 0.5);
}
```

### Neon Glow Effect
```css
.neon-glow {
  box-shadow: 0 0 10px rgba(0, 217, 255, 0.5),
              0 0 20px rgba(0, 217, 255, 0.3),
              0 0 30px rgba(0, 217, 255, 0.1);
}

.neon-text {
  text-shadow: 0 0 10px rgba(0, 217, 255, 0.8),
               0 0 20px rgba(0, 217, 255, 0.5);
}
```

## Content Tone & Copy

### Messaging (Azeri - Latin)
- "Baku Performance Lab"
- "Texniki Performans Analizi"
- "Tuning və Modifikasiya Ekspertizası"

### Messaging (Russian)
- "Лаборатория Производительности Баку"
- "Технический Анализ Производительности"

### Messaging (English)
- "Performance Engineering Lab"
- "Technical Tuning Analysis"
- "Modified Vehicle Assessment"
- "Dyno-Verified Reports"

### Voice Guidelines
- Technical, precise language
- Performance enthusiast tone
- Lab/research terminology
- Data-driven statements
- Tuning community language
- Horsepower, torque, 0-100 times
- Mod-friendly, enthusiast-focused

### Terminology Focus
- HP/kW (power)
- Nm (torque)
- 0-100 km/h times
- Quarter mile times
- Dyno runs
- ECU tunes
- Modifications list
- Performance parts

## Core Functionality

### Request Flow (Performance Focus)
1. User pastes link OR submits modified car details
2. System detects modifications, performance specs
3. Extract: base HP, claimed mods, performance claims
4. Perplexity search: aftermarket parts verification
5. Performance analysis: realistic HP gains, safety
6. Pricing accounts for mods (positive/negative value)
7. Report includes: dyno estimates, mod verification, safety concerns

### Supported Platforms (Azerbaijan)
- Turbo.az (performance section)
- Tap.az (tuned cars)
- Private tuner networks
- Performance shops
- Import tuner listings

### Special Features
- **Mod Detection:** Identify aftermarket parts from photos/description
- **Dyno Estimates:** Predict realistic HP/torque
- **Safety Warnings:** Flag dangerous mods
- **Parts Verification:** Check if claimed parts are genuine
- **Performance Comps:** Compare to stock & modified examples
- **Tuning Potential:** Suggest safe upgrade paths

### Pricing (AZN) - Performance Premium
- **Remote Assessment:** 59 AZN (standard) / 99 AZN (24h)
- **On-Site + Dyno Coordination:** 299 AZN (includes dyno shop visit)
- **Mod Verification:** 149 AZN (detailed parts check)
- **Pre-Tune Consultation:** 199 AZN (upgrade planning)
- **Deposit:** 20% of max bid

## Technical Implementation Priorities

### Phase 1 - Cyber Brand Identity
- [ ] Dark theme with cyber blue accents
- [ ] Implement neon glow effects
- [ ] Create motion streak backgrounds
- [ ] Add animated elements
- [ ] Generate neon performance imagery
- [ ] Design lab-style logo
- [ ] Create technical grid overlays

### Phase 2 - Performance UI
- [ ] Animated hero with motion blur
- [ ] Dyno curve visualizations (Chart.js)
- [ ] Performance stat cards (HP, torque, 0-100)
- [ ] Mod checklist components
- [ ] Parts verification interface
- [ ] Technical spec tables

### Phase 3 - Tuning Content
- [ ] Write performance-focused copy (AZ/RU/EN)
- [ ] Create mod detection guides
- [ ] Build safety warning system
- [ ] Performance terminology glossary
- [ ] Tuner community language

### Phase 4 - Performance Features
- [ ] Mod detection AI (OpenAI vision)
- [ ] Dyno estimate calculator
- [ ] Parts database (common mods)
- [ ] Performance comps (modified cars)
- [ ] Safety flag system
- [ ] Tuning potential analyzer

### Phase 5 - Community Features
- [ ] Tuner shop directory (Baku)
- [ ] Dyno shop integrations
- [ ] Performance parts suppliers
- [ ] Mod showcase gallery
- [ ] Community forum (future)

## File Structure Priority

```
baku-drive-lab/
├── app/
│   ├── [locale]/          # AZ/RU/EN
│   │   ├── layout.js      # Dark cyber theme
│   │   ├── page.js        # Motion hero
│   │   └── ...
│   ├── globals.css        # Cyber blue + dark theme
│   └── ...
├── components/
│   ├── performance/
│   │   ├── DynoChart.js
│   │   ├── ModChecklist.js
│   │   ├── PerformanceStats.js
│   │   └── MotionHero.js
│   ├── cyber/
│   │   ├── NeonGlow.js
│   │   ├── GridOverlay.js
│   │   └── MotionStreak.js
│   └── ...
├── public/
│   ├── images/
│   │   ├── hero-performance-night.jpg
│   │   ├── flame-towers-neon.jpg
│   │   ├── motion-streaks.png
│   │   └── lab-logo.svg
│   ├── data/
│   │   └── common-mods.json    # Turbo kits, exhausts, etc.
│   └── locales/
│       ├── az.json
│       ├── ru.json
│       └── en.json
└── ...
```

## Mod Detection System

### Common Modifications to Detect
- **Engine:** Turbo/supercharger, intercooler, intake, exhaust, ECU tune
- **Suspension:** Coilovers, sway bars, camber kits, air ride
- **Brakes:** Big brake kits, upgraded rotors, performance pads
- **Exterior:** Body kits, spoilers, diffusers, widebody
- **Wheels:** Aftermarket wheels, tire sizes
- **Interior:** Racing seats, harnesses, roll cage, gauges

### Detection Methods
1. **Text parsing:** Search description for mod keywords (AZ/RU/EN)
2. **Image analysis:** OpenAI vision to spot visual mods
3. **Spec comparison:** Compare claimed HP to stock
4. **Price signals:** Higher price = likely modified
5. **Seller type:** Tuning shops = modified cars

### Safety Flags
- ⚠️ No tune with turbo (dangerous)
- ⚠️ Cheap eBay turbo (reliability risk)
- ⚠️ Extreme camber (safety issue)
- ⚠️ No supporting mods (incomplete build)
- ⚠️ Mismatched tire sizes
- ⚠️ Claimed HP unrealistic

## Performance Report Sections

### 1. Stock Baseline
- Factory HP/torque
- Stock 0-100 time
- Factory specs

### 2. Claimed Modifications
- List from ad (parsed)
- Photos showing mods
- Seller's HP claims

### 3. Verification Analysis
- Mod authenticity check
- Realistic HP estimate
- Safety concerns
- Missing components

### 4. Market Value Impact
- Positive mods (quality, bolt-on)
- Negative mods (cheap, incomplete, dangerous)
- Net effect on value

### 5. Recommendations
- Safe max bid (accounting for mods)
- Pre-purchase inspection focus
- Dyno verification advice
- Upgrade potential

## Animations & Motion

### Hero Animation
- Motion blur streaks (CSS)
- Particles.js background (cyber blue)
- Animated specs counter (HP, torque counting up)
- Parallax scroll effect

### Micro-interactions
- Neon glow on hover
- Button pulse effects
- Stat counters (performance numbers)
- Progress bars (HP gains)
- Smooth transitions (400ms)

### Performance (60fps)
- Use CSS transforms (not position)
- GPU acceleration
- Debounce scroll events
- Lazy load heavy animations
- Reduced motion support

## Multi-Language (AZ/RU/EN)

### Priority
1. **Azeri** - Primary (Latin script)
2. **Russian** - Secondary (tuning community)
3. **English** - Tertiary (expats, international)

### Tuning Terminology
- Keep some English terms (HP, dyno, ECU, etc.)
- Translate explanations
- Use tuner slang where appropriate
- Test with actual tuners/enthusiasts

## Next Steps
1. Install dependencies (Framer Motion, Chart.js)
2. Implement dark cyber theme
3. Create neon glow components
4. Generate motion streak imagery
5. Build dyno chart components
6. Create mod detection system
7. Write performance-focused copy
8. Test with tuning community
9. Set up performance parts database
10. Deploy with dark theme

## Resources
- Fonts: Inter (all weights), Space Mono
- Animations: Framer Motion, Particles.js
- Charts: Chart.js (for dyno curves)
- Icons: Lucide React (outlined style)
- Image Generation: Neon cyber motion prompts
- Mod Database: JSON file with common parts
- Community: Baku tuner shops, forums

## Differentiation

| Aspect | BAKU DRIVE LAB | AVTOCERT |
|--------|----------------|----------|
| Audience | Tuners, enthusiasts | General public |
| Focus | Performance, mods | Standard vehicles |
| Tone | Cyber, technical | Official, simple |
| Features | Mod detection, dyno | Basic assessment |
| Price | Premium (59 AZN+) | Affordable (39 AZN+) |
| Style | Dark, neon, motion | Bright, clean, simple |
| Language | Tuner slang | Simple, clear |

**BAKU DRIVE LAB = For the tuning community, by the tuning community.**

## Baku Performance Culture

### Local Context
- Growing tuning scene in Baku
- Popular cars: BMW, Mercedes, JDM imports
- Limited dyno shops (coordinate visits)
- Import parts from Turkey, Russia, China
- Mix of quality builds and cheap mods
- Need for verification (many fake claims)

### Trust Building
- Showcase local dyno partnerships
- Feature real Baku tuned cars
- Partner with reputable shops
- Community testimonials
- Before/after examples
- Transparent mod verification

**Serve the enthusiasts, protect the community.**
