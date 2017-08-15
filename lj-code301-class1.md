# LJ Code 301 - Day 1

Today I learned a little bit about responsive web design and how to use conditional media queries in CSS. One of the key selectors for this feature to work is by using: @media in CSS file.

Example:

@media screen and (min-width: 700px) {
	h1 {
	background-color: blue;
	}
}

(When the window is shrunk to 700px the color of the background will turn blue. If you want other changes to happen at 700px width then you can add multiple selectors within @media braces)

To make sure that code works a meta tag needs to be put in to the HTML file.
<meta name=“viewport” content=“width=device-width,initial-scale=1”>

—SMACSS—

SMACSS is the proper standard how to organize your CSS files and what selectors go into each file.

BASE = html, body, article, nav, aside, p, a, input

LAYOUT = classes (and sometimes ids),  header, footer

MODULE = internal, smaller components, navigation, headings, ul

Vendor directory (3rd party) - reset file
