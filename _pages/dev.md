---
layout: archive
title: "nothing to see here..."
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
  <div class="hex-cell">
    <a target="_blank" href="../images/gallery/cira-rammb-slider - -goes-17 - -full_disk - -geocolor-opacity-100 - -20201119151031-20201119220031.gif">
      <img src="../images/gallery/cira-rammb-slider - -goes-17 - -full_disk - -geocolor-opacity-100 - -20201119151031-20201119220031.gif" alt="vortex_street_gif">
    </a>
     <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png">
      <img src="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png" alt="vortex_street_gif">
    </a>
  </div>
  <div class="hex-cell">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png">
      <img src="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png" alt="vortex_street_gif">
    </a>
  </div>
</body>

</html>

