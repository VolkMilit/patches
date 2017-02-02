#Patches

I'm getting tired of trash can, that some programs try to do from my $HOME dir, so I started patch them to follow XDG. Anyway I have other patch for several programms. Maybe somebody will find them useful.						

###How to install patch:
On Debian (Stretch):														
$ apt source $package_name
$ sudo apt build-beb $package_name			
$ cd $package_name/src_or_smth					
$ patch < patchname.diff								
$ debuild -us -uc												
$ cd $directory_there_where_you_download_source		
$ sudo dpkg -i $package_name-smth.deb			

##XDG patches

####dosbox
Must follow XDG. There is only one config file, so store it in $HOME/.config/dosbox

####Emulationstation
Must follow XDG. Move all configs and themes in $HOME/.config/emulationstation

####pcsxr
Must follow XDG. Move configs in $HOME/.config/pcsxr. All bios, plugins, memcards, states in $HOME/.local/share/pcsxr

####prboom-plus
Must follow XDG. Move configs in $HOME/.config/prboom-plus

####Simple screen recorder
Must follow XDG. Move all configs in $HOME/.config/ssr

####UHexen
Need to fix something. BTW it's proprietary software, so I dunno, if that legal to publish this.												
~~Must follow XDG. Move all stuff to $HOME/.local/share/hexen2 and $HOME/.local/share/hexen2demo.

##Other patches

####Skippy-xd
Run one copy of the program at a time.

####st (Suckless terminal emulator)
- Fix unknow terminal by rename to xterm-256color		
- Add numix color palete									
- Default colls and rows are 140 and 46				

###TODO:
- Mednafen - can't read that pasta code. I found (maybe not), where is dotfiles is stored in code, but can't figure how can I fix that.
- FBReader - same as Mednafen. Cool structure of code, yep, but I just CANT find where dotfiles created\writed.
- QCalculator - there is two package depends of each other. I found, and fix the dots, but it's doesn't work.
- Audacity - todo
- QTCreator - todo
- Tux racer - todo
- GStreamer - todo
- vim - todo
- Firefox and Thunderbird - you know, right? There is was bug on bug-tracker, but nobody give a fuck about this. Especially Mozilla.		

Some shit-ware:
- RPM - I don't know, why that shitty absolutly proprietary Hamachi depends on rpm, but well... Maybe I just need to use tarball version. Fuck you, Hamachi!
- Steam - without comments. And, yeah, there is also: .steampid, .steampath, just wtf, Gaben?!
- lgp (Postal 2, I believe) - oh, yeah, that Running with scissors Postal 2, yeah... Fuck you too!
- Minecraft - why... Just why do you created that dotdir, even when I run you with HOME=blabla?! But how, just how? BTW dir is empty...
- Nvidia (.nv) - wtf? Even with export __GL_SHADER_DISK_CACHE_PATH="$HOME/.cache/nv" it continues creating this dir. (there goes middle finger of Linus)
- CLion and IDEA - no comments, bloody proprietary software.
