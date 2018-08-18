# custom-playback-loop

## DOCUMENTATION

#### Purpose:
You set the time you want to loop a youtube video!

#### Clarification: #### 
While I use the words "hack" in my code, this is by no means a hack. Just a simple, personal solution to a problem I faced.

#### Steps:
(These steps are only applicable for youtube! For other pages follow the other pages step before you do these)
1. Download the `custom loop (youtube).txt` file
2. Set the `hack` variables (hackMin, hackRMin, etc.) that are right on top of the file.
3. Copy & paste the new code onto your browser's `console` (for chrome, right click->inspect->change tab to console->paste)
4. Hit `enter` and enjoy!

#### Other Pages:
1. Open developer tools on chrome
2. Use `Select an element on this page to inspect it` on the top-left side of the dev tools
3. Hover over the video till the whole video is highlighted, and click on it. You'll be shown the corresponding webpage code.
4. If the corresponding code is in this format `<video ...someText...>...moreText...</video>` this code will work :), otherwise you're out of luck :(
5. Right click and select `add attribute`
6. Type the following `id="myCustomName"` (**don't use spaces in your name**)
7. Replace every instance of `document.getElementsByClassName("someClassName")` with `document.getElementByID("myCustomName")`
8. Now follow the regular steps and enjoy!
  
#### Drawbacks/Warnings:
- You need to paste the code everytime you reload the page. These are edits you make to the local copy of the website. Each reload loads the website from Youtube, which does not store the edits you made.
- The code uses class names to identify your video. If youtube ever changes that in the future this code may be useless. In the same manner this code is useless on pages other than youtube.
