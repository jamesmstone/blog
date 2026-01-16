---
id: 193
title: 'IFTTT: Spotify playlist to Dropbox'
author: James Stone
layout: post
guid: http://blog.jamesst.one/?p=193
permalink: /2013/11/ifttt-spotify-playlist-dropbox/
categories:
  - IFTTT
---
[New Version now available](/2015/02/ifttt-spotify-playlist-dropbox-version-2/)

* * *

This is a post about an IFTTT recipe I made. Not sure what [IFTTT is][2]?

## What this recipe does

These recipes download the songs in your Spotify Playlist via Last.fm Free Music and Soundcloud downloadable tracks. The tracks at these sites have been submitted by the artist and been marked as free and downloadable for the public.

## Recipes

**What&#8217;s the difference?** *Download only exact matches* only does steps 1 to 3 of *How it Works  *Below. As such it is very limiting (it only gets the exact song).

### Download only exact matches (source Last.fm Free Music)

Save to box  
<a id="embed_recipe-126747" class="embed_recipe embed_recipe-l_83" href="https://ifttt.com/view_embed_recipe/126747" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126747" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Box #free #music #Exact" width="370px" /></a>

Save to dropbox

<a id="embed_recipe-126750" class="embed_recipe embed_recipe-l_87" href="https://ifttt.com/view_embed_recipe/126750" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126750" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Dropbox #free #music #Exact" width="370px" /></a>  
Save to google drive  
<a id="embed_recipe-126748" class="embed_recipe embed_recipe-l_91" href="https://ifttt.com/view_embed_recipe/126748" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126748" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #googledrive #free #music #Exact" width="370px" /></a>

save to skydrive

<a id="embed_recipe-126749" class="embed_recipe embed_recipe-l_88" href="https://ifttt.com/view_embed_recipe/126749" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126749" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Skydrive #free #music #Exact" width="370px" /></a>

### Download all (Source Last.fm Free Music and Soundcloud)

Save to box  
<a id="embed_recipe-126754" class="embed_recipe embed_recipe-l_81" href="https://ifttt.com/view_embed_recipe/126754" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126754" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Box #free #music #all" width="370px" /></a>

Save to dropbox

<a id="embed_recipe-126753" class="embed_recipe embed_recipe-l_85" href="https://ifttt.com/view_embed_recipe/126753" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126753" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Dropbox #free #music #all" width="370px" /></a>  
Save to google drive  
<a id="embed_recipe-126752" class="embed_recipe embed_recipe-l_89" href="https://ifttt.com/view_embed_recipe/126752" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126752" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #googledrive #free #music #all" width="370px" /></a>

save to skydrive

<a id="embed_recipe-126751" class="embed_recipe embed_recipe-l_86" href="https://ifttt.com/view_embed_recipe/126751" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126751" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Skydrive #free #music #all" width="370px" /></a>

## Set up Instructions

  1. In Spotify right click on your playlist and select *Copy Spotify URI * then go to the desired recipe 
    
      * ![How to Copy Spotify URI](/post_assets/Screenshot-2013-11-06-17.29.24.png) How to Copy Spotify URI
      * Then go to the desired recipe (*links above*)
      * In the URL field paste your *Spotify URI *after the `=` sign ( or you can leave it as  *spotify:user:spotify:playlist:4hOKQuZbraPDIfaGbM3lKI* for [Top 100 tracks currently on Spotify][3] playlist ) 
      * ![Paste the Spotify URI after the &quot;=&quot; sign](/post_assets/Screenshot-2013-11-06-18.23.19.png) Paste the Spotify URI after the `=` sign

## How it works
        
 1. Yahoo pipes checks your spotify playlist
 2. Then song by song it checks to see if the song is available legally for free from Last.fm
 3. If it is Yahoo Pipes tells IFTTT to add it to your dropbox or equivilent.
 4. If it isn&#8217;t Yahoo Pipes searches Soundcloud for the songs title and artist and then downloads the first *downloadable* song. This is why remixed version are often downloaded.
        
## <del>Update: Issues</del>
        
<del>The recipes will still work, however the recipes aren&#8217;t triggered as frequently as they should be. [<a title="Update: Spotify playlist to Dropbox" href="/2013/11/update-spotify-playlist-dropbox/">Details</a>]</del>
        
Fixed [[Details][4]]
        
## Other IFTTT recipes
        
  * I recently made a post about how I use IFTTT -*[interested][5]?*
  * <a href="https://ifttt.com/p/jamesmstone" target="_blank">My Public IFTTT Profile</a>
        
## Help
        
Need help? Have a suggestion? Please leave a comment

 [1]: /2015/02/ifttt-spotify-playlist-dropbox-version-2/ "IFTTT: Spotify playlist to Dropbox – Version 2"
 [2]: /2013/11/ifttt/ "Why you should use IFTTT?"
 [3]: spotify:user:spotify:playlist:4hOKQuZbraPDIfaGbM3lKI
 [4]: /2013/11/update-spotify-playlist-dropbox/ "Update: Spotify playlist to Dropbox"
 [5]: /2013/11/my-ifttt-recipes/ "How I use IFTTT"