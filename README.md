# Food Blog

- [Food Blog](#food-blog)
  - [Steps to make a website](#steps-to-make-a-website)
  - [Design Specs](#design-specs)
  - [Folder structure](#folder-structure)
  - [Fetch font from Internet](#fetch-font-from-internet)
  - [Css Fonts](#css-fonts)
  - [Responsive Web design](#responsive-web-design)
  - [External References](#external-references)
  - [Steps to be executed](#steps-to-be-executed)
  - [Headers](#headers)
  - [Figure](#figure)
  - [Floats](#floats)
  - [Selectors](#selectors)
  - [Tips](#tips)
  - [Bookmarks](#bookmarks)

## Steps to make a website

1. Define Goal
2. Define Content
   - Plan content - Imae, vieo etc
   - Plan Hierarchy
   - Define Navigtion
   - Define Side structure
3. Sketch your ideas
   - Draw your ideas
   - No need to make it too perfect
   - Never start a website without having a visual planning
4. Develop
   - Follow all industry practices, guidelines
   - Design using HTML and css
5. Optimize performance
6. Deploy
7. Maintenance
   - Update content regularly
   - Monitor the content

## Design Specs

- Color - Orange
- Font - LATO

## Folder structure

- `Resources` Stores folders/ files created by us
- `Vendors` Stores foldres/files downloaded from internet

## Fetch font from Internet

1. Go to [google fonts](https://fonts.google.com/)
2. Search for a font name eg. Lato
3. Select the specific font styles/sizes you ned
4. Copy the generated CDN link

## Css Fonts

- We can specify multiple fonts, so that if first is not available, other will be used and so on

```css
html {
  font-family: 'Lato', 'Arial', sans-serif;
}
```

## Responsive Web design

- Works well on all resolution
- Changes with different screen size
- Achieved by
  - `Fluid Grid` - All elementes are sized using relative values like % instead of fixed pixels
  - `Flexible Images` - Images must be sized relatively
  - **`Media queries`** - Specify different CSS rules for Different browser widths

## External References

- Fonts <https://fonts.google.com/>
- Normalize CSS <https://necolas.github.io/normalize.css>
- Siple Grid classes <http://www.responsivegridsystem.com/>

## Steps to be executed

1. WOrk with headers, ul, li
2. Put text on image, make iamge darker
3. Make imge as high as browser viewport
4. Make horizontal, vertical center box
5. Design Buttons
6. 4 link CSS: link, visisited, hover, active
7. CSS animation
8. Navigaion

## Headers

- Used to define tile, image, navigation etc.
- Used by SEOs to know about the site
- Better than using div which provides no meaning

## Figure

- Similar to image
- Used to organize image content
- img and its caption is added as child element in figure

## Floats

- After creating floats, always clear the,
- It can mess up DOM hierarchy

```css
/* Apply class in parent of child having float property */
.clearfix {
  zoom: 1;
}
.clearfix::after {
  content: '.';
  clear: both;
  height: 0;
  visibility: hidden;
  display: block;
}
```

- How to apply

```html
<ul class="clearfix">
  <li></li>
  <li></li>
</ul>
```

## Selectors

```css
/* Select nth element */
div:first-child {
}
/* Select by type */
input[type='text'] {
}
/* Select child item of a class */
.plan-box ul li {
}

/* Removes blackish outline on clicking n elemnt */
*:focus {
  outline: none;
}
```

## Tips

- Section can be separated by applying a slight tint to one of the section
- If we make an element absolute, make sure its parent is relative

## Bookmarks

1. Choose colors at <https://www.flatuicolors.com/>
2. Look for color shades at <https://www.0to255.com/>
3. Icons <https://ionicons.com/>
4. HTML glyphs <https://css-tricks.com/snippets/html/glyphs/>
5. Social media icon color <https://www.designpieces.com/2012/12/social-media-colours-hex-and-rgb/>
