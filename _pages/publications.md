---
layout: page
permalink: /research/
title: research
description: Journal publications, work in progress, book chapters, and presentations.
nav: true
nav_order: 2
---

{% include bib_search.liquid %}

<div class="publications">

  <h2>Refereed Journal Publications</h2>
  {% bibliography --query @*[section=journal]* %}

  <h2>Work in Progress</h2>
  {% bibliography --query @*[section=wip]* %}

  <h2>Book Chapters and Conference Papers</h2>
  {% bibliography --query @*[section=bookchapter]* %}

  <h2>Conference Presentations</h2>
  <ul class="card-text font-weight-light list-group list-group-flush">
    <li class="list-group-item">
      <strong>Pacing in Real-Time Bidding for Online Display Advertising</strong><br>
      7th European Marketing Academy (EMAC) Job Market Simulation, Madrid, Spain, 2025.<br>
      European Marketing Academy (EMAC) Doctoral Colloquium, Madrid, Spain, 2025.<br>
      Digital Economy Workshop, Berlin, 2025.<br>
      Hi! Paris Summer School 2023 on AI & Data for Science, Paris, France, 2023. Best Poster Award.<br>
      19th Symposium on Statistical Challenges in Electronic Commerce Research (SCECR), Bogotá, Colombia, 2023.<br>
      Marketing Dynamics Conference, Atlanta, USA, 2022.<br>
      Proceedings of the 44th INFORMS Marketing Science Conference, virtual, 2022.<br>
      Proceedings of the 51st Conference of the European Marketing Academy (EMAC), Budapest, Hungary, 2022.
    </li>
    <li class="list-group-item">
      <strong>Finding the Right Pace: A New Pacing Heuristic for Real-Time Bidding</strong><br>
      20th Annual Symposium on Statistical Challenges in Electronic Commerce Research (SCECR), Lisbon, Portugal, 2024.<br>
      46th INFORMS Society for Marketing Science (ISMS) Marketing Science Conference, Sydney, Australia, 2024.
    </li>
    <li class="list-group-item">
      <strong>Privacy-Friendly Targeting: Is Context Enough to Replace Behavior?</strong><br>
      47th INFORMS Society for Marketing Science (ISMS) Marketing Science Conference, Washington, D.C., USA, 2025.<br>
      21st Symposium on Statistical Challenges in Electronic Commerce Research (SCECR), Paphos, Cyprus, 2025.
    </li>
  </ul>

  <h2>Invited Presentations</h2>
  <ul class="card-text font-weight-light list-group list-group-flush">
    <li class="list-group-item">
      <strong>Pacing in Real-Time Bidding for Online Display Advertising</strong><br>
      Seminar Series at Google, Paris, 2023.<br>
      Seminar Series at Zalando, Berlin, 2024.
    </li>
  </ul>

</div>
