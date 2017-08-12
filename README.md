# Art Book, an EmulationStation theme (WIP)
A simple theme for Emulation Station and RetroPie based around the look of a coffee table book.  
Discussion ongoing in this thread: https://retropie.org.uk/forum/topic/11728/new-theme-art-book

## Preview

### Screenshots

*Detailed View*
![Detailed View](http://i.imgur.com/45WMfc3.png)

*Video View*
![Video View](http://i.imgur.com/rjfopnF.png)

*Basic View*
![Basic View](http://i.imgur.com/YH4oAci.png)


## Details

- Has support for system, basic, detailed and video views
- Support for new All Games, Favorites, Recently Played and Custom Collections in latest version of Emulation Station
- Displays the following metadata on detailed and video views: rating, description, # of players, genre, publish date & last played
- 16x9 resolutions only (tested at 1280x720 and 1920x1080)
- Layout designed to support hardware accelerated OMX player on video views
- Has SMB (Super Mario), TLOZ (Legend of Zelda) and Megaman custom systems

## Acknowledgments

- Some game console logo graphics are modified from the Carbom theme by Eric Hettervik
- ChangaOne font by Eduardo Tunni

## Scraping

### Arcade

- First Scrape Flyers (from GDB): /opt/retropie/supplementary/scraper/scraper -mame=true -mame_src=gdb,adb,ss -mame_img=fly,b,t,s -max_height=540 -max_width=394 -image_dir=media -image_path=media

- Then Scrape Videos and Marquees (from SS): /opt/retropie/supplementary/scraper/scraper -mame=true -mame_src=ss,gdb,adb -download_videos=true -download_marquees=true -image_dir=media -image_path=media -video_dir=media -video_path=media -marquee_dir=media -marquee_path=media

### Console

- Run this command in a system's folder (i.e. /roms/nes): /opt/retropie/supplementary/scraper/scraper -console_src=ss -max_height=540 -max_width=505 -download_videos=true -download_marquees=true -image_dir=media -image_path=media -video_dir=media -video_path=media -marquee_dir=media -marquee_path=media -use_nointro_name=false 

### Game & Watch

- Run this command in the /roms/gameandwatch folder: /opt/retropie/supplementary/scraper/scraper -console_src=ss -console_img=clabel,b,s -img_format=png -max_height=540 -max_width=505 -image_dir=media -image_path=media
