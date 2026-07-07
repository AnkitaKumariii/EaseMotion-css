# Ease NFT Card Gallery

A modern, highly interactive 3D NFT card gallery with perspective tilt, staggered floating animations, and parallax layering. 

## What does this do?
This component creates a visually stunning gallery of NFT cards. The cards feature a continuous staggered floating animation. When a user hovers over a card, it smoothly transitions into a 3D perspective tilt (tracking an angled rotation), complete with neon glowing accents, depth-based parallax on the inner image and text, and glassmorphism styling. 

## How is it used?
Copy the `style.css` and the HTML structure from `demo.html` into your project.

### HTML Structure
Wrap your cards in the `.gallery-container`, and construct each card using `.nft-card`, `.nft-card-inner`, and the nested content elements:

```html
<div class="gallery-container">
  <div class="nft-card">
    <div class="nft-card-inner">
      <div class="nft-image nft-bg-1">
        <div class="nft-badge">Rare</div>
      </div>
      <div class="nft-details">
        <h3>Cosmic Wanderer #124</h3>
        <div class="nft-meta">
          <span class="nft-price">0.45 ETH</span>
          <span class="nft-time">Ending in 12h</span>
        </div>
      </div>
    </div>
  </div>
</div>
```

### Customization
You can easily tweak the component's appearance and behavior by modifying the CSS variables provided at the top of the stylesheet:

```css
:root {
  /* Core Variables */
  --nft-card-bg: rgba(255, 255, 255, 0.05);
  --nft-accent-color: #00ffcc;
  
  /* Dimensions & Spacing */
  --nft-card-width: 300px;
  --nft-card-height: 440px;
  
  /* Animation Settings */
  --nft-transition-speed: 0.5s;
  --nft-tilt-angle: 15deg;
  --nft-hover-lift: -15px;
}
```

## Why is it useful?
This component aligns perfectly with EaseMotion's philosophy of delivering premium, dynamic, and state-of-the-art interactive web experiences. 
It uses **pure CSS** (no JavaScript required for the 3D transforms or animations), making it extremely performant. It also leverages CSS `transform-style: preserve-3d` to create an actual z-axis separation between the card background and its contents, offering a true premium feel suited for Web3 platforms, crypto dashboards, and creative portfolios.
