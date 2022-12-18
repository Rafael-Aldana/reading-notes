# Class 11 code-201d93

Explain how the ability to use video and audio on the web has evolved since the early 2000s.
The video and audio abilities first started as proprietary plugin-based technologies like flash and silverlight. Both of these had security and accessibility issues and since become absolete.

Describe the use of the src and controls attributes in the <video> element.
The src attribute contains a path to the video you want to embed, and the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.

Why is it important to have fallback content inside the <video> element?
The importance of having the fallback content inside the video element is because if the video isn't supported by the browser the user can at least have a direct link to the video file so the user can access it.

Write a very short story where <audio> and <video> are characters. Video and and audio are partners but they both different things to the relationship for obvious reasons.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content).
********************************************************************************************************************
How does Grid layout differ from Flex?
CSS Grid Layout (aka “Grid” or “CSS Grid”), is a two-dimensional grid-based layout system that, compared to any web layout system of the past, completely changes the way we design user interfaces. CSS has always been used to layout our web pages, but it’s never done a very good job of it. First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance). Flexbox is also a very great layout tool, but its one-directional flow.

Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.
To get started you have to define a container element as a grid with display: grid, set the column and row sizes with grid-template-columns and grid-template-rows, and then place its child elements into the grid with grid-column and grid-row. Similarly to flexbox, the source order of the grid items doesn’t matter. Your CSS can place them in any order, which makes it super easy to rearrange your grid with media queries. Imagine defining the layout of your entire page, and then completely rearranging it to accommodate a different screen width all with only a couple lines of CSS. Grid is one of the most powerful CSS modules ever introduced.

[link-to-reading-notes](https://css-tricks.com/snippets/css/complete-guide-grid/).
********************************************************************************************************************
Besides making a site visually appealing across different screen sizes, why should developers make images responsive?
The advantages of having responsive images is that if the user is utilizing a narrow screen device the image won't break or crop itself.

Define the following <img> attributes srcset and sizes. Write an example of how they are used.
The srcset attribute defines the set of images the browser is allowed to choose between and what size each image is, each set is seperated by a comma. As for the sizes attribute defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true.
<img
  srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
  sizes="(max-width: 600px) 480px,
         800px"
  src="elva-fairy-800w.jpg"
  alt="Elva dressed as a fairy" />

How is srcset more helpful for responsive images than CSS or JavaScript?
The srcset allows the browser to choose which picture best fits the current version of the browser.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images).