# Readings: Images, Color, Text

## Index

[HOME](./README.md)  

[HTML Media](#html-media)

- [Using Images in HTML](#using-images-in-html)
- [Common Image Types](#common-image-types)
- [Choosing Image Formats](#choosing-image-formats)

[Learn CSS](#learn-css)

- [Using Color in CSS](#using-color-in-css)
- [HTML Text Elements](#html-text-elements)

## [HTML Media](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding)

### [Using Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

1. What is a real world use case for the `alt` attribute being used in a website?
   - The user is visually impaired, and is using a screen reader to read the web out to them. In fact, having alt text available to describe images is useful to most users.
   - As described above, the spelling of the file or path name might be wrong.
   - The browser doesn't support the image type. Some people still use text-only browsers, such as Lynx, which displays the alt text of images.
   - You may want to provide text for search engines to utilize; for example, search engines can match alt text with search queries.
   - Users have turned off images to reduce data transfer volume and distractions. This is especially common on mobile phones, and in countries where bandwidth is limited or expensive.

2. How can you improve accessibility of images in an HTML document?
   - **It is better to include supporting information in the main article text, rather than attached to the image.**
   - Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
   - Don't say "link" or "links to" in the link text — it's just noise. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
   - Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
   - Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here".

### [Common Image Types](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types)

1. Provide an example of when the [figure](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure) element would be useful in an HTML document.
   - Quotations
   - Poems
   - Code snippets
   - Images

### [Choosing Image Formats](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types#choosing_an_image_format)

1. Describe the difference between a `gif` image and an `svg` image, pretend you are explaining to an elder in your community.
   - Gif's are awesome and playing small animations silly meme's and svg's are really good for icons, diagrams and interfaces like buttons on a page.
2. What image type would you use to display a screenshot on your website and why?
   - PNG mostly and mabe WebP, PNG particularly if there is any text in the image.  Text tends to get fuzzy if compressed too much so lossless formats are the best choice.

## [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

### [Using Color in CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color)

1. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.
   - Basically, the foreground color is mainly text and the background is literally just that, the backgrounds color.
  
2. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?
   - The first step is to define a base color
     - A color that is naturally associated with the topic of your content, such as the existing color identified with a product or idea or a color representative of the emotion you wish to convey.
     - A color that comes from imagery associated with what your content is about. If you're creating a website about a given item or product, choose a color that's physically present on that item.
     - Browse websites that let you look at lots of existing color palettes and images to find inspiration.
   - Fleshing out the palette
     - With base establised it's time to pick a palette and there are many tools available
       - [MDN's color picker tool](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Color_picker_tool);
       - [Paletton](https://paletton.com/)
       - [Adobe Color CC online color wheel](https://color.adobe.com/create/color-wheel)
       - And a personal favorite of mine [Coolor Pallet Generater](https://coolors.co/generate)
     - Something to consider here would be [accessability]( Color and accessibility) for the color blind and the like.

### [HTML Text Elements](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

1. What should you consider when choosing fonts for an HTML document?
   - Web safe fonts
   - Mono spacing
   - Style
   - Font Stacks
     - Since you can't guarantee the availability of the fonts you want to use on your webpages (even a web font could fail for some reason), you can supply a font stack so that the browser has multiple fonts it can choose from. The browser starts at the beginning of the list and looks to see if that font is available on the machine. If it is, it applies that font to the selected elements. If not, it moves on to the next font, and so on.
   - An incredible resource for fonts lives at [CSS Font Stack](https://www.cssfontstack.com/). You can find links to fonts and easily accessible information about the likelyhood of the operating system having access to it.

2. What do `font-size`, `font-weight`, and `font-style` do to HTML text elements?
   - [font-size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size) **changes the font size using multiple different possible attributes. A few of which are listed below**
     - `px` (pixels): The number of pixels high you want the text to be. This is an absolute unit — it results in the same final computed value for the font on the page in pretty much any situation.
     - `em`s: 1 `em` is equal to the font size set on the parent element of the current element we are styling (more specifically, the width of a capital letter M contained inside the parent element). This can become tricky to work out if you have a lot of nested elements with different font sizes set, but it is doable, as you'll see below. Why bother? It is quite natural once you get used to it, and you can use `em` to size everything, not just text. You can have an entire website sized using `em`, which makes maintenance easy.
     - `rem`s: These work just like em, except that 1 rem is equal to the font size set on the root element of the document (i.e. `<html>`), not the parent element. This makes doing the maths to work out your font sizes much easier, although if you want to support really old browsers, you might struggle — rem is not supported in Internet Explorer 8 and below.

     ```css
     /* <absolute-size> values */
     font-size: xx-small;
     font-size: x-small;
     font-size: small;
     font-size: medium;
     font-size: large;
     font-size: x-large;
     font-size: xx-large;
     font-size: xxx-large;

     /* <relative-size> values */
     font-size: smaller;
     font-size: larger;

     /* <length> values */
     font-size: 12px;
     font-size: 0.8em;

     /* <percentage> values */
     font-size: 80%;

     /* math value */
     font-size: math;

     /* Global values */
     font-size: inherit;
     font-size: initial;
     font-size: revert;
     font-size: revert-layer;
     font-size: unset;
     ```

     - [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight) sets the weight (or boldness) of the font. The weights available depend on the font-family that is currently set.

     ```css
     /* Keyword values */
     font-weight: normal;
     font-weight: bold;

     /* Keyword values relative to the parent */
     font-weight: lighter;
     font-weight: bolder;

     /* Numeric keyword values */
     font-weight: 100;
     font-weight: 200;
     font-weight: 300;
     font-weight: 400;// normal
     font-weight: 500;
     font-weight: 600;
     font-weight: 700;// bold
     font-weight: 800;
     font-weight: 900;

     /* Global values */
     font-weight: inherit;
     font-weight: initial;
     font-weight: revert;
     font-weight: revert-layer;
     font-weight: unset;
     ```

     - [font-style](https://developer.mozilla.org/en-US/docs/Web/CSS/font-style) sets whether a font should be styled with a normal, italic, or oblique face from its `font-family`.

     ```css
     font-style: normal;
     font-style: italic;
     font-style: oblique;
     font-style: oblique 10deg;

     /* Global values */
     font-style: inherit;
     font-style: initial;
     font-style: revert;
     font-style: revert-layer;
     font-style: unset;
     ```

3. Describe two ways you could add spacing around the characters displayed in an `h1` element.
   - The [letter-spacing](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing) CSS property sets the horizontal spacing behavior between text characters. This value is added to the natural spacing between characters while rendering the text. Positive values of `letter-spacing` causes characters to spread farther apart, while negative values of `letter-spacing` bring characters closer together.

     ```css
     /* Keyword value */
     letter-spacing: normal;

     /* <length> values */
     letter-spacing: 0.3em;
     letter-spacing: 3px;
     letter-spacing: .3px;

     /* Global values */
     letter-spacing: inherit;
     letter-spacing: initial;
     letter-spacing: revert;
     letter-spacing: revert-layer;
     letter-spacing: unset;
     ```

   - The [word-spacing](https://developer.mozilla.org/en-US/docs/Web/CSS/word-spacing) property sets the length of space between words and between tags.

      ```css
      /* Keyword value */
      word-spacing: normal;

      /* <length> values */
      word-spacing: 3px;
      word-spacing: 0.3em;

      /* <percentage> values */
      word-spacing: 50%;
      word-spacing: 200%;

      /* Global values */
      word-spacing: inherit;
      word-spacing: initial;
      word-spacing: revert;
      word-spacing: revert-layer;
      word-spacing: unset;
      ```

[Back to Top](#index)
