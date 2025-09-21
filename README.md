# ashlies floral creations website

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ashlie's Floral Creations - Eternal & Natural Floral Arrangements</title>
<style>
* {
margin: 0;
padding: 0;
box-sizing: border-box;
}

```
body {
font-family: 'Georgia', serif;
line-height: 1.6;
color: #333;
overflow-x: hidden;
}

.hero {
background: linear-gradient(135deg, #fdf2f8 0%, #fce7f3 50%, #f9a8d4 100%);
min-height: 100vh;
display: flex;
align-items: center;
position: relative;
padding: 2rem;
}

.hero::before {
content: '';
position: absolute;
top: 0;
left: 0;
right: 0;
bottom: 0;
background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="%23ffffff20"/><circle cx="80" cy="40" r="1.5" fill="%23ffffff30"/><circle cx="40" cy="80" r="1" fill="%23ffffff20"/><circle cx="70" cy="15" r="1" fill="%23ffffff25"/><circle cx="15" cy="60" r="1.5" fill="%23ffffff20"/></svg>') repeat;
animation: float 20s infinite linear;
}

@keyframes float {
0% { transform: translateY(0px) translateX(0px); }
33% { transform: translateY(-10px) translateX(5px); }
66% { transform: translateY(5px) translateX(-5px); }
100% { transform: translateY(0px) translateX(0px); }
}

.hero-content {
max-width: 1200px;
margin: 0 auto;
display: grid;
grid-template-columns: 1fr 1fr;
gap: 4rem;
align-items: center;
position: relative;
z-index: 2;
}

.hero-text h1 {
font-size: 4rem;
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
margin-bottom: 1rem;
text-shadow: none;
font-style: italic;
}

.hero-text h2 {
font-size: 1.5rem;
color: #be185d;
margin-bottom: 2rem;
font-weight: normal;
}

.hero-gallery {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 1rem;
transform: perspective(1000px) rotateY(-5deg);
}

.gallery-item {
background: linear-gradient(135deg, #fff7ed, #fef3c7);
border-radius: 20px;
padding: 1rem;
box-shadow: 0 10px 30px rgba(217, 70, 239, 0.2);
transform: translateZ(50px);
transition: all 0.3s ease;
aspect-ratio: 1;
display: flex;
align-items: center;
justify-content: center;
position: relative;
overflow: hidden;
border: 2px solid #f59e0b;
}

.gallery-item:hover {
transform: translateZ(80px) scale(1.05);
box-shadow: 0 20px 40px rgba(217, 70, 239, 0.3);
}

.gallery-item::before {
content: '🌸';
font-size: 4rem;
opacity: 0.1;
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
}

.gallery-text {
text-align: center;
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
font-weight: bold;
z-index: 2;
position: relative;
}

.cta-button {
display: inline-block;
background: linear-gradient(45deg, #d946ef, #f59e0b);
color: white;
padding: 1rem 2rem;
text-decoration: none;
border-radius: 50px;
font-weight: bold;
margin-top: 2rem;
transition: all 0.3s ease;
box-shadow: 0 5px 15px rgba(217, 70, 239, 0.3);
}

.cta-button:hover {
transform: translateY(-3px);
box-shadow: 0 10px 25px rgba(217, 70, 239, 0.4);
}

.services {
background: white;
padding: 5rem 2rem;
}

.services-container {
max-width: 1200px;
margin: 0 auto;
}

.services h2 {
text-align: center;
font-size: 3rem;
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
margin-bottom: 3rem;
font-style: italic;
}

.services-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
gap: 2rem;
margin-bottom: 3rem;
}

.service-card {
background: linear-gradient(135deg, #fdf2f8, #fef3c7);
padding: 2rem;
border-radius: 20px;
text-align: center;
transition: all 0.3s ease;
border: 2px solid #f59e0b;
position: relative;
overflow: hidden;
}

.service-card::before {
content: '';
position: absolute;
top: -50%;
left: -50%;
width: 200%;
height: 200%;
background: linear-gradient(45deg, transparent, rgba(217, 70, 239, 0.1), transparent);
transform: rotate(45deg);
transition: all 0.5s ease;
opacity: 0;
}

.service-card:hover::before {
opacity: 1;
animation: shimmer 1.5s ease-in-out;
}

@keyframes shimmer {
0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
}

.service-card:hover {
transform: translateY(-10px);
border-color: #d946ef;
box-shadow: 0 15px 35px rgba(217, 70, 239, 0.2);
}

.service-icon {
font-size: 4rem;
margin-bottom: 1rem;
}

.service-card h3 {
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
margin-bottom: 1rem;
font-size: 1.5rem;
}

.service-card p {
color: #666;
line-height: 1.6;
}

.portfolio {
background: linear-gradient(135deg, #fff1f2, #fef7cd);
padding: 5rem 2rem;
}

.portfolio-container {
max-width: 1200px;
margin: 0 auto;
}

.portfolio h2 {
text-align: center;
font-size: 3rem;
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
margin-bottom: 1rem;
font-style: italic;
}

.portfolio-subtitle {
text-align: center;
font-size: 1.2rem;
color: #be185d;
margin-bottom: 3rem;
font-style: italic;
}

.portfolio-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
gap: 2rem;
margin-bottom: 3rem;
}

.portfolio-item {
background: white;
border-radius: 20px;
overflow: hidden;
box-shadow: 0 10px 30px rgba(217, 70, 239, 0.15);
transition: all 0.3s ease;
border: 2px solid #f59e0b;
}

.portfolio-item:hover {
transform: translateY(-10px);
box-shadow: 0 20px 40px rgba(217, 70, 239, 0.25);
}

.portfolio-image {
height: 250px;
background: linear-gradient(135deg, #fdf2f8, #fef3c7);
display: flex;
align-items: center;
justify-content: center;
position: relative;
overflow: hidden;
}

.placeholder-content {
text-align: center;
color: #be185d;
}

.portfolio-icon {
font-size: 4rem;
display: block;
margin-bottom: 0.5rem;
}

.portfolio-image p {
font-weight: bold;
font-size: 1.1rem;
}

.portfolio-info {
padding: 1.5rem;
}

.portfolio-info h4 {
background: linear-gradient(45deg, #d946ef, #f59e0b);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
font-size: 1.3rem;
margin-bottom: 0.5rem;
}

.portfolio-info p {
color: #666;
line-height: 1.5;
}

.portfolio-note {
text-align: center;
background: rgba(217, 70, 239, 0.1);
padding: 2rem;
border-radius: 15px;
border: 2px dashed #d946ef;
margin-top: 2rem;
}

.portfolio-note p {
color: #be185d;
font-size: 1.1rem;
margin: 0;
}
background: linear-gradient(135deg, #d946ef, #f59e0b);
color: white;
padding: 5rem 2rem;
text-align: center;
}

.contact-container {
max-width: 800px;
margin: 0 auto;
}

.contact h2 {
font-size: 3rem;
margin-bottom: 2rem;
font-style: italic;
}

.contact-info {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
gap: 2rem;
margin-bottom: 3rem;
}

.contact-item {
background: rgba(255, 255, 255, 0.1);
padding: 2rem;
border-radius: 15px;
backdrop-filter: blur(10px);
border: 1px solid rgba(255, 255, 255, 0.2);
transition: all 0.3s ease;
}

.contact-item:hover {
background: rgba(255, 255, 255, 0.2);
transform: scale(1.05);
}

.contact-item h3 {
font-size: 1.2rem;
margin-bottom: 0.5rem;
}

.contact-item p {
font-size: 1.1rem;
}

.notice {
background: rgba(255, 255, 255, 0.2);
padding: 2rem;
border-radius: 15px;
backdrop-filter: blur(10px);
border: 1px solid rgba(255, 255, 255, 0.3);
margin-top: 2rem;
}

.notice h3 {
margin-bottom: 1rem;
font-size: 1.5rem;
}

.footer {
background: #881337;
color: white;
text-align: center;
padding: 2rem;
}

@media (max-width: 768px) {
.portfolio-grid {
grid-template-columns: 1fr;
}
}
.hero-content {
grid-template-columns: 1fr;
text-align: center;
}

.hero-text h1 {
font-size: 2.5rem;
}

.hero-gallery {
transform: none;
margin-top: 2rem;
}

.services-grid {
grid-template-columns: 1fr;
}

.contact-info {
grid-template-columns: 1fr;
}
}
</style>
```

