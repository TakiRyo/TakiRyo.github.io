---
layout: about
title: about
permalink: /
subtitle: PhD Candidate, Nozaki Laboratory, Keio University

profile:
  align: right
  image: prof_pic.png
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Tokyo, Japan</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # news section disabled

latest_posts:
  enabled: false # blog section disabled
---

<strong>I build robots that reason about their surroundings with vision-language models and refine their actions through physical interaction.</strong>

I am a PhD candidate in Nozaki Laboratory at Keio University, working on **VLM-based manipulation**. My research uses vision-language models to reason about articulated objects — doors, drawers, and other mechanisms — and closes the loop with force feedback and physical trial-and-error, so a robot can adapt when its first guess is wrong.

<p style="margin-bottom:1.75rem;">
{% assign keywords = "VLM-Based Manipulation,Articulated Objects,Visual Reasoning,Force Control,3D Semantic SLAM,ROS2" | split: "," %}
{% for k in keywords %}<span style="display:inline-block;padding:.22em .75em;margin:.15em .3em .15em 0;border-radius:1em;border:1px solid rgba(127,127,127,.3);font-size:.75rem;line-height:1.7;white-space:nowrap;">{{ k }}</span>{% endfor %}
</p>

<!--
  No hero banner: the research focus images below carry the page. Sources for a hero,
  if one is ever wanted again, are kept out of the repo in assets/original/ (gitignored):
    video  - hero_door.mp4 (3.7MB, 5x speed; a burnt-in "x5" badge sits top-left, so a
             hero <video> needs object-position:50% 100% to crop it out of frame)
    still  - sips -c 950 2144 --cropOffset 300 700 assets/original/norman_door_after.png --out /tmp/h.png
             sips -Z 1600 -s format jpeg -s formatOptions 82 /tmp/h.png --out assets/img/hero_door.jpg
-->

## research focus

<div style="display:flex;flex-direction:column;gap:2.25rem;margin:1.25rem 0 2.75rem;">

  <div style="display:flex;flex-wrap:wrap;gap:1.75rem;align-items:center;">
    <div style="flex:1 1 250px;min-width:230px;">
      <img src="{{ '/assets/img/norman_door.jpg' | relative_url }}" alt="Robot arm gripping and turning a real door handle"
           style="width:100%;display:block;aspect-ratio:16/9;object-fit:cover;border-radius:8px;">
    </div>
    <div style="flex:1 1 290px;min-width:250px;">
      <h3 style="margin:0 0 .45rem;font-size:1.05rem;font-weight:600;line-height:1.35;">VLM-Based Manipulation of Articulated Objects</h3>
      <p style="margin:0 0 .55rem;font-size:.9rem;line-height:1.65;opacity:.8;">A vision-language model proposes how a mechanism should move; the robot tests that hypothesis against the real object and revises it from what it feels. One policy, many unseen doors, drawers, and hinges.</p>
      <p style="margin:0;font-size:.72rem;letter-spacing:.03em;text-transform:uppercase;opacity:.55;">JIASC 2026</p>
    </div>
  </div>

  <div style="display:flex;flex-wrap:wrap;gap:1.75rem;align-items:center;">
    <div style="flex:1 1 250px;min-width:230px;">
      <div style="display:flex;gap:2px;border-radius:8px;overflow:hidden;">
        <img src="{{ '/assets/img/geometric_map.jpg' | relative_url }}" alt="Geometric point-cloud reconstruction of a room"
             style="width:50%;display:block;aspect-ratio:1/1;object-fit:cover;">
        <img src="{{ '/assets/img/semantic_map.jpg' | relative_url }}" alt="The same room with every point semantically labelled"
             style="width:50%;display:block;aspect-ratio:1/1;object-fit:cover;">
      </div>
      <p style="margin:.4rem 0 0;font-size:.72rem;opacity:.6;">geometric reconstruction → semantic labels</p>
    </div>
    <div style="flex:1 1 290px;min-width:250px;">
      <h3 style="margin:0 0 .45rem;font-size:1.05rem;font-weight:600;line-height:1.35;">Robotic Perception &amp; 3D Semantic Mapping</h3>
      <p style="margin:0 0 .55rem;font-size:.9rem;line-height:1.65;opacity:.8;">Dense SLAM turns RGB-D video into a geometric reconstruction; confidence-weighted multi-view fusion then labels every point, so a mobile robot knows not just where surfaces are but what they are.</p>
      <p style="margin:0;font-size:.72rem;letter-spacing:.03em;text-transform:uppercase;opacity:.55;">AMC 2026 · ISIE 2026</p>
    </div>
  </div>

</div>

I am part of the [JEMARO](https://www.jemaro.eu/) program (Keio University & École Centrale de Nantes), an international double-degree program through which I work in an international research environment. I previously completed a workshop with [TIER IV Inc.](https://tier4.jp/), where I implemented planning modules of Autoware and developed a restart function for autonomous vehicles.
