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

{{< list title="## Made at *Home*" cardView=true limit=6 where="Params.genre" value="project_perso" >}}

{{< list title="## Made for [*TIM*](https://www.timupsinsa.com/) " cardView=true limit=6 where="Params.genre" value="project_tim" >}}

{{< list title="## Made at [*University*](https://www.univ-tlse3.fr/decouvrir-nos-diplomes/master-parcours-systemes-et-microsystemes-embarques-sme)" cardView=true limit=6 where="Params.genre" value="project_school" >}}

{{< list title="## Made for [*Eurêkafé*](https://eurekafe.fr)" cardView=true limit=6 where="Params.genre" value="project_work" >}}