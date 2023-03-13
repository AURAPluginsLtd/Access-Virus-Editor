**Version 3.0.0 build 9033 / 2023-Mar-13**

- **(fixed)** Resolved issue where legacy patch data was not loaded properly when Virus TI was chosen as active model.
- **(fixed)** Resolved issue where Mod Matrix Distortion Mix destination was not working.
- **(fixed)** Resolved issue where selected bank character was incorrect.
- **(fixed)** Resolved Pro Tools crash when removing Editor with MIDI I/O set.
- **(fixed)** Automation works from Editor itself, external midi controller or from hardware itself.
- **(fixed)** Resolved issue where arp mode didn't work as expected.
- **(fixed)** Resolved issue where global arp switch didn't work as expected.
- **(fixed)** Resolved issue where disabling / enabling global EQ displayed EQ parameters on top of Multimode Mixer view.
- **(fixed)** Resolved issue where User Interface was not drawn properly on different screen sizes.
- **(fixed)** Resolved issue where filter 1 mode was always set to LP on Virus A, Virus Rack and Virus B.
- **(fixed)** Some list items displayed wrong value in User Interface.
- **(fixed)** Resolved issue where onscreen keyboard was not shown even when it was toggled on after closing the editor window.
- **(fixed)** Resolved issue where user interface scaling didn't work as expected on smaller displays (i.e. macbooks with 13-inch display).
- **(fixed)** Resolved issue where MIDI I/O was not recalled as expected after updating the MIDI framework.
- **(new)** Sliders can be set to snap on mouse position or adjust freely from clicked position.
- **(new)** Category browsing can be limited to currently active bank from Editor Preferences menu.
- **(new)** User can now sync single part from hardware to Editor with Sync Data from HW button when main TAB is not set to MULTIMODE MIXER view.
- **(new)** Added function that will display a new window if Total Recall is interrupted while Session & Editor are loading.
- **(new)** Disable Total Recall function added to Editor Preferences menu.
- **(new)** Randomizer can now be limited to randomize active TAB content only, ie. Effects 1. This option has been added to Editor Preferences menu.
- **(new)** Multimode mixer key range controls now show as a menu when clicked. Same applies to Filter Key Follow Base. 
- **(improvement)** PC Standalone App MIDI I/O Dropdown menus are now wider.
- **(improvement)** Request interval is now automated. All patch writing is clocked between 500ms intervals.
- **(improvement)** MIDI Message handling adjusted.
- **(improvement)** When global keyboard or control mode is off, data gets sent to hardware more efficiently.

**Version 3.0.0 build 9024 / 2022-Oct-07**

- **(fixed)** Resolved issue where plugin was not found after updating to build 9022.
- **(fixed)** Resolved issue where predefined model was not applied accordingly.

**Version 3.0.0 build 9022 / 2022-Sep-30**

- **(new)** Demo version ships with USB MIDI Driver for macOS Users.
- **(new)** Added option in Utilities menu to limit search on active bank.
- **(new)** Added option in Utilities menu to show search results containing search term.
- **(new)** Added option in Utilities menu to set default skin (use only if you have one Virus).
- **(new)** Added option in Utilities menu to set default model (use only if you have one Virus).
- **(new)** Added option in Utilities menu to load HiRes graphics if needed - Uses more RAM.
- **(new)** Added option in Utilities menu to route all incoming MIDI data to currently active part (when DAW is stopped).
- **(new)** Advanced MIDI Filters page has option for Randomizer Target - All / Excluding Pitch.
- **(fixed)** Softknobs were set to global mode - They work again as expected.
- **(fixed)** Pitch Bender, Modulation Wheel and Note input from Virus Keyboard models work as expected.
- **(fixed)** Draw and control issues of Delay and Reverb on Effects #1 sorted.
- **(fixed)** Resolved issue where TI was set to USB mode when MIDI Dins were used.
- **(fixed)** If data was received from channel 1 and part 2-16 had MIDI channel set to 1, data was not processed.
- **(fixed)** Writing Single Patches to hardware works as expected.
- **(fixed)** Bank Edit menu items didn't update accordingly in some cases.
- **(fixed)** FM Amount was recalled to zero in some cases.
- **(fixed)** Search input was not able to take in @ sign.
- **(fixed)** Editor went to Device ID check loop before it was supposed to.
- **(improvement)** Requesting data from hardware takes less time now (with MIDI Din connectors).
- **(note)** Virus TI users: If you use USB connection, it is much slower than using MIDI Dins. We recommend setting up a soundcard and MIDI interface for Editor use.

**Version 3.0.0 build 9019 / 2022-Aug-18**

- **(fixed)** USB Audio Mode should be recalled properly now and values set accordingly.
- **(fixed)** Virus TI Reverb was incorrectly set when data was read from patch and when data was sent to hardware.
- **(fixed)** Virus TI Global settings we recalled incorrectly.
- **(fixed)** Windows installer now works as expected even with custom install.
- **(fixed)** macOS installer now works as expected.

**Version 3.0.0 build 9015 / 2022-May-12**

- **(new)** If new update is available, a button is shown above the Logo instead of popup window.

**Version 3.0.0 build 9013 / 2022-May-08**

- **(fixed)** Resolved issue where Virus TI was forced to USB mode even when regular MIDI Dins were used.
- **(fixed)** Resolved issue where deviceID scope did not check for omni value.

**Version 3.0.0 build 9011 / 2022-April-25**

- **(new)** AURA Plugins Ltd is now taking over Mystery Islands Music to continue developing great Editor & Librarian products for years to come. Product URLs will be updated soon.
- **(new)** Adjust how many USB output stream Virus TI will output (macOS only).
- **(new)** Surround output for TI now includes USB outputs as well (macOS only).
- **(new)** Included Guide how to get USB data stream working in macOS 10.12 or greater.
- **(fixed)** Resolved issue where TI with Device ID omni was not found.
- **(fixed)** Resolved issue where TI Delay Time knob was missing when Tape Free or Doppler was chosen.
- **(fixed)** Resolved issues with TI Reverb modes.

**Version 3.0.0 build 9003 / 2022-April-17**

- **(fixed)** Resolved issue with Windows installer and Plugin / Application not able to run.

**Version 3.0.0 build 9001 / 2022-April-13**

IMPORTANT: This version is not backwards compatible. Backup "access virus editor.vst/component/app/exe/vs3/dll" before installing build 9001!

- **(new)** Virus TI users can now use USB Audio stream with macOS. More details here: https://docs.auraplugins.com/kb/article/virus-ti-usb-audio-with-every-macos/

**Version 3.0.0 build 8841 / 2022-April-08**

- **(fixed)** Resolved issue where plugin would crash if LEDs were enabled.
- **(improvement)** Consuming less CPU when user interface is open.

**Version 3.0.0 build 8838 / 2022-March-25**

- **(new)** If bank contains data which has Access Virus header in it, but the data is too small per Virus model standards, it will be ignored and initialized for safety reasons.
    This might remove some patches from the bank, but it allows user to open banks which are corrupted for some reason.
    Backup your banks before installing!

**Version 3.0.0 build 8836 / 2022-March-25**

- **(fixed)** Resolved issue where patches were loaded to part 1 only.

**Version 3.0.0 build 8834 / 2022-March-23**

- **(fixed)** Resolved issue which caused crash when setting MIDI I/O.
- **(fixed)** Resolved issue which caused constant time out messages.

**Version 3.0.0 build 8832 / 2022-March-22**

- **(new)** Added missing Ableton Live guide.
- **(fixed)** Resolved issue where Sync Data from HW did not work as expected.
- **(fixed)** When using USB on macOS, time out window is longer.
- **(improvement)** Data requests work faster.
- **(improvement)** Data sending work faster.

**Version 3.0.0 build 8830 / 2022-March-21**

