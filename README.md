# about:custom-home
A self-contained HTML page to replace your browsers start page with. Shows current time, greets you and tells you how far the year, month and day have progressed so far.

## Installation

Download the `custom-home.html` and place it somewhere accessible for your browser like your documents folder.
Open the file in your browser and copy the address from the address bar (should start with `file:///`).
Go to your browser settings, change your homepage to a URL and paste the address copied previously.
Restart your browser to see the effect.

Tested in the following browsers:
- Firefox 128.0.3
- Chrome 109
- Microsoft Edge 109

![Example of what it looks like](./img/example.png?raw=true "Here is an example of what about:custom-home may look like")

## Usage
To customize some things, find the beginning of the `<script>` tag at the bottom of the html document.
Modify the following constants to your liking:
- `yourName`: Put your name here so the script knows how to greet you
- `updateIntervalSeconds`: Changes the time between updates of the progress bars
- `precision`: Modify the number of decimals of the progress bars
- `usePicsum`: Set this to `true` to get a random background image from [Unsplash](https://unsplash.com/). Use `false` to use neutral colors (depending on whether light or dark mode is used)
- `filter`: Only has an effect when `usePicsum` is active. Use this to apply filters such as `grayscale` or `blur` (see [whats possible](https://picsum.photos/)). Separate filters by a comma and keep the `?` in front. If you want no filters, use an empty string.

## Contributing
Pull requests are welcome.

## Acknowledgment
With the recent changes to Twitter, one of my [favorite bots (@year_progress)](https://twitter.com/year_progress) will soon stop to work, so I was looking for a way of showing the years progress in a place visible but not obtrusive.
Thanks to [Filip Hráček](https://filiph.net/) ([@filiph](https://github.com/filiph)), the creator of said bot, and his [server that controls it](http://progressbarserver.appspot.com/), I had the idea to use something similar for my browsers homepage. I didn't want to rely it loading from a server, so I made this local html file.
Filip's bot is also available on [Mastodon](https://techhub.social/@year_progress), if you're interested.