// Autoexec

// Settings
cl_autowepswitch "0"					// Disable auto weapon pickup
con_enable "1"						// Enable developer console
cl_clock_24hour "0"					// 24 hour time
lobby_default_privacy_bits1 "6"				// Lobby default privacy
mm_dedicated_search_maxping "80"			// Max ping for game search [Min = 50, Max = 350]

// Netgraph						// Shows netgraph with scoreboard
net_graph "1"
net_graphheight "9999"
bind "TAB" "+scorenet"
alias "+scorenet" "+showscores; net_graphheight 0"
alias "-scorenet" "-showscores; net_graphheight 9999"

// Crosshair
cl_crosshair_drawoutline "0.000000"
cl_crosshair_dynamic_maxdist_splitratio "0"
cl_crosshair_dynamic_splitalpha_innermod "1"
cl_crosshair_dynamic_splitalpha_outermod "1.000000"
cl_crosshair_dynamic_splitdist "5"
cl_crosshair_outlinethickness "1.000000"
cl_crosshair_sniper_show_normal_inaccuracy "0"
cl_crosshair_sniper_width "2"
cl_crosshair_t "0.000000"
cl_crosshairalpha "800.000000"
cl_crosshaircolor "5.000000"
cl_crosshaircolor_b "0.000000"
cl_crosshaircolor_g "0.000000"
cl_crosshaircolor_r "255.000000"
cl_crosshairdot "0.000000"
cl_crosshairgap "-2.000000"
cl_crosshairgap_useweaponvalue "0"
cl_crosshairscale "1000"
cl_crosshairsize "3.000000"
cl_crosshairstyle "4.000000"
cl_crosshairthickness "1.500000"
cl_crosshairusealpha "1"
cl_fixedcrosshairgap "3"

// Radar
cl_hud_radar_scale "1.1"				// Scale the physical radar
cl_radar_always_centered "0"				// Allows you to be on edge of map and see maximum distance
cl_radar_icon_scale_min "0.7"				// Scale the map icons
cl_radar_rotate "1"					// Rotate the rader so north is always where you are facing
cl_radar_scale "0.3"					// Scale the map inside the radar
cl_radar_square_with_scoreboard "1"			// Full map radar when scoreboard is open

// Video
mat_monitorgamma_tv_enabled "0"				// TV
mat_powersavingsmode "0"				// Power saving mode

// Audio
snd_musicvolume "0"					// Overall music volume
snd_menumusic_volume "0"				// Main menu

// HUD
cl_showhelp "0"						// Disable help
cl_autohelp "0"						// Disable help
gameinstructor_enable "0"				// Disable game hints
cl_loadout_colorweaponnames "1"				// Weapon names are colored in the weapon loadout to match their rarity
cl_hud_playercount_showcount "0"			// Mini-scoreboard style [0 = show player avatars, 1 = show count number, no avatars
ui_steam_overlay_notification_position "bottomright"

// Mouse
m_customaccel "0"					// Mouse acceleration off
m_customaccel_exponent "0"				// Acceleration amount
m_customaccel_max "0"					// Acceleration max
m_customaccel_scale "0"					// Acceleration scale
m_forward "1"						// Mouse forward factor
m_mouseaccel1 "0"					// Windows mouse acceleration initial threshold (2x movement)
m_mouseaccel2 "0"					// Windows mouse acceleration secondary threshold (4x movement)
m_mousespeed "0"					// Windows mouse acceleration
m_pitch "-0.022000"					// Mouse pitch factor
m_rawinput "1"						// Use raw mouse input
m_side "0.8"						// Mouse side factor
m_yaw "0.022"						// Mouse yaw factor
sensitivity "1"						// Sensitivity
zoom_sensitivity_ratio_mouse "1"			// Sensitivity is multiplied by this factor when the player zooms down the sight of a scoped weapon

echo "Majlund' CS:GO config loaded"			// Show that config is loaded

// Show damage top left (at end of round or death)
con_filter_text Damage Given To; con_filter_text_out Player:; con_filter_enable 2; developer 1;

// Persist
key_updatelayout;host_writeconfig;			// Makes sure the config is loaded properly