- **(new)** Access Virus Editor User Manual included in PDF format.
- **(new)** All manual shortcuts are now available in Utilities menu.
- **(new)** If debug is enabled, "LOGGING ENABLED" text will appear under the product logo.
- **(fixed)** Resolved issues with Delay, Reverb and Osc Sync parameters across all models.
- **(fixed)** When bank has unsaved changes, it won't change upper bank on part change.
- **(fixed)** Upper bank view won't show unsaved changes unless the bank content is really changed.
- **(fixed)** Mod Matrix and LFO2 destination pop-up menus fixed.
- **(fixed)** Submit Support Ticket now takes user to proper URL.
- **(improvement)** Changed the way how timeout is handled while waiting for System Exclusive transfers.
- **(improvement)** Cleaned Patch Librarian "other helpful things" -menu.
- **(other)** Small Virus TI Snow model specific updates.

**Version 3.0.0 build 8825 / 2022-March-10**

- **(new)** Full version now includes USB driver for Virus TI users. Users with macOS 10.15 and beyond can now connect to "Virus TI USB Plugin I/O" with Virus TI USB. (yes, Big Sur and Monterey users as well). Audio has to be routed from Virus to sound card or console, but we are investigating...
    Addendum: USB seems to be very slow, so if you have MIDI device, use that instead!

- **(fixed)** Resolved issue where MIDI data was not properly handled causing continuous Device ID checks.
- **(fixed)** Resolved issue where bank edit indicator did not display when requesting data from hardware to librarian.

**Version 3.0.0 build 8823 / 2022-March-09**

- **(fixed)** Resolved issue where plugin would crash when clicking "Push Data To HW" in some cases.
- **(fixed)** Resolved issue where plugin would crash when parameter was changed and LED tracking was set for outgoing MIDI data.
- **(fixed)** Resolved issue where Bank Edit Menu button was not functioning under certain circumstances.

**Version 3.0.0 build 8821 / 2022-March-06**

- **(other)** This version might be incompatible with previous version save-state.

- **(new)** Plugin now has multichannel MIDI input channels available in Pro Tools.
- **(new)** Effects are no longer available in the plugin / app when they are set to disabled (delay, eq, reverb and arp).
- **(new)** User Interface LEDs can be disabled from the bottom bar. This function replaced "menu 2" function.
- **(fixed)** Channel routing inside the plugin and app should work as expected, even with remote keyboards.
- **(fixed)** Resolved issue where some Mod Matrix destinations didn't work as expected.
- **(improvement)** Reduced plugin CPU load.
- **(improvement)** Graphics improvements.

**Version 3.0.0 build 7556 / 2022-January-30**

- **(new)** Bottom bar has new option to "AutoSave" changes made in Patch Librarian to upper bank. Use with caution.
- **(new)** Randomizer Trigger with MIDI CC. User can now define which incoming MIDI CC will trigger randomizer. Setting adjustable in Advanced MIDI Settings tab. Only applies if MIDI CC comes from DAW or Remote Input (standalone app).
- **(new)** Randomizer Percentage. User can now define in percentage how much Randomness takes place when triggered. Setting adjustable in Advanced MIDI Settings tab.
- **(fixed)** Resolved issue where bank disappeared after "bank edit menu" -> "overwrite bank".
- **(fixed)** Resolved issue where program up and down buttons did not work as expected.
- **(fixed)** Resolved issue where Section Locks did not work as expected.
- **(fixed)** Section Locks now indicate ON and OFF status when toggled on or off.
- **(fixed)** When changing Reverb Mode from Virus TI, Reverb Mode should now reflect to proper value in the editor.
- **(improvement)** MIDI initialization commands are now sent to hardware if MIDI output is connected and model is changed afterwards.
- **(improvement)** Download links now point to direct download page. Remember to login for FULL version access.

**Version 3.0.0 build 7554 / 2022-January-28**

- **(new)** Windows installer is now signed.
- **(fixed)** Resolved issue where macOS was not able to read Patches data nor the license file.
- **(improvement)** On Screen Keyboard now responses to hardware and DAW note messages.

**Version 3.0.0 build 7552 / 2022-January-27**

