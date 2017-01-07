# Facematter

My previous portfolio website versions were based off standard portfolio templates found on the internet (e.g. wix, squarespace and wordpress themes). Over time, my needs outgrew their features and the lack of complete control over code and my increasing interest in programming led to me hand-code this website myself and get the layout and typography I wanted.

# Development environment

## Setting up Jade templating engine

Jade is a templating engine that makes it very easy for me to write HTML code. I like Jade very much because I don't have to worry about closing HTML tags correctly and the syntax being concise makes the code very readable.

For simpler pieces of html content I use Markdown, but for my website I needed to be able to specify element IDs and CSS classes which I could not do in Markdown.

I installed Jade using the following commands

`
npm install jade
npm install jade-cli
`

I use Brackets as my text editor for web development and I installed the Jade plugin for syntax highlighting.

## Setting up CSS preprocessor

It was very easy to setup SCSS preprocessor in Brackets. I just installed a plugin and that was it! As long as I created a new file with a .scss extension, Brackets noticed it and setup the necessary compilers to compile this to CSS file.

I didn't start out with SCSS, but as I started writing more HTML I found out that I had some common parts of CSS between my various page types (Home, work pages and About Me). I didn't want to copy-paste the code as that would be less maintainable.

I also wanted to experiment with various typographic settings. SCSS gives support for variables and calculation functions using which I was able to write SCSS code such that if I changed the font-size variable for the base text then everything else (the font-size, line-height, margins, padding for H1, H2, H3, p etc) were automatically adjusted based on the base font size. This made it easy for me to test out various typographic scales (like the Golden ratio, Standard scale, Perfect fourth etc.)

`
$selected-stack: $font-stack;
$header-stack: $freightsanspro-stack;
$width: 50%;
$sidenotemargin: -($width+10%);
$black: rgba(0,0,0,.8);
$psize: 1.06rem;
$ledding: 1.86rem;
$fontweight: 400;
`

Here is my Brackets window demonstrating my setup
