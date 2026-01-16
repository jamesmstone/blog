---
id: 1105
title: 'IFTTT: Spotify playlist to Dropbox &#8211; Version 2'
author: James Stone
layout: post
guid: http://blog.jamesst.one/?p=1105
permalink: /2015/02/ifttt-spotify-playlist-dropbox-version-2/
switch_like_status:
  - 1
categories:
  - IFTTT
---
This is a post about an IFTTT recipe I made. Not sure what [IFTTT is](/2013/11/ifttt/) ?

Unfortunately for sometime now [version 1](/2013/11/ifttt-spotify-playlist-dropbox/) of these recipes hasn&#8217;t been working.
Now that I have some more time on my hands I have decided to fix it.

## Improvements

  * It now works again!
  * Its quicker than version 1
  * Works more reliably.

## Disadvantages

  * Only works for the first 100 songs in playlists with more the 100 songs

## Technical differences between versions

<table class="table table-striped table-bordered">
  <tr>
    <th>
    </th>
    
    <th>
      Version 1
    </th>
    
    <th>
      Version 2
    </th>
  </tr>
  
  <tr>
    <th>
      Backend
    </th>
    
    <td>
      <ul>
        <li>
          Yahoo Pipes
        </li>
      </ul>
    </td>
    
    <td>
      <ul>
        <li>
          PHP ( I now know PHP :D )
        </li>
        <li>
          Memcache
        </li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <th>
      APIs used
    </th>
    
    <td>
      <ul>
        <li>
          Last Fm
        </li>
        <li>
          Soundcloud
        </li>
        <li>
          Spotify (Unofficial through webpage scrapping)
        </li>
      </ul>
    </td>
    
    <td>
      <ul>
        <li>
          Last Fm
        </li>
        <li>
          Soundcloud
        </li>
        <li>
          Spotify (Official)
        </li>
      </ul>
    </td>
  </tr>
</table>


## Upgrading to new version

Nothing should need to be changed when upgrading from the previous version.

## Using New Version

### What this recipe does

These recipes download the songs in your Spotify Playlist via Last.fm Free Music and Soundcloud downloadable tracks. The tracks at these sites have been submitted by the artist and been marked as free and downloadable for the public.

### Recipes

**What&#8217;s the difference?** *Download only exact matches* only does steps 1 to 3 of *How it Works  *Below. As such it is very limiting (it only gets the exact song).

#### Download only exact matches (source Last.fm Free Music)

Save to box

<a id="embed_recipe-126747" class="embed_recipe embed_recipe-l_83" href="https://ifttt.com/view_embed_recipe/126747" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126747" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Box #free #music #Exact" width="370px" /></a>

Save to dropbox

<a id="embed_recipe-126750" class="embed_recipe embed_recipe-l_87" href="https://ifttt.com/view_embed_recipe/126750" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126750" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Dropbox #free #music #Exact" width="370px" /></a>

Save to google drive

<a id="embed_recipe-126748" class="embed_recipe embed_recipe-l_91" href="https://ifttt.com/view_embed_recipe/126748" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126748" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #googledrive #free #music #Exact" width="370px" /></a>

save to skydrive

<a id="embed_recipe-126749" class="embed_recipe embed_recipe-l_88" href="https://ifttt.com/view_embed_recipe/126749" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126749" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Skydrive #free #music #Exact" width="370px" /></a>

#### Download all (Source Last.fm Free Music and Soundcloud)

Save to box

<a id="embed_recipe-126754" class="embed_recipe embed_recipe-l_81" href="https://ifttt.com/view_embed_recipe/126754" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126754" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Box #free #music #all" width="370px" /></a>

Save to dropbox

<a id="embed_recipe-126753" class="embed_recipe embed_recipe-l_85" href="https://ifttt.com/view_embed_recipe/126753" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126753" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Dropbox #free #music #all" width="370px" /></a>

Save to google drive

<a id="embed_recipe-126752" class="embed_recipe embed_recipe-l_89" href="https://ifttt.com/view_embed_recipe/126752" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126752" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #googledrive #free #music #all" width="370px" /></a>

save to skydrive

<a id="embed_recipe-126751" class="embed_recipe embed_recipe-l_86" href="https://ifttt.com/view_embed_recipe/126751" target="_blank"><img src="https://ifttt.com/recipe_embed_img/126751" alt="IFTTT Recipe: auto #Download the new songs in a #Spotify playlist  to my #Skydrive #free #music #all" width="370px" /></a>

## Set up Instructions

  1. In Spotify right click on your playlist and select *Copy Spotify URI
  
     ![How to Copy Spotify URI](/post_assets/Screenshot-2013-11-06-17.29.24.png)
     
     How to Copy Spotify URI

    
      * Then go to the desired recipe (*links above*)
      * In the URL field paste your *Spotify URI *after the &#8220;=&#8221; sign 
        
     ![Paste the Spotify URI after the &quot;=&quot; sign](/post_assets/Screenshot-2013-11-06-18.23.19.png)
          
     Paste the Spotify URI after the &quot;=&quot; sign    
        
     * In order for the script to work the feed url you just completed in step 3 needs to be loaded once ( without IFTTT) so copy the complete feed url from IFTTT and paste it into your browser</ol> 
        
## How it works
        
  1. The script checks your Spotify playlist
  2. Then song by song it checks to see if the song is available legally for free from Last.fm
  3. If it is the script tells IFTTT to add it to your Dropbox or equivalent.
  4. If it isn’t the script searches Soundcloud for the songs title and artist and then downloads the first *downloadable* song. This is why remixed version are often downloaded.
        
## Other IFTTT recipes
  
  * I made a post about how I use IFTTT -*[interested][3]?*
  * [My Public IFTTT Profile](https://ifttt.com/p/jamesmstone)
        
## Help
        
Need help? Have a suggestion? Please leave a comment
        
Note: I&#8217;m still working on the *Download all (Source Last.fm Free Music and Soundcloud)* version Soundcloud API issues so  for now the  *Download all* version is working like the *exact* version, but that is soon to change.
        

 [1]: /2013/11/ifttt/ "Why you should use IFTTT?"
 [2]: /2013/11/ifttt-spotify-playlist-dropbox/ "IFTTT: Spotify playlist to Dropbox"
 [3]: /2013/11/my-ifttt-recipes/ "How I use IFTTT"
