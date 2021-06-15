https://github.com/splewis/csgo-practice-mode/wiki/Overview-of-Commands
tokovoip ts3 na serwerze
General commands
.setup displays the practicemode menu
.help: displays this page
Saving grenade positions
.nades [player or category]: displays a menu to select saved grenade positions, this shows all frenades if no player or category is given
.cats : displays a menu of all saved grenades by category
.save <name>: saves your current position as a grenade spot with the given name
.goto [playername] <grenadeid>: teleports you to a player's saved grenade (or your own if no player is named)
.delete: deletes the last grenade of yours that you used .goto (or .nades) to teleport to
Modifying a saved grenade
All of the following commands can only be used on your grenades. They will apply to the last saved grenade you went to, whether by .save, .nades, or .goto.

.desc <description>: adds a grenade description to your last grenade
.rename <new name>: renames your last grenade
.addcat <category> ...: adds a category to your last grenade
.removecat <category>: removes a category from your last grenade
.clearcats: removes all categories on your last grenade
.deletecat <category>: removes a category from all of your saved grenades
.copy <username> <grenadeid>: copies another user's grenade and saves it for you
Testing grenades
.last: teleports you back to where you threw your last grenade from
.back: teleports you back a position in your grenade history
.forward: teleports you forward a position in your grenade history
.flash: saves you position to test flashbangs against it. Use this command in a spot you want to try to blind, then move and throw the flashbang; you will be teleported back to the position and see how effective the flashbang is
.stopflash: stops flash testing
Bot commands (new in 1.1.3+)
.bot: adds a bot where you're standing (or crouching!); .crouchbot to force a crouching bot
.botplace: adds a bot at the point you're looking at (similar to the bot_place command)
.boost: spawns a bot boosting you (crouch-boosting if you're crouching); .crouchboost to force a crouching bot
.movebot: moves the last bot you placed to your current position
.nobot: removes a bot you've added with .bot (can also use .kickbot or .removebot)
.nobots: clears all bots (.clearbots, .removebots, .kickbots also work)
Spawn commands
.spawn: same as .bestspawn (closest spawn)
.spawn <number>: teleports you to a spawn # for the maps's spawns
.namespawn <name>: saves the closest spawn to you under a name, which can then be gone to via .spawn <name>
.bestspawn: teleports you to your team's closest spawn from your current position
.worstspawn: teleports you to your team's furthest spawn from your current position
Miscellaneous
.timer: starts a timer when you start moving in any direction, and stops it when you stop moving, telling you the duration of time between starting/stopping
.timer2: starts a timer immediately and stops it when you type .timer2 again, telling you the duration of time
.fastfoward (or .ff): speeds up the server clock so the next 20 seconds lasts just 1 second
Client settings (cookies)
Clients can change some settings via sourcemod cookies.

practicemode_grenade_airtime: whether grenade airtime duration is shown
practicemode_flash_threshold: number of seconds a flash must last to be successful (when using .flash)
practicemode_testflash_delay: number of seconds after throwing a flash before being teleported (when using .flash)
These can be changed in console using sm_cookies <cookiename> <value>.

For example:

sm_cookies practicemode_grenade_airtime 1
sm_cookies practicemode_flash_threshold 2.0
sm_cookies practicemode_testflash_delay 0.3
