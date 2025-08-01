---
description: Deliver a tailored documentation experience based on who's reading.
icon: stars
---

# Adaptive content

{% include "../../.gitbook/includes/ultimate-hint.md" %}

When a user visits your site, you may already know things about them - who they are, which plan they're subscribed to, which features they have access to.

Adaptive content helps to build a tailored documentation experience based on who is reading.

<figure><img src="../../.gitbook/assets/28_07_25_adaptive_content (1).svg" alt="A GitBook screenshot showing adaptive content controls"><figcaption><p>Personalize your user’s documentation experience through adaptive content</p></figcaption></figure>

<p align="center"><a href="https://gitbook.com/adaptive-content-demo/" class="button primary">Launch the demo site</a></p>

{% hint style="info" %}
Adaptive content is slightly different from [authenticated access](../authenticated-access/), although they can work together.&#x20;

While authenticated access allows you to protect your docs through a login, adaptive content customizes published material based on various authentication methods — including authenticated access or those from your own app.
{% endhint %}

### How it works

Adaptive content works in 1 of 2 ways:

1. Passing data from your app to GitBook
2. Passing data from authenticated access

When a user visits your sites, we call the data they bring with them their "claims"—basically data that helps to identify a user. These claims are controllable by you - the site author - and can be used through the GitBook editor to show or hide different pages, variants, and sections in your docs.

Head to [Enabling adaptive content](enabling-adaptive-content/) to start setting up adaptive content for your site.
