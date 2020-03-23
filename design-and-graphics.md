# Design and Graphics

## Photo Editing / Painting

- [Krita](https://krita.org/en/) - Open-source painting program. Pretty slick and developing a big following.
- [GIMP](https://www.gimp.org/) - Or GNU Image Manipulation Program. Photoshop if it were designed by Linux engineers. Always been an ugly interface, but it has lots of power.
- See [Non-Data Python](non-data-python.md) for info on Pillow, a Python image manipulation library. Good stuff.

## Stock Photos

- [Unsplash](https://unsplash.com/) - "Beautiful, free photos. Gifted by the world’s most generous community of photographers."
- [Pexels](https://www.pexels.com/) - Free stock photos & videos

## Vector Graphics

- [Inkscape](https://inkscape.org/en/) - Imagine Adobe Illustrator if it were designed by Linux engineers. Again, ugly interface, but plenty of power.
- [Undraw](https://undraw.co/) - A constantly updated design project with beautiful SVG images that you can use completely free and without attribution
- [Humaaans](https://www.humaaans.com/) - Mix-&-match illustrations of people with a design library

## Prototyping

- [Adobe XD](https://www.adobe.com/products/xd.html) - Finally available for all editions of Windows 10, this is pretty legit. I can't believe Adobe is giving it away for free. Update: Adobe is putting restrictions on free plan, like ending local storage in April 2020)
- [Canva](https://www.canva.com) - Collaborative group design and brand editor.
- [MockFlow](https://mockflow.com) - Pretty easy to use wireframing/prototyping tool. Good if limited free plan (only 3 mockups allowed).
- [Miro](https://miro.com/) - Online collaborative whiteboarding platform.
- [Overflow](https://overflow.io) - "User flows done right." [Here's an example.](https://overflow.io/s/9ST7SX/)
- [Figma](https://www.figma.com) - Doesn't have UI components built-in like MockFlow, but for making quick drawings, sharing them with team members, and having everything sync beautifully online/offline, it's really pretty good.
- [Pencil Project](https://pencil.evolus.vn/) - Undergoing a major overhaul to make it a more modern system. Supposedly quite robust.
- [Atomic](https://atomic.io)
- [Sketch](https://www.sketch.com/) - macOS digital desgin toolkit with a strong plugin community. Probably the most popular thing on here.
- [Zeplin](https://zeplin.io/) - Collaboration tool between designers and developers to share designs, assets, and measurements.
- [Mural](https://mural.co/) - Digital workspace for visual collaboration.
- [Notely](https://note.ly/) - Free sticky note application.
- [Idea Flip](https://ideaflip.com/) - Web app for group brainstorms and individual ideas.

Also of interest may be this [comparison from the Vox Product Team](https://product.voxmedia.com/2017/11/1/16562200/a-highly-subjective-guide-to-design-prototyping-tools) that's pretty useful.

Additionally, Lucid Meeting has a [blog post](https://blog.lucidmeetings.com/blog/25-tools-for-online-brainstorming-and-decision-making-in-meetings) that tests out and categories many of these design / collaboration tools.

## Site Templates / Components

- [USWDS - US Web Design System](https://designsystem.digital.gov/) - A comprehensive design system developed by the US Digital Service.
- [HTML5Up](https://html5up.net/) - Free, responsive, nice-looking HTML5 site templates.

## Flowcharts

- [Coggle](https://coggle.it/flowcharts) - An offshoot of a mindmapping tool, this is a well-designed, easy-to-use flowchart tool. Nice free plan: 3 private flowcharts, unlimited public ones.

## Timeline Tools

- [Adobe Spark Timeline Maker](https://spark.adobe.com/make/timeline-maker/)

## Video

- [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve/) - To quote [Engadget](https://www.engadget.com/2018/08/22/davinci-resolve-15-free-hollywood-video-editor-review/), "DaVinci Resolve 15 is a free, Hollywood-grade video editor." Incredibly powerful stuff. I kinda can't believe how much is in the free version.
- [AutoEdit](http://www.autoedit.io/) - Interesting concept. This thing will automatically generate a transcript of your video, then allow you to make selections from the transcript. The selections you make can be exported to be stitched together into a proper video. Apparently cuts down the video editing process immensely.
- [OBS Studio](https://obsproject.com/) - World-class open-source screen recorder / video streamer. Warning: can get funky on Windows Surface Books, etc. or anything with multiple graphics cards. Trust me. But it generally just really does the trick.
- [ffmpeg](https://www.ffmpeg.org/) - Incredibly powerful command-line video conversion tool. Like so: `$ ffmpeg -i input.mp4 output.avi`. As a more serious example, I recorded a screencast using OBS Studio as a `.mkv` file, and wanted to make a GIF out of it. [GIPHY Engineering](https://engineering.giphy.com/how-to-make-gifs-with-ffmpeg/) blog helped me out, but it was pretty easy:
  - Generate a color palette `.png` file using this command: `ffmpeg -i '.\2020-01-07 10-26-50.mkv' -filter_complex "[0:v] palettegen" palette.png`.
  - Use that palette as kind of a key/overlay from which to pull colors during the conversion:
  `ffmpeg -i '.\2020-01-07 10-26-50.mkv' -i .\palette.png -filter_complex "[0:v][1:v] paletteuse" 2020_01_07-screencast.gif`

## Stock Video

- [MixKit](https://mixkit.co) - Completely free stock videos, license free. They ask for attribution, if possible.

## Content Management Systems

- [Site Leaf](https://www.siteleaf.com/) - Based on [Jekyll](http://jekyllrb.com/).

## General

- [Product Hunt has a good collection of $0 design tools](https://www.producthunt.com/e/0-design-tools), some of which are already on this list.