- **(new)** Native 64-bit AAX for Windows included in the installer. (macOS AAX was out already).
- **(fixed)** Open Data Folder did not open proper location on Windows.
- **(fixed)** Patch Librarian bank menu items are now shown correctly if folder has subfolders.
- **(fixed)** Bank Overwrite and Save As no longer removes file from Patches folder.
- **(fixed)** Resolved issue where plugin / app would crash under certain circumstances if lower bank selection was triggered.
- **(improvement)** Mod Matrix and LFO Destinations are now broken down to groups and lists are alphabetically ordered.
- **(improvement)** Removed logging completely from Release build to avoid clicks in audio engine.

**Version 3.0.0 build 7020 / 2022-January-12**

- **(new)** Less clicking when recalling a project: Main tab and Quick tab values are stored within project.
- **(fixed)** When dragging and dropping patches between slots, name is now shown in the drag box.
- **(fixed)** Shortcut in Windows startup menu fixed for Editor executable.
- **(fixed)** Patch Librarian "Save Part Data To Slot" button was not behaving as expected when dropping patch from bottom list to top list.
- **(fixed)** Fixed macOS installer error further.
- **(improvement)** Selected Librarian Banks per part are now automatically stored and recalled as expected.
- **(improvement)** If Application or Plugin is exiting while tasks are running, tasks are terminated to quit faster.
- **(other)** Total Recalling projects prior to build 7020 might show some weird behavior.
- **(other)** Removed deep debugging. No more clicks and crackles when using the plugin.

**Version 3.0.0 build 7018 / 2022-January-09**

- **(new)** Star sign is shown in the Main Tab next to "PATCH LIBRARIAN" if bank has unsaved changes.
- **(new)** If bank contains TI and classic patches, bank is converted to TI bank. Classic models can still load these presets without TI functions.
- **(new)** Check if MIDI ports are free to use. If port cannot be opened, warning message will appear, instead of hard crash.
- **(fixed)** Resolved issue where importing banks did not work if bank was not fully loaded with single patches. Now import works even if bank has one patch in it.
- **(fixed)** Resolved issue where storing banks did not work as expect when bank contained data from classic and TI models.
- **(fixed)** Resolved issue where writing data to current bank & patch combination did not work as expected.
- **(fixed)** Resolved issue where DAW would crash when removing plugin from track and then adding it back in again in some cases.
- **(fixed)** Oscillator Phase Init knob was not available when Unison Mode was set to OFF.
- **(fixed)** Resolved macOS Installer error ...

**Version 3.0.0 build 7016 / 2022-January-05**

- **(fixed)** Resolved issue where 0xf8 and 0xfe were passed through even when they were set to OFF. This should eliminate "connection error" issues all together.

**Version 3.0.0 build 7014 / 2022-January-04**

- **(other)** Improved data handling when setting MIDI input and output. Initial commands are now sent to output port before checking if the device is present.

**Version 3.0.0 build 7012 / 2022-January-02**

- **(fixed)** Wrong MIDI out port was called when setting MIDI output port on Windows.
- **(other)** External MIDI Sense is set to be ignored. Might add option to filter midi sense and midi clock messages directly from advanced midi settings.
- **(other)** Extended logging system for development purposes. Send the plugin log file from /Music/AURA Plugins/Access Virus Editor/ folder to support@auraplugins.com with steps how to reproduce the issue. Thank you!

**Version 3.0.0 build 7001 / 2021-December-25**

- **(new)** First UNTESTED Windows release candidate. (I was not able to test this during Christmas, but I will be testing it out with my Viruses in the upcoming days).

**Version 3.0.0 build 6967 / 2021-December-19**

- **(fixed)** Resolved issue where Delay FX mode was not working as expected when model was Virus TI or TI Snow.
IN PROGRESS - **(fixed)** Resolved issue where plugin and application did not start if macOS is below 10.13.

**Version 3.0.0 build 6963 / 2021-December-15**

