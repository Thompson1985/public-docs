---
description: >-
  Add an image or a gallery of images to a page, add image variants for dark
  mode, and resize and align images to your needs
---

# Images

You can insert images into your page, then choose their size and whether to align them to the left, center, or right. You can also optionally include alt text and/or a caption on your image block.&#x20;

{% hint style="info" %}
**Tip:** For accessibility purposes, we recommend setting alt text for your images.
{% endhint %}

### Example of an image block <a href="#example-of-an-image-block" id="example-of-an-image-block"></a>

<div align="center"><img src="https://images.unsplash.com/photo-1446776709462-d6b525c57bd3?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxzcGFjZXxlbnwwfHx8fDE3MzMxOTY5NTR8MA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt="A photograph taken from space looking back towards Earth. A satellite is in the foreground, and in the background is an ocean-covered part of our planet with patchy clouds."></div>

### Uploading an image

There are two ways to add images to your content:

1. Drag and drop the image from your file management system directly into an empty block on your page.
2. [Add an image block](./#inserting-a-new-content-block) to your page and use the **Select images** side panel that appears on the right of the window.&#x20;

If you follow the second process, you can choose to upload a file, select a previously-uploaded file, paste an image URL or add an image from [Unsplash](https://unsplash.com/) using the built-in search.

{% hint style="warning" %}
GitBook allows you to upload images up to 100MB per file.
{% endhint %}

#### Create an image gallery

Adding more than one image to an image block will create a gallery. To do this, open the block’s **Options menu** <picture><source srcset="../../.gitbook/assets/options_menu_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/options_menu_icon_light.svg" alt="The Options menu icon in GitBook"></picture> and choose **Add images…** to open the **Select images** side panel again.

To delete an image from a gallery, open the **Actions menu** <picture><source srcset="../../.gitbook/assets/actions_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/actions_icon_light.svg" alt="The Actions menu icon in GitBook"></picture> on the image you want to delete and press the **Delete ⌫** key.

### Adding images for light & dark mode <a href="#light-and-dark-mode" id="light-and-dark-mode"></a>

You can set different images for the light and dark mode versions of your published site. GitBook will automatically display the correct image depending on the mode your visitor is in.

To add an image for dark mode, hover over your image, open the **Actions menu** <picture><source srcset="../../.gitbook/assets/actions_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/actions_icon_light.svg" alt="The Actions menu icon in GitBook"></picture> and click **Replace image** <picture><source srcset="../../.gitbook/assets/replace_image_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/replace_image_icon_light.svg" alt="The Replace image icon in GitBook"></picture>.&#x20;

In the drop-down menu, choose **Add image for Dark mode**. Once you’ve set this, you can replace either image from this same menu.

{% hint style="warning" %}
**Note:** GitBook doesn’t currently support light and dark mode images for certain cases, including page covers or image covers on [cards](cards.md).
{% endhint %}

### Light and dark mode images through GitHub/GitLab Sync <a href="#light-and-dark-mode-through-github-gitlab-sync" id="light-and-dark-mode-through-github-gitlab-sync"></a>

You can also add light and dark mode images in Markdown through HTML syntax (`<picture>` and `<source>`).

For block images, use the `<figure>` HTML element with a `<picture>` and `<source>` in it:

```html
Text before

<figure>
  <picture>
    <source
      srcset="
        https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png
      "
      media="(prefers-color-scheme: dark)"
    />
    <img
      src="https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png"
      alt="GitHub logo"
    />
  </picture>
  <figcaption>Caption text</figcaption>
</figure>

Text after
```

For inline images (images that sit inline with text), use the `<picture>` HTML element with a `<source>` in it:

```html
Text before the image
<picture
  ><source
    srcset="
      https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png
    "
    media="(prefers-color-scheme: dark)" />
  <img
    src="https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png"
    alt="The GitHub Logo"
/></picture>
and text after the image
```

{% hint style="warning" %}
**Note:** We don’t yet support [GitHub-only syntax](https://github.blog/changelog/2021-11-24-specify-theme-context-for-images-in-markdown/) through `#gh-dark-mode-only` or `#gh-light-mode-only`.
{% endhint %}

### Resizing

To resize your image, hover over it and open the **Actions menu** <picture><source srcset="../../.gitbook/assets/actions_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/actions_icon_light.svg" alt="The Actions menu icon in GitBook"></picture>. Click the **Size** button to change the size of your image from the available options.

<figure><img src="../../.gitbook/assets/10_01_25_image_resizing.svg" alt="A GitBook screenshot showing how to resize an image" ><figcaption><p>Resize an image</p></figcaption></figure>

- **Small** – 25% of the image size
- **Medium** – 50% of the image size
- **Large** – 75% of the image size
- **Fit** – Removes all size specifications and displays either at full size or capped at a maximum width of **735** **pixels** for larger images.

If your image is wider than the editor, GitBook will limit the image’s width to the editor’s width instead, and resizing will be based on this limit.

{% hint style="info" %}
**Note:** When resizing images in an image gallery, the results can differ from resizing an individual image.
{% endhint %}

{% hint style="info" %}
You can make image blocks [span the full width of your window](./#full-width-blocks) by clicking on the **Options menu** <picture><source srcset="../../.gitbook/assets/options_menu_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/options_menu_icon_light.svg" alt="The Options menu icon in GitBook"></picture> next to the block and choosing **Full width**.
{% endhint %}

### Resizing images through Git Sync

If you want more control over the sizing of your image, you can specify the exact size using Markdown in GitHub or GitLab.

When we export an image, we use the HTML tag `<img/>`. As per the specifications, we can specify the dimensions of the image using the `width` and `height` attributes, which only accept values in pixels or a combination of a number and a `%` sign.\
\
Valid variants for specifying the image dimensions are:\
\
`<img width="100" />` Sets the image to 100 pixels wide\
`<img width="100%" />` Sets the image to full size (although this will be limited by the editor)

### Aligning images

By default, image blocks will show your image at its full size, aligned centrally.

To change the alignment of an image, open the block’s **Options menu** <picture><source srcset="../../.gitbook/assets/options_menu_icon_dark.svg" media="(prefers-color-scheme: dark)"><img src="../../.gitbook/assets/options_menu_icon_light.svg" alt="The Options menu icon in GitBook"></picture> and choose the alignment you want. This will only affect images that are narrower than the editor, or images you’ve [resized](insert-images.md#resizing).

### Representation in Markdown

```markdown
//Simple Block
![](https://gitbook.com/images/gitbook.png)

//Block with Caption
![The GitBook Logo](https://gitbook.com/images/gitbook.png)

//Block with Alt text

<figure><img src="https://gitbook.com/images/gitbook.png" alt="The GitBook Logo"></figure>

//Block with Caption and Alt text

<figure><img src="https://gitbook.com/images/gitbook.png" alt="The GitBook Logo"><figcaption><p>GitBook Logo</p></figcaption></figure>

//Block with different image for dark and light mode, with caption

<figure>
  <picture>
    <source srcset="https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png" media="(prefers-color-scheme: dark)">
    <img src="https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png" alt="GitHub logo">
  </picture>
  <figcaption>Caption text</figcaption>
</figure>
```
