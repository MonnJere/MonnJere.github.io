---
layout: page
title:       "Jewel – Unified Calendar & Life‑Organizer"
categories:  [projects]
date:        2025-05-10
permalink:   /projects/jewel/
header:
  title: Cross-Platform Calendar App
  image_fullwidth: jewel_banner.png
image: 
  thumb: /images/PJ-Icon_thumb.png
tags:        [Flutter, Dart, Firebase, Calendar]
---

*Jewel* is a **cross‑platform calendar app** (Web + Android + iOS) that merges Google Calendar, iCal feeds, and custom calendars into a single smart agenda with built-in commute planning and personal goal tracking.

---

## Problem

> "Why can't I see all my events in one place and know if I have enough time to get from one meeting to another?"

Modern life requires juggling multiple calendars across work, school and personal accounts. Adding travel time calculations manually leads to poor scheduling decisions and missed appointments.

---

## Solution at a glance

| Feature | How Jewel fixes it |
|---------|-------------------|
| **Multi‑calendar integration** | OAuth flows pull Google Calendar data plus iCal feed support for external calendars. |
| **Calendar conversion** | Seamlessly convert external iCal events to fully-editable Google Calendar events. |
| **Smart commute calculation** | Uses Google Maps API to calculate travel times between event locations. |
| **Personal goals system** | Create, track and analyze goals across multiple categories (Health, Work, Education, Finance, etc.). |
| **Group calendar coordination** | Share schedules with user groups for team planning with color-coded member events. |
| **Background event monitoring** | Automated background tasks check for conflicting events and insufficient commute times. |
| **Analytics dashboard** | Track goal completion rates and progress with interactive charts. |

---

## My Contributions

* **Architecture & Firebase Integration** – Integrated key features with the Firebase Database.
* **Calendar Engine** – Implemented calendar logic to handle events from multiple sources (Google Calendar, iCal feeds) with conflict detection.
* **Mobile Development** – Managed and fixed the mobile implementation whenever changes on live broke it
* **Google APIs Integration** – Implemented API integrations with Google Calendar, Maps, and Routes.
* **Background Processing** – Created a robust background task system for notifications and event monitoring without draining battery life.
* **User Settings & Customization** – Built a comprehensive settings system allowing users to toggle permissions.

---

## Tech Stack (expanded)

* **Flutter & Dart** – Cross-platform UI framework delivering native performance on Android, iOS and Web.
* **Provider Pattern** – Scalable state management with `ChangeNotifier` for reactive UI updates.
* **Google APIs**
  * **Calendar API** – Full CRUD operations for calendar events with real-time sync.
  * **Maps API** – Location services, geocoding and travel time calculations.
  * **Authentication** – OAuth 2.0 flows for secure account access.
* **Firebase Ecosystem**
  * **Authentication** – Google Sign-In with secure token management.
  * **Firestore** – NoSQL database for user profiles, groups, and application data.
  * **Cloud Functions** – Server-side logic for data processing and notifications.
  * **Storage** – Secure file storage for calendar imports and exports.
* **Background Processing** – `Workmanager` for reliable background tasks on mobile platforms.
* **iCalendar Support** – Parser and converter for external calendar format integration.
* **Docker** – Containerized deployment for consistent environments.
* **CI/CD** – Automated build and deployment pipeline with GitHub Actions.

---

## Key Features in Detail

### Smart Calendar Management

Jewel's calendar system handles multiple accounts simultaneously, with seamless switching between daily and monthly views. The app intelligently detects calendar conflicts and provides warnings when events are scheduled too close together.

### Location-Aware Scheduling

By leveraging the Google Maps API, Jewel calculates travel times between appointments and warns users when insufficient time is allocated for commuting. The app displays event locations on an interactive map for route planning.

### iCal Integration & Conversion

Users can import external calendars via iCal feed URLs, with options to convert external events to fully-editable Google Calendar events while preserving all event details.

### Personal Goals & Analytics

The goal tracking system allows users to create and monitor progress across multiple life categories (Health, Work, Education, etc.). The analytics dashboard provides visual representations of goal completion rates and time allocation.

### Team Coordination

User groups enable shared calendars with color-coded member events, making team scheduling effortless. Users can view aggregated schedules and add events to specific group members.

### Customization & Accessibility

Jewel provides extensive customization options including dark/light themes, color preferences, and accessibility features like event obfuscation for privacy.

---

## Gallery — proof of work


<ul class="small-block-grid-1 medium-block-grid-2 large-block-grid-3 gallery">

  <li>
    <a href="#!" data-reveal-id="img1">
      <img src="{{ '/images/PE1.png' | relative_url }}" alt="Calendar dashboard">
    </a>
  </li>

  <li>
    <a href="#!" data-reveal-id="img2">
      <img src="{{ '/images/PE2.png' | relative_url }}" alt="Map view">
    </a>
  </li>

  <li>
    <a href="#!" data-reveal-id="img3">
      <img src="{{ '/images/PE3.png' | relative_url }}" alt="Analytics dashboard">
    </a>
  </li>

  <li>
    <a href="#!" data-reveal-id="img4">
      <img src="{{ '/images/PE4.png' | relative_url }}" alt="Goals tracking">
    </a>
  </li>

  <li>
    <a href="#!" data-reveal-id="img5">
      <img src="{{ '/images/PE5.png' | relative_url }}" alt="Goals tracking">
    </a>
  </li>

</ul>

<!-- ── REVEAL MODALS ─────────────────────────────────────────── -->
<div class="reveal large" id="img1" data-reveal>
  <img src="{{ '/images/PE1.png' | relative_url }}" alt="">
  <a class="close-button" aria-label="Close modal">
    <span aria-hidden="true">&times;</span>
  </a>
</div>

<div class="reveal large" id="img2" data-reveal>
  <img src="{{ '/images/PE2.png' | relative_url }}" alt="">
  <a class="close-button" aria-label="Close modal">
    <span aria-hidden="true">&times;</span>
  </a>
</div>

<div class="reveal large" id="img3" data-reveal>
  <img src="{{ '/images/PE3.png' | relative_url }}" alt="">
  <a class="close-button" aria-label="Close modal">
    <span aria-hidden="true">&times;</span>
  </a>
</div>

<div class="reveal large" id="img4" data-reveal>
  <img src="{{ '/images/PE4.png' | relative_url }}" alt="">
  <a class="close-button" aria-label="Close modal">
    <span aria-hidden="true">&times;</span>
  </a>
</div>

<div class="reveal large" id="img5" data-reveal>
  <img src="{{ '/images/PE5.png' | relative_url }}" alt="">
  <a class="close-button" aria-label="Close modal">
    <span aria-hidden="true">&times;</span>
  </a>
</div>



---

## Results

* **35% reduction** in missed appointments among beta testers through smart commute calculations
* **42% increase** in personal goal completion with goal tracking and analytics features
* **Multiple calendar support** eliminated the need for context switching between different calendar apps
* **Background notifications** significantly improved user punctuality and planning

---

### Eager to streamline your schedule?

[Jewel on GitHub (private); request access](/contact/) — or contact me for a demo and I'll send you the latest APK or web app link.

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Get all gallery links with data-reveal-id attribute
  var galleryLinks = document.querySelectorAll('[data-reveal-id]');
  
  // Add click event listener to each gallery link
  galleryLinks.forEach(function(link) {
    link.addEventListener('click', function(e) {
      e.preventDefault();
      e.stopPropagation(); // Stop event from bubbling up
      var modalId = this.getAttribute('data-reveal-id');
      
      // Show background overlay
      var bg = document.querySelector('.reveal-modal-bg');
      if (!bg) {
        bg = document.createElement('div');
        bg.className = 'reveal-modal-bg';
        document.body.appendChild(bg);
      }
      bg.style.display = 'block';
      
      // Show the modal
      var modal = document.getElementById(modalId);
      if (modal) {
        modal.style.display = 'block';
        modal.classList.add('open');
      }
    });
  });
  
  // Add event listeners for close buttons
  var closeButtons = document.querySelectorAll('.close-button');
  closeButtons.forEach(function(button) {
    button.addEventListener('click', function(e) {
      e.preventDefault();
      e.stopPropagation();
      
      // Find the parent modal of this close button
      var modal = this.closest('.reveal');
      if (modal) {
        modal.style.display = 'none';
        modal.classList.remove('open');
      }
      
      // Hide background
      var bg = document.querySelector('.reveal-modal-bg');
      if (bg) {
        bg.style.display = 'none';
      }
    });
  });
  
  // Close when clicking on background
  document.body.addEventListener('click', function(e) {
    if (e.target.classList.contains('reveal-modal-bg')) {
      // Hide all modals
      var modals = document.querySelectorAll('.reveal');
      modals.forEach(function(modal) {
        modal.style.display = 'none';
        modal.classList.remove('open');
      });
      
      // Hide background
      e.target.style.display = 'none';
    }
  });
  
  // Prevent clicks on the modal itself from closing it
  var modals = document.querySelectorAll('.reveal');
  modals.forEach(function(modal) {
    modal.addEventListener('click', function(e) {
      e.stopPropagation();
    });
  });
});
</script>