- **(new)** Remote input port added for Standalone Application. Use this port to send notes / control hardware with external controller.
- **(new)** macOS 10.9 (64-bit) or greater required. Metal framework is no longer required.
- **(new)** plugin ID changed so that it can be ran alongside v1.x or v2 to migrate settings on new version.
- **(new)** Option to disable Total Recall in cases where editor is attended to be used "on the go". User has to sync data from HW each time the editor is loaded to get the HW data to SW. This setting is in Advanced MIDI Settings page.
- **(fixed)** Virus OS version is now set properly during total recall. (latest VirusOS is required per model).
- **(fixed)** MIDI Input and MIDI output tooltips were showing wrong tooltip.
- **(fixed)** Resolved issue where plugin / app would crash when toggling between banks (with - and + buttons).
- **(fixed)** Resolved issue where pan pot did not update the multimode / quick mixer pan levels as expected.
- **(fixed)** Resolved issue where plugin or application would crash if MIDI clock was running while exiting host.
- **(fixed)** Resolved issue where plugin would crash during total recall / push data to hw was triggered with TI selected as a model.
- **(fixed)** Resolved issue where Keyboard tab Mod Wheel and Pitch Bender did follow incoming MIDI as expected.
- **(fixed)** Resolved issue where plugin got stuck while making total recall when TI Snow was chosen model.

**Version 3.0.0 build 6949 / 2021-December-13**

- **(new)** Warning dialog will appear if
  a) user attempts to write data from librarian to hardware.
  b) user attempts to connect midi output before midi input.
  c) memory protect is enabled.
- **(new)** Global LED settings added to FX / Settings #2 tab as well as Memory Protect menu. LCD contrast on legacy models apply only when globals are sent to hardware.
- **(new)** Virus TI models are now forced into multi mode when when data is recalled or when plugin is initialized.
- **(fixed)** Resolved issue where global -> midi clock on legacy models was not working as expected.
- **(fixed)** Resolved issue where global -> midi destination on legacy models was not working as expected.
- **(fixed)** Resolved issue where global input settings were not applied / recalled on legacy models.
- **(fixed)** Resolved issue where master tuning and keyboard aftertouch sensitivity controls did not display value as expected.
- **(fixed)** Resolved issue where plugin could potentially cause feedback loop.
- **(fixed)** Resolved issue where all settings were initialized if MIDI out port was not present during recall.

**Version 3.0.0 build 6943 / 2021-December-11**

- **(new)** When part is changed, plugin / application display will show the current value.
- **(fixed)** Resolved issue where part 1 button remained active at multimode mixer page when part was changed.
- **(fixed)** Resolved issue where save and load UI Data and CC Maps was pointing to wrong location.
- **(fixed)** Resolved issue where Logic Pro did not show the plugin User Interface on initialization.
- **(fixed)** Resolved issue where VST3 had only one MIDI input channel instead of 16.
- **(improvement)** Virus OS type specifier improvements. Now OS is tied to specific model selection. We expect user to have latest available OS installed in their Virus to use the plugin / application the way it is expected to work.

**Version 3.0.0 build 6932 / 2021-December-08**

- **(new)** Patch Librarian can now export "classic" banks to TC Electronic Virus|PowerCore compatible format. Patch Librarian -> Bank Edit Menu -> Save As ... -> Virus|Powercore.
- **(fixed)** Resolved issue where User Interface was downscaled even when there was room to display it in full scale.

**Version 3.0.0 build 6923 / 2021-December-05**

- **(new)** Native Apple Silicon support for Standalone Application and Plugins *.
- **(new)** Apple Silicon forced us to change the data folder structure completely. You can find all plugin / application related files as follows;
    (Patches): "/Library/Mystery Islands Music/Presets/Access Virus Editor/Patches/".
    (CC Maps): "/Library/Mystery Islands Music/Presets/Access Virus Editor/CC Maps/".
    (UI Data): "/Library/Mystery Islands Music/Presets/Access Virus Editor/UI Data/".
    (License and LOG file): "/Library/Mystery Islands Music/Access Virus Editor/".
- **(new)** If plugin or application fails to load license, user can initiate license loading dialog from the top left corner of our plugin / application.
- **(new)** Plugin / Application window will be automatically resized if it will not fit to current display.
- **(fixed)** Update checker did not work as expected.
- **(fixed)** Standalone Application menu titles shown as they should.
- **(fixed)** Using "Menu 2" for Application / Plugins now has scrolling option if menu draw area exceeds the display area.

