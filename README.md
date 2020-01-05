# i3 Configuration Notes

## January 2020 - i3-gaps

Having seen references to i3-gaps (a fork of the i3 I was already
using), I decided to try it.

The process required two stages. The first was to install the i3-gaps
functionality. I already had a working i3, so the change was carried
out using the script here:

https://www.reddit.com/r/unixporn/comments/5rw91n/i3gaps_my_installscript_for_i3gaps/

You have to run it as sudo. Otherwise, it works as expected.

Once i3-gaps is installed you can start adding configuration
instructions as required. The first thing you need is to switch off
the title bars of the windows. I'm not sure whether I like this, and I
may end up going back to i3 just because of this... We'll see.

The relevant code to add to the i3 configuration file is:

for_window [class="^.*"] border pixel 2

The border width is added to the active window when there is more than
one window on a desktop.

The initial gaps are then set using:

gaps inner 10
gaps outer 5

This produces a gap that the wallpaper can then be seen through. It is
a pleasing effect, though, as I say, I'm not sure I will stick with
it...

The final configuration I added was to have smart borders active:

smart_borders on
