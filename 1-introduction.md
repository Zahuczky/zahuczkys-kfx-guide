# KFX Guide – 01 – Introduction

So, this is more or less going to be an introductionary piece to my KFX guide.

The guide itself is cut up into smaller, different guides, as you’ll progress through the what, why and how of creating fancy karaoke effects with Aegisub.

Let’s quickly go through what you’re going to need.

-   **A computer**  (duh)  
    No but seriously, with the rapid advancements of mobile technology, I see more and more people asking about how to edit subtitles on phones/tablets, or people applying to fansub groups, without even having a computer. You’re gonna need one here, specifically one that runs either Windows, Linux or MacOS. (so no chromebooks and whatnot)
-   **[Aegisub](https://github.com/arch1t3cht/Aegisub/releases)** (<- this is a link, get this. not any other aegisub, but this)  
    I recommend using arch1t3cht’s Aegisub fork, as it’s the most up-to-date and maintained Aegisub version. You might encounter various problems using any other Aegisub version.
-   [**mpv**](https://mpv.io/installation/) (it’s a video player, no you shouldn’t use VLC/MPC/built in players…)  
    mpv is the best player to play back any kind of video if you want to display ASS subtitles on them. The libass(the current preferred ass subtitle renderer) version is always up to date, it doesn’t do anything funky to the videos blablabla, get mpv.
-   [**The KaraOK library and templater**](https://github.com/logarrhythmic/karaOK)  
    While Aegisub comes with a built in KFX templater, with this guide you’re going to get familiarized with the KaraOK templater and library made by logarithm.
    
    **Install steps:  
    **Clone the repository, or if you’re not familiar with git/github just press the green “Code” button to the upper right and click “Download ZIP”  
    **Windows:** Go to your AppData/Aegisub/Automation folder(you can get to appdata by typing %appdata% in the start menu and hitting enter) and copy the contents of the autoload directory of karaOK into your autoload directory, and copy the contents of KaraOK’s include directory to your include directory.  
    Li**nux:**  Copy the contents of the autoload and include directories into your ~/.aegisub/automation/autoload and include directories. If they don’t exist, you have to create them.  
    **MacOS:** In a finder window press cmd+shift+g and type ~/Library/Application Support/Aegisub/ into the dropdown. If you don’t have automation/autoload and include folders, create them and copy the KaraOK’s folders contents into them.
    
    After the copy process you can restart Aegisub(or rescan your autoload directory) and you have KaraOK installed.
    
-   The two major other options currently are [PyonFX](https://github.com/CoffeeStraw/PyonFX) which is a Python based kfx creation tool. The main idea is that you can code your entire effect in python, and [The0x539’s templater,](https://github.com/The0x539/Aegisub-Scripts/blob/trunk/src/0x.KaraTemplater.moon) which is similar to the built in templater and KaraOK, but works in a bit of a different way.  
    A lot of the knowledge that you can get from this guide can be adapted to other templaters later down the line, if you wish to switch, but this guide is not going to help you with that.
-   **Some programming experience** (optional)  
    A very integral part of creating KFX-es is coding.  
    While for the basic KFX template lines, you don’t really need any kind of coding knowledge, those can only get you so far. The real muscle KFX-ers can leverage for KFX-es are LUA programming. You can basically insert any kind of lua code into your kfx template, so you can create very complex stuff. As long as you can code it.  
    
-   **Creativity**  
    I’m sure when you first thought about becoming a KFX-er, you already had some bangin style ideas in your head. That’s good.  
    Hopefully, when you reach the end of this guide, you won’t have any technical obstacles ahead of you, your creativity is going to be the limit.
    
    I guess that’s it for the “what.” Now let’s focus on the “why.”
    
This a bit of a harder topic, as there are very few technical arguments for creating any kind of KFX or song styling for the openings/endings/insert songs for anime fansubs.  
    It looks cool. It gives a bit more  _umphh_ to the songs. It can enhance the experience. I think so. Some people don’t even like the idea of adding any kind of romaji to the song translations, with the argument of “you’re creating subtitles in X language, why would you add Japanese back?”  
    Eh. If you’re here and reading this, you probably don’t think about it that way, although you can create karaoke effects for translated lyrics as well, like how it usually is in GJM releases. Takes a bit more effort on the translation side of things tho, to make your translation singable.
    

We can go through some examples now. (File sizes of these videos can reach up to 100MB/video. So if you’re on a metered connection, like mobile data, you might want to skip watching these)  
These are all kfx-es made by me.

<a href="https://files.catbox.moe/pz2gkz.mp4" target="_blank"> 
<img src="https://files.catbox.moe/yjey14.png" />
</a>

This is the opening of Ijiranaide, Nagatoro-san, with the KFX I made for the BullySubs release.  
I would call this a “medium complexity” kfx. The shake and color change of every line require some knowledge(and a lot of time, especially for the color change), so this is not the “first KFX you’re gonna create” but you can get on this level relatively quickly.

<a href="https://files.catbox.moe/8zscy5.mp4" target="_blank"> 
<img src="https://files.catbox.moe/zez1q9.png" />
</a>

This the opening of the 3rd season of Kaguya-sama wa Kokurasetai, I made this(a couple of lines were done by LightArrowsEXE) for the GJM release. The keen-eyed among you might’ve already noticed, that this is not a “KFX” in a sense that most lines are not even k-timed, there are no per-syllable effects and the sort. I prefer to call these “song stylings” rather than karaoke effects, since well, the karaoke part is largely missing. While there are a few lines kfx-ed, that’s just for stylistic reasons. Some of these lines were made with regular typesetting practices, but most of them were done with kfx templates. Only that the karaoke part was left out. So as you can see, you can use templates like this as well.

<a href="https://files.catbox.moe/pyrb91.mp4" target="_blank"> 
<img src="https://files.catbox.moe/5usute.png" />
</a>

This the special ending for the 6th episode of Ijiranaide, Nagatoro-san, I made for the BullySubs release.  
Yes, this is a kfx. No, there are no actual lyrics.  
Got it? No? Whatever.  
Don’t let them haters tell you that you need lyrics.  
(okay, the music is a chiptune verion of the actual song)

<a href="https://files.catbox.moe/qeomjo.mp4" target="_blank"> 
<img src="https://files.catbox.moe/8s3kvs.png" />
</a>

This the ending of Ranpo Kitan, but it was never used in a release, only shared as itself on nyaa under my ZahuFX tag.  
With some of the previous examples I’ve shown, you might think now that you need multiple effects for each song, greatly increasing the time and effort needed to make one effect. That is not the case. Most of the times, you can make an effect that is fitting for the entire song, as you can see here.

So, what did all of these had in common?  
Nothing?  
Come on, be a bit more open-minded.  
What they have in common is the fact, that they were specifically tailored for the given show. They’re matched to the stlye of the visuals.  
This is the  _essence_ of KFX-ing and song styling in general in my opinion. Make it pleasing to look at, while it blends in well. It should look like it was originally made for the song.

I think that’s it for this introduction.  
In the next chapter you’re going to get introduced to the ASS format.  
Soon™

_Legal disclaimer: The usage of all copyrighted material used on this page_  _falls under FAIR USE(Copyright act 1976, section 107) as it is used for  **educational porpuses,** these are **published fictional works,** generally **on average less than 1% of the copyrighted material is used, and has no effect on the distribution and market of the material.**_