* We are waiting for Pro Tools Native M1 support to arrive so we can include M1 AAX version.

**Version 3.0.0 build 6895 / 2021-November-27**

- **(new)** Extended tooltips. Once mouse is hover over the control, a popup will appear with explanation of the control function. Previously user could only see the control value and name in the plugin / app display.
- **(new)** Completely rewrote partition of the code which handles the patch and multi renaming. No more waiting of data transfers after renaming.
- **(fixed)** Reverb Feedback value was not recorded properly when parsing patch data nor while sending data to hardware.
- **(fixed)** Resolved issue where multi fx settings were not updated accordingly when master fx part patch was changed.
- **(fixed)** Resolved issue where Oscillator 2 Local Detune was not working as expected.
- **(fixed)** Virus TI models total recall rate adjusted. Might be slower, but this ensures better data processing in hardware.
- **(other)** In order for data sending to succeed, you MUST follow these steps when loading new instance of Virus Editor:
1) Select your Virus model. 2) Select MIDI input device. 3) Select MIDI output device. 4) Click 'SYNC DATA FROM HW' button from the User Interface. Enjoy usage as normal!

**Version 3.0.0 build 6891 / 2021-November-24**

- **(new)** Initialize Bank from Patch Librarian -> Bank Edit Menu -> Other Helpful Things...
- **(new)** UTILITY button added next to Save UI Data button.
  This opens a new menu with options to:
    - Initialize Active Part, Multi or Arrangement.
    - Copy and Paste Data between parts.
    - Load and Save MIDI CC Map files.
    - Version Notifier:
      (if internet and update are available, "Update Available" opens new window with recent changes).
- **(new)** MIDI In & Out Devices listed with "FROM:" and "TO:" prefixes.
- **(fixed)** MIDI In and MIDI Out Device names were not assigned properly in some cases.
- **(fixed)** Librarian right click menu "Paste" option is no longer available if clipboard is empty.
- **(fixed)** Resolved issue where DAW could crash in some cases if User Interface was closed.
- **(fixed)** Resolved issue where automation did not work as expected.
- **(fixed)** Tempo from host was not updated to plugin and hardware until User Interface was opened.
- **(improvement)** Librarian right click menu now has "Copy" option available for Upper list as well.
- **(improvement)** Drag and Drop works now from Lower to Upper list and within Upper list.
- **(improvement)** Clear MIDI button now opens a menu to Clear All or Active Parameter CC assignment.
- **(improvement)** If user attempts to set MIDI output before MIDI input, plugin/app display notifies user to set MIDI input first.
- **(improvement)** Updated Tips layer to reflect new changes in the User Interface.
- **(other)** Patch Librarian -> Bank Edit Menu -> Other Helpful Things... -> Check for updates now opens a new view if update is available.

**Version 3.0.0 build 6882 / 2021-November-16**

- **(new)** Part Solo, Part Mute and Part Selection switches added to main Multimode Mixer view.
- **(fixed)** Requesting ROM banks returned wrong patch data in Patch Librarian while model was set to TI or TI Snow.
- **(fixed)** Plugin / Application display will now indicate if Request Interval is too small.
- **(fixed)** Save Data to Slot button is now properly disabled in Multi Mode.
- **(fixed)** If part is muted by user or by requested multi, solo behaves as expected: if every solo switch is toggled off, then part mute set earlier keeps its value.
- **(fixed)** Part Solo didn't update plug-in display accordingly.
- **(fixed)** Part Mute didn't update plug-in display accordingly.
- **(fixed)** Whole arrangement data was not sent to hardware once "Push Data To HW" was triggered.
- **(fixed)** Resolved issue where plug-in was caught in a void loop when Total Recall or Load UI Data was triggered.
- **(other)** Request Interval default values set as follows: non-ti models (300ms) and ti models (400ms).

**Version 3.0.0 build 6875 / 2021-November-11**

