---
layout: archive
title: "dev"
permalink: /dev/
author_profile: true
---

{% include base_path %}

<html>
<style>

@import 'compass/css3';

.body {
  --l: calc(100vw/var(--n-cols));
  --hl: calc(.5*var(--l));
  --ri: calc(.5*#{sqrt(3)}*var(--l));
  box-sizing: border-box;
  display: grid;
  place-content: center;
  grid-template: repeat(var(--n-rows), var(--l))/ repeat(var(--n-cols), var(--ri));
  grid-gap: var(--hl) 0;
  overflow: hidden;
  margin: 0;
  padding: var(--hl) 0;
  height: 100vh;
  background: #262626;
  filter: drop-shadow(2px 2px 5px);
  
  @media (orientation: landscape) { --l: calc(100vh/(var(--n-rows) + 3)) }
}

.hex-cell {
  overflow: hidden;
  grid-column-end: span 2;
  margin: calc(-1*var(--hl)) 0;
  transform: scale(.95);
  clip-path: polygon(50% 0, 100% 25%, 100% 75%, 50% 100%, 0 75%, 0 25%)
}

.img {
  --hl: 0;
  width: 100%; height: 100%;
  object-fit: cover;
  transform: scale(calc(1 + .2*var(--hl)));
  filter: brightness(calc(.6*(1 + var(--hl))));
  transition: .7s;
  
  &:hover { --hl: 1 }
}

</style>

<body>

- let imgs = [
-   'https://images.unsplash.com/photo-1519681393784-d120267933ba?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1497733942558-e74c87ef89db?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1540744276164-9dc898353c7b?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1469975692758-66d107a536cb?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1490845060161-85f9ce08a9f4?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1541673504494-8bcc1a340180?w=650&fm=jpg', 
-   'https://images.unsplash.com/photo-1515937350506-3e7b51a95339?w=650&fm=jpg'
- ];

- let n_cols_max = n_cols_min + 1, n_cols_sum = n_cols_max + n_cols_min;
- let n = Math.ceil(.5*n_rows)*n_cols_min + Math.floor(.5*n_rows)*n_cols_max;
- let ni = imgs.length;

body(style=`--n-rows: ${n_rows}; --n-cols: ${2*n_cols_max}`)
  style .hex-cell:nth-of-type(#{n_cols_sum}n + 1) { grid-column-start: 2 }
  - for(let i = 0; i < n; i++)
    .hex-cell: img(src=imgs[i%ni])
</body>

</html>

