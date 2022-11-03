# KFX Guide – 02 – The ASS subtitle format

In this chapter, you’re going to get introduced to the ASS subtitle format, and every ASS tag.

I will make it clear now, that this is not a full-on “Aegisub guide,” it is assumed that you already know your way around Aegisub, at least in a sense that you can navigate the software.

If you have no experience with the software, google can probably help you with getting going, and you can always ask others for help.  
The best place to ask help in is the [GoodJob! Media Discord server](https://discord.gg/hQewDqS).  
Upon joining, you can ask an admin or a moderator to give you the “Subber role” and with that you can have access to subtitling specific channels. I recommend asking these kind of questions in the #typesetting channel.

With that out of the way, let’s go through how a line is constructed in the ASS format.  
You can divide what’s inside a line into two basic parts.  
Things that are in {curly brackets} and things that are outside of it.

<?xml version="1.0" encoding="utf-8"?>
<svg version="1.1"
     xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     width="100" height="50"
>
  <text font-size="16" x="10" y="20">
    <tspan fill="red">Hello</tspan>,
    <tspan fill="green">world</tspan>!
  </text>
</svg>

