# Installation

## Chrome
First you have to install the Stylebot extension. Then you have two options, choose whichever you prefer.

### Easy way
Go to http://stylebot.me/ and search for Wanikani Prettify.
If the style was found, there should be a button below it that you can click to install it.

The only disadvantage of this choice is that the style that is there might not be up to date with the one in this repository, but I'll try to keep it up to date.

### Slightly harder way
Open the extension's options page. Go to the Styles tab and click `Add a new style...`.
In the URL put `www.wanikani.com` and below paste the contents of the wanikani.css file.
Click Add and it's done!


## Other browsers
Waiting for someone to tell me how they're doing it. xD


# Customization
Open the extension's options page. Go to the Styles tab and click the `Edit Style`.
There you can add, change or delete styling rules. In the end just press `Save`.

All rules are commented, so even if you don't understand the syntax, you can still delete rules you don't like.
To do this, delete everything from the comment you don't like up to the next comment.

For example, if you wanted to remove the rules that replace the review background colors with weaker ones, you'd do the following.
Before:
```css
/* Remove review background pattern */
#reviews #character.radical,
#reviews #character.kanji,
#reviews #character.vocabulary {
    background-image: none;
}

/* Use weaker colors for review background so it hurts eyes less*/
#reviews #character.kanji {
    background: #E000A0;
}

#reviews #character.radical {
    background: #0090E0;
}

/* Improve review options readability */
#reviews #hotkeys {
    font-weight: bold;
    color: #777777;
}
```

After:
```css
/* Remove review background pattern */
#reviews #character.radical,
#reviews #character.kanji,
#reviews #character.vocabulary {
    background-image: none;
}

/* Improve review options readability */
#reviews #hotkeys {
    font-weight: bold;
    color: #777777;
}
```
