---
aliases:
  - How to/Embed files
  - Linking notes and files/Embedding files
cssclasses:
  - soft-embed
---

Learn how you can embed other notes and media into your notes. By embedding files in your notes, you can reuse content across your vault.

To embed a file in your vault, add an exclamation mark (`!`) in front of an [[Internal links|Internal link]] or use [[HTML content|HTML tags]]. You can embed files in any of the [[Accepted file formats]].

## Embed a note in another note

To embed a note:

```md
![[Internal links]]
```

You can also embed links to [[Internal links#Link to a heading in a note|headings]] and [[Internal links#Link to a block in a note|blocks]].

```md
![[Internal links#^b15695]]
```

The text below is an example of an embedded block:

![[Internal links#^b15695]]

## Embed an image in a note

To embed an image, drag and drop it into your note. This will upload the file to your vault, and add a reference to it like this:

```md
![[Engelbart.jpg]]
```

![[Engelbart.jpg#outline]]

You can change the image dimensions, by adding `|640x480` to the link destination, where 640 is the width and 480 is the height.

```md
![[Engelbart.jpg|100x145]]
```

If you only specify the width, the image scales according to its original aspect ratio. For example, `![[Engelbart.jpg|100]]`.

![[Engelbart.jpg#outline|100]]

You can also embed an externally hosted image by using a markdown link. You can control the width and height the same way as a wikilink. 

```md
![250](https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/Engelbart.jpg)
```

![250](https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/Engelbart.jpg)

Likewise, you can embed an image stored on your PC without copying it to your vault like so:

```md
![local photo](<C:\Users\username\Pictures\image file.PNG>)
```

## Embed an audio file in a note

To embed an audio file, drag and drop it into your note. This will upload the file to your vault, and add a reference to it like this:

```md
![[Excerpt from Mother of All Demos (1968).ogg]]
```

![[Excerpt from Mother of All Demos (1968).ogg]]

To embed an audio file hosted online, use [[HTML content]]:

```html
<audio controls src="https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/audio/Excerpt%20from%20Mother%20of%20All%20Demos%20(1968).ogg" type="audio/ogg">
</audio>
```

<audio controls src="https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/audio/Excerpt%20from%20Mother%20of%20All%20Demos%20(1968).ogg" type="audio/ogg">
</audio>

To embed an audio file saved on your PC outside of your vault, you can use also use [[HTML content]] like so:

```html
<audio controls src="C:\Users\username\Music\audio file.mp3" type="audio/mpeg"></audio>
```

## Embed a video file in a note

To embed a video, drag and drop it into your note. This will upload the file to your vault, and add a reference to it like this:

```md
![[Video clip.mp4]]
```

To embed a video file hosted online, use [[HTML content]]:

```html
<video controls src="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" type="video/mp4">
</video>
```
<video controls src="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" type="video/mp4">
</video>

To embed a video file saved on your PC outside of your vault, you can use also use [[HTML content]] like so:

```html
<video controls src="C:\Users\username\Videos\video file.webm" type="video/webm"></video>
```

![[Embed web pages#Embed a YouTube video]]

## Embed a PDF in a note

To embed a PDF, drag and drop it into your note. This will upload the file to your vault, and add a reference to it like this:

```md
![[Document.pdf]]
```

You can also open a specific page in the PDF, by adding `#page=N` to the link destination, where `N` is the number of the page:

```md
![[Document.pdf#page=3]]
```

You can also specify the height in pixels for the embedded PDF viewer, by adding `#height=[number]` to the link. For example:

```md
![[Document.pdf#height=400]]
```

## Embed a list in a note

To embed a list from a different note, first add a [[Internal links#Link to a block in a note|block identifier]] to your list:

```md

- list item 1
- list item 2

^my-list-id
```

Then link to the list using the block identifier:

```md
![[My note#^my-list-id]]
```

## Embed search results 

![[Search#Embed search results in a note]]
