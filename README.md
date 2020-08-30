# Remixed themes for Obsidian

I've frankensteined some themes together to get the color pallettes I want with my favorite layout.  I have Keyboard Maestro switch between these during the day because I have a very late-shifted natural clock and bright screens in the afternoon reinforce that, which is something I want to avoid.  And I just like to have a bit a variety in my themes.

The base is forked from [mediapathic's arsmagna
theme](https://github.com/mediapathic/obsidian-arsmagna-theme) because I like its layout and functionality.  Thorough commenting is added because I use css infrequently enough that I sometimes forget what it all means.  

For the light/dark file I've included some palette choices from [GuangluWu's pisum theme](https://github.com/GuangluWu/obsidian-pisum).

For the afternoon theme I used the settings from [Chad Bennett's warmth theme](https://github.com/chad-bennett/warmth-obsidian-theme)

For fun, the neon80's theme is remixed from [deathau's 80's Neon theme](https://github.com/deathau/80s-Neon-for-Obsidian.md)

I'm in the process of integrating [isanum's Nord theme](https://github.com/insanum/obsidian_nord) and [nickmilo's Cybertron theme](https://github.com/nickmilo/Cybertron/raw/master/obsidian.css) for more dark options.

## Making it work

I'm using two kinds of triggers to automate switching themes: time-of-day and voice commands.  You can do time-of-day triggers with Keyboard Maestro, and voice commands by turning on Voice Control in the Accessibility settings in System Preferences and creating new commands for each phrase you want to use.  

Neither of these talk to each other, but both can trigger an Automator workflow, so just create a workflow for each theme with the copy command to replace the obsidian.css file in your vault with the appropriate one in your theme folder, sosomething like:

```
cp /Users/yourusername/themes-folder/theme.css /Users/yourusername/obsidian-vault/obsidian.css
```

## Licence

It's licensed under [The Unlicense](./LICENSE).