- **(new)** All Notes Off ie, PANIC button can be found from the top right corner with MIDI plug icon (just in case...).
- **(fixed)** Resolved issue where wrong tab was opened after opening the plug-in window in DAW.
- **(fixed)** Plugin/Hardware tempo is now synchronized to DAW tempo by default.
- **(fixed)** Virus C scheme background was blurry on default scale level.
- **(fixed)** Changed the way how images are loaded once changing the UI Scheme.
- **(fixed)** Plugin display always "reset" when DAW playback was toggled on.
- **(fixed)** Double clicking resize handle now sets the window back to default state.
- **(other)** Performance improvements with graphics framework.

**Version 3.0.0 build 6868 / 2021-November-08**

- **(fixed)** Resolved issue where wrong background & buttons were loaded for some color schemes.
- **(fixed)** Resolved issue which could cause Live to crash when loading a project containing our plug-in.

**Version 3.0.0 build 6863 / 2021-November-08**

- **(new)** Part solo - user can now solo a single part or multiple parts from the part mixer view (patch librarian tab onwards).
- **(new)** Part Focus - If View Keyboard is toggled on, all MIDI CC data is driven to currently active part. There is a symbol in the mini mixer name view indicating data capture and a warning text below our logo. This only works when DAW is stopped.
- **(new)** Added missing input controls for other than TI models in multimode settings tab.
- **(new)** System Delays and System Arpeggiator On/Off switches added for models prior to Virus TI. These switches can be found from FX #1 and Arpeggiator tabs.
- **(new)** When data is being recalled / loaded from UI, visual feedback of data transmission is shown in the plug-in display.
- **(fixed)** Resolved issue where Bank popup menu items were not updated accordingly after initialization.
- **(fixed)** Resolved issue where part data was not properly set once data was synchronized from hardware or requested from hardware to part.
- **(fixed)** Resolved issue where incoming Global SysEx messages from other than TI models were not detected.
- **(fixed)** Resolved issue where data was overlapping when dumping data to hardware.
- **(fixed)** Resolved issue where data was not assigned to non-automated parameters correctly.
- **(fixed)** Selected Program value changed in Patch Librarian after recalling a project.
- **(fixed)** Some parameter alignments were off inside multi settings tabs.
- **(other)** Removed Save (overwrite) function from Patch Librarian -> Bank Edit Menu since macOS latest changes does not give us the permission to save files outside their desired "safe" zone.

**Version 3.0.0 build 6809 / 2021-November-02**

- **(fixed)** Resolved issue where Total Recall or naming a multi in multimode mixer view would freeze the user interface.
- **(fixed)** Resolved issue where Virus TI Snow user might have experienced a crash in some cases.
- **(fixed)** Patch / Multi rename input field aligned properly.

**Version 3.0.0 build 6737 / 2021-November-01**

- **(fixed)** Resolved issue which caused fatal crash when Clear MIDI was clicked.
- **(fixed)** Resolved issue where requesting temp multi data to librarian did not work as expected.
- **(fixed)** Resolved small SysEx error when requesting data to librarian by slot & bank.
- **(fixed)** Resolved issue where TI low and high key ranges were not responding at user interface.
- **(fixed)** Resolved issue where "Remember Bank" button did not work as expected.
- **(fixed)** Resolved issue where model selection and various other parameters were "reset" after plug-in window was closed.
- **(fixed)** Program Popup menu did not show correct program being selected when program number was 9 or greater.
- **(fixed)** Wrong program was requested from or sent to hardware when program popup menu was used.
- **(fixed)** Part change now reflects the current program number in librarian view.
- **(fixed)** Toggling between single and multi program mode did not update the librarian view as expected.
- **(fixed)** "Remember Bank" switch was shown in wrong tabs when data request was cancelled.
- **(improvement)** "Abort Process" switch is now shown above "Release All Locks" button when librarian view is not active.
- **(improvement)** "Save Part To Slot" button is no longer available in librarian multi mode.
- **(improvement)** Program selector indicator does not move in patch librarian view, when librarian is set to view multi programs and part program changes are received / sent.
- **(improvement)** "Set Virus to MULTI mode!" text will appear in the plugin / app display if single mode message is detected.

