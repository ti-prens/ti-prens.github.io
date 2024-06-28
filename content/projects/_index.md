---
title: "My Projects"
type: "page"
date: 2020-08-14
layout: "simple"
type : "page"
---

{{< lead >}}
Projects that I contributed to.
Those I can share.😉
{{< /lead >}}

<!-- {{< carousel images="{https://i.ibb.co/twRyF6S/Add-a-heading.png}"  >}}   -->
<!-- {{< carousel images="{https://i.ibb.co/V3XN84p/Click.png}"  >}}   -->
<!-- FOR SOME REASON IF I DO NOT USE CAROUSEL IMAGE BEFORE CAROUSEL PAGES THE LOGIC (THE BUTTONS AND THE TIME BASED CYCLE ) DO NOT WORK -->

{{< list title="## Made for [TIM](https://www.timupsinsa.com/) " cardView=true limit=6 where="Params.genre" value="project_tim" >}}


{{< list title="## Made for school" cardView=true limit=6 where="Params.genre" value="project_school" >}}



{{< list title="## Made for **work**" cardView=true limit=6 where="Params.genre" value="project_work" >}}

{{< list title="## Made for fun" cardView=true limit=6 where="Params.genre" value="project_perso" >}}