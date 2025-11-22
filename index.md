---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">

<div class="home-container">
  <h1 class="site-title">{{ site.title }}</h1>
  
  <div class="image-container">
    <p class="image-placeholder">Image placeholder - Add your image here</p>
    <!-- Replace the above line with: <img src="{{ '/assets/images/your-image.jpg' | relative_url }}" alt="Site Image"> -->
  </div>
  
  <p class="site-description">{{ site.description }}</p>
</div>