</head>
<body>
<section class="hero">
<div class="hero-content">
<div class="hero-text">
<h1>Ashlie's Floral Creations</h1>
<h2>Specializing in Eternal & Natural Floral Arrangements</h2>
<p>Creating beautiful, personalized bouquets that capture your special moments and last for years to come.</p>
<a href="#portfolio" class="cta-button">View Our Work</a>
</div>
<div class="hero-gallery">
<div class="gallery-item">
<div class="gallery-text">Eternal Flowers<br><small>Last for Years</small></div>
</div>
<div class="gallery-item">
<div class="gallery-text">Custom Bouquets<br><small>All Occasions</small></div>
</div>
<div class="gallery-item">
<div class="gallery-text">Natural Flowers<br><small>Fresh & Beautiful</small></div>
</div>
<div class="gallery-item">
<div class="gallery-text">Personal Gifts<br><small>Add Plushies</small></div>
</div>
</div>
</div>
</section>

```
<section class="services">
<div class="services-container">
<h2>Our Services</h2>
<div class="services-grid">
<div class="service-card">
<div class="service-icon">💐</div>
<h3>Personalized Bouquets</h3>
<p>Custom designed floral arrangements for all your special occasions - weddings, anniversaries, graduations, and more. Each bouquet is crafted with love and attention to detail.</p>
</div>
<div class="service-card">
<div class="service-icon">✨</div>
<h3>Eternal Flowers</h3>
<p>Our signature eternal flowers are specially treated to maintain their beauty for years. Perfect for preserving memories of your most precious moments.</p>
</div>
<div class="service-card">
<div class="service-icon">🌸</div>
<h3>Natural Fresh Flowers</h3>
<p>Beautiful, fresh natural flowers sourced from the finest growers. Available for those who prefer the classic beauty of traditional floral arrangements.</p>
</div>
<div class="service-card">
<div class="service-icon">🎁</div>
<h3>Custom Orders & Gifts</h3>
<p>Make your arrangement extra special by adding plushies or other personal gifts. We work with you to create the perfect custom order for your needs.</p>
</div>
</div>
</div>
</section>

<section class="portfolio" id="portfolio">
<div class="portfolio-container">
<h2>Our Beautiful Creations</h2>
<p class="portfolio-subtitle">See some of our recent floral designs and custom arrangements</p>

<div class="portfolio-grid">
<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">🌸</span>
<p>Eternal Rose Bouquet</p>
</div>
</div>
<div class="portfolio-info">
<h4>Blue Eternal Roses</h4>
<p>Custom arrangement with blue preserved roses</p>
</div>
</div>

<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">💐</span>
<p>Sunflower Arrangement</p>
</div>
</div>
<div class="portfolio-info">
<h4>Sunflower & Roses</h4>
<p>Bright yellow sunflowers with elegant wrapping</p>
</div>
</div>

<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">🌹</span>
<p>Heart Arrangement</p>
</div>
</div>
<div class="portfolio-info">
<h4>Heart Shape Design</h4>
<p>Romantic heart-shaped floral arrangement</p>
</div>
</div>

<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">🧸</span>
<p>Gift Set</p>
</div>
</div>
<div class="portfolio-info">
<h4>Flowers & Plushie</h4>
<p>Custom bouquet with adorable plushie gift</p>
</div>
</div>

<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">🌺</span>
<p>Mixed Bouquet</p>
</div>
</div>
<div class="portfolio-info">
<h4>Colorful Mix</h4>
<p>Vibrant multi-colored rose arrangement</p>
</div>
</div>

<div class="portfolio-item">
<div class="portfolio-image">
<div class="placeholder-content">
<span class="portfolio-icon">❄️</span>
<p>Special Occasion</p>
</div>
</div>
<div class="portfolio-info">
<h4>Winter Theme</h4>
<p>Elegant white and blue themed arrangement</p>
</div>
</div>
</div>

<div class="portfolio-note">
<p><strong>Want to add your photo here?</strong> Simply replace the placeholder images with photos of your actual floral creations!</p>
</div>
</div>
</section>

<section class="contact" id="contact">
<div class="contact-container">
<h2>Get in Touch</h2>
<p>Ready to create something beautiful? Contact us to discuss your floral needs.</p>
<div class="contact-info">
<div class="contact-item">
<h3>📞 Phone</h3>
<p>(703) 867-4023</p>
<div class="contact-item">
<h3>📧 Email</h3>
<p>aediaz504@gmail.com</p>
</div>
<div class="notice">
<h3>⏰ Important Notice</h3>
<p>Please place orders at least 4-7 days in advance to ensure we can create the perfect arrangement for your special occasion.</p>
</div>
</div>
</section>

<footer class="footer">
<p>&copy; 2024 Ashlie's Floral Creations. All rights reserved. | Specializing in Eternal & Natural Floral Arrangements</p>
</footer>

<script>
// Smooth scrolling for navigation links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
anchor.addEventListener('click', function (e) {
e.preventDefault();
document.querySelector(this.getAttribute('href')).scrollIntoView({
behavior: 'smooth'
});
});
});

// Add scroll animation for service cards
const observerOptions = {
threshold: 0.1,
rootMargin: '0px 0px -50px 0px'
};

const observer = new IntersectionObserver(function(entries) {
entries.forEach(entry => {
if (entry.isIntersecting) {
entry.target.style.animation = 'slideInUp 0.6s ease forwards';
}
});
}, observerOptions);

document.querySelectorAll('.service-card').forEach(card => {
observer.observe(card);
});

// Add CSS for slide in animation
const style = document.createElement('style');
style.textContent = `
@keyframes slideInUp {
from {
opacity: 0;
transform: translateY(30px);
}
to {
opacity: 1;
transform: translateY(0);
}
}

.service-card {
opacity: 0;
transform: translateY(30px);
}
`;
document.head.appendChild(style);
</script>
```

</body>
</html>
