---
layout: page
permalink: /thesis-supervision/
title: thesis supervision
description: Bachelor thesis topics, process, and available materials.
nav: false
nav_order: 7
google_sheet_embed:
---

This page lists current bachelor thesis topics, their status, and the supervision process.

## Available Topics

The list below is maintained directly on the website, so students can immediately see whether a topic is still available.

<div class="table-responsive thesis-table">
  <table class="table table-sm table-borderless">
    <thead>
      <tr>
        <th>Area</th>
        <th>Topic</th>
        <th>Status</th>
        <th>Notes</th>
      </tr>
    </thead>
    <tbody>
      {% for item in site.data.thesis_topics %}
        <tr>
          <td>{{ item.area }}</td>
          <td>{{ item.topic }}</td>
          <td>
            <span class="thesis-status thesis-status-{{ item.status | slugify }}">
              {{ item.status }}
            </span>
          </td>
          <td>{{ item.notes }}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

## Optional Sheet View

If you want to manage this externally, you can publish a Google Sheet and embed it here. Add the published embed URL to `google_sheet_embed` in this page.

{% if page.google_sheet_embed %}
  <div class="thesis-sheet">
    <iframe
      src="{{ page.google_sheet_embed }}"
      width="100%"
      height="520"
      frameborder="0"
      loading="lazy"
    ></iframe>
  </div>
{% endif %}

## Download

- [Bachelor thesis topics (CSV)](/assets/files/bachelor-thesis-topics.csv)

## What Students Should Prepare

- A short statement of interest
- Relevant methods or domain background
- A ranked list of preferred topics

## Process

1. Review the topic list.
2. Contact me by email with your ranked preferences.
3. We discuss fit, scope, and data availability.
4. We finalize the topic and timeline.

## How I Update This Page

- `open`: available
- `reserved`: currently discussed or assigned
- `completed`: no longer available / already done

To update a status, edit `_data/thesis_topics.yml`.