**Version 3.0.0 build 6621 / 2021-October-31**

- **(fixed)** Resolved issue which caused fatal crash when Randomizer was clicked.
- **(fixed)** Resolved issue data transfer got timed-out while requesting data from hardware.
- **(fixed)** Resolved issue where wrong part LED was lit during part change with Virus TI models.
- **(fixed)** Parameter display did not display value / control name while moving controls from hardware.
- **(fixed)** Resolved issue where registered plug-in instance would crash up on opening the plug-in.
- **(fixed)** In some cases, license.key was not written to disk even with right permissions.
- Registering plug-in via Patch Librarian -> Bank Edit Menu -> Register Plug-in.. now prompts for the license.key file and in the next window it will ask to store it in its readable location. Do not change the folder where you save the license, nor its name.
- **(improvement)** SysEx control movements consume less CPU now.

**Version 3.0.0 build 6598 / 2021-October-29**

- **(fixed)** Resolved issue why some parameter changes did not update plug-in display status accordingly.
- **(fixed)** Some parameters caused lag when value was changes from hardware.
- **(fixed)** Parameters did not update on the plug-in / app display properly when mouse was out of plug-in / app window.
- **(fixed)** Oscillator 3 Semitone did not adjust as expected.
- **(fixed)** SysEx parameters did not work as expected.
- **(fixed)** Part LEDs did not blink as expected when part change was applied from the hardware.
- **(improvement)** Mouse dragging / mouse wheel adjust for controls is a lot smoother now.
- For finer parameter control, hold down "ctrl" while adjusting the value.

**Version 3.0.0 build 6531 / 2021-October-26**

- **(fixed)** M1 Should validate now without warnings.
- **(fixed)** When about window was closed, MIDI i/o terminals were kept hidden (plug-ins only).

**Version 3.0.0 build 6526 / 2021-October-26**

- **(fixed)** File import dialog was showing save dialog instead.
- **(fixed)** license.key import dialog was showing save dialog instead.
- **(fixed)** Patch file Save As location hardcoded to Patches folder.
- **(fixed)** Various folder permission fixes.
- **(fixed)** Wrong url was shown in about page.
- **(other)** Patch files are located in: /Library/Audio/Presets/Mystery Islands Music/Access Virus Editor/Patches/
- **(other)** license.key should be placed in: /Library/Application Support/Mystery Islands Music/Resources/Access Virus Editor/ - license.key can be imported via Patch Librarian -&gt; Bank Edit Menu -&gt; Register Plug-in...
- **(bug)** Warnings do occur on some M1 macs - investigating.

**Version 3.0.0 build 4326 / 2021-October-25**

- **(new)** Question mark in the bottom right corner now pops up a hints window.
- **(fixed)** Virus TI SysEx data was not handled due to "MAX_SYSEX_SIZE" restriction.
- **(fixed)** If patches folder was missing, plug-in / app crashed under certain conditions.
- **(fixed)** Retina graphics for arpeggiator step length was non-retina image.
- **(other)** About window can be accessed from Patch Librarian -&gt; Bank Edit Menu.
- **(other)** Patch Data folder is now set at /Library/Audio/Presets/Mystery Islands Music/Access Virus Editor/Patches/

**Version 3.0.0 build 3815 / 2021-October-21**

** this release is available for macOS users only! Windows update in the works **

- **(new)** Plugin has been completely overhauled.
- **(new)** AAX, VST3 and Standalone Applications included.
- **(new)** Retina graphics.
- **(new)** Realtime User Interface size adjust.
- **(new)** Realtime User Interface skin adjust.
- **(new)** QWERTY keyboard included and functional when Keyboard is toggled on.
- **(new)** Load and Save current Multi arrangement data from the User Interface.
- **(new)** MIDI Learn. Ability to assign MIDI CC to selected SysEx controls as well.
- **(new)** Installer and APP are now notarized.
- **(new)** M1 support for Audio Unit, VST2, VST3 and Standalone APP.
- **(important)** Due to macOS development, macOS 10.12 or greater is required.
