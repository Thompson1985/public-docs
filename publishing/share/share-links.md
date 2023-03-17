---
description: >-
  Share links give you greater control over who can view your GitBook
  documentation.
---

# Share links

{% hint style="info" %}
This feature is available on our **Pro** and **Enterprise** plans.
{% endhint %}

Share your private content with customers and partners without inviting them to your organization by using a secret shareable link or links!

## Publish via share link

<figure><img src="../../.gitbook/assets/publish-via-share-link.png" alt="A screenshot of a GitBook space, with the visibility menu open. The selected visibility option is share link."><figcaption><p>A GitBook space published via share link</p></figcaption></figure>

To publish via share link(s), open the space or collection you want to share in GitBook. Open the visibility menu and select **share link**.

Next, click on **link and domain settings** to access your share links. From this area you can copy, re-generate, or revoke a share link.

<figure><img src="../../.gitbook/assets/configure-share-links.png" alt="A screenshot of a GitBook space with link and domain settings, which is accessed from the visibility menu, open. Specific share links can be configured from here."><figcaption><p>Link and domain settings for a GitBook space published via share link</p></figcaption></figure>

Once the link is active, a private token is generated within your URL, which is unique to your space. Sharing this link will give non-GitBook users access to your private content in read mode only.

{% hint style="info" %}
Share links can be [revoked](share-links.md#revoke-a-link) and regenerated at any time.
{% endhint %}

## Permissions

The content will be accessible to **anyone following the link**. Your team members will always be able to access your content from their dashboard.

{% hint style="info" %}
Make sure you share the link only with people you want to share your private content. Don't forget that you can [revoke](share-links.md#revoke-a-link) a link at any time.
{% endhint %}

## Revoke a link

The shareable link can be disabled or regenerated by revoking a link. You can see and revoke any previously generated link by opening the visibility menu and clicking through to link and domain settings.

{% hint style="warning" %}
**Heads up!** Anyone using a revoked link will no longer have access to your content.
{% endhint %}

## Security

### Privacy of my content is not critical

If you don't have strong privacy and security requirements, a better solution may be to publish the space as [unlisted](https://docs.gitbook.com/getting-started/publishing/space-publishing#unlisted-space). Unlisted spaces are not indexed by search engines, and therefore will not be easily discoverable.

### I need a more secure alternative

The most secure way to share your content with a private audience is to have them create a GitBook account and join your organization.

This process can be [automated using SSO/SAML](../publishing/broken-reference/), which can be used to create custom authentication for your documentation. However, this will require more setup on your end, and is a feature of our **Enterprise** plan only.

If you need complete control over access to your public content, you might like to use our [visitor authentication](../visitor-authentication.md) feature. Again, this is a feature of our **Enterprise** plan only.