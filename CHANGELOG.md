Changes in [1.9.7](https://github.com/vector-im/element-desktop/releases/tag/v1.9.7) (2021-12-13)
=================================================================================================

 * Security release with updated version of Olm to fix https://matrix.org/blog/2021/12/03/pre-disclosure-upcoming-security-release-of-libolm-and-matrix-js-sdk
 * Fix a crash on logout

Changes in [1.9.6](https://github.com/vector-im/element-desktop/releases/tag/v1.9.6) (2021-12-06)
=================================================================================================

## ✨ Features
 * Add unread indicator to the timelineCard header icon ([\#7156](https://github.com/matrix-org/matrix-react-sdk/pull/7156)). Fixes vector-im/element-web#19635.
 * Only show core navigation elements (call/chat/notification/info) when a widget is maximised ([\#7114](https://github.com/matrix-org/matrix-react-sdk/pull/7114)). Fixes vector-im/element-web#19632.
 * Improve ThreadPanel ctx menu accessibility ([\#7217](https://github.com/matrix-org/matrix-react-sdk/pull/7217)). Fixes vector-im/element-web#19885.
 * Allow filtering room list during treeview navigation ([\#7219](https://github.com/matrix-org/matrix-react-sdk/pull/7219)). Fixes vector-im/element-web#14702.
 * Add right panel chat timeline ([\#7112](https://github.com/matrix-org/matrix-react-sdk/pull/7112)). Fixes vector-im/element-web#19633.
 * Hide server options hint when disable_custom_urls is true ([\#7215](https://github.com/matrix-org/matrix-react-sdk/pull/7215)). Fixes vector-im/element-web#19919.
 * Improve right panel resize handle usability ([\#7204](https://github.com/matrix-org/matrix-react-sdk/pull/7204)). Fixes vector-im/element-web#15145. Contributed by @weeman1337.
 * Spaces quick settings ([\#7196](https://github.com/matrix-org/matrix-react-sdk/pull/7196)).
 * Maximised widgets always force a call to be shown in PIP mode ([\#7163](https://github.com/matrix-org/matrix-react-sdk/pull/7163)). Fixes vector-im/element-web#19637.
 * Group Labs flags ([\#7190](https://github.com/matrix-org/matrix-react-sdk/pull/7190)).
 * Show room context details in forward dialog ([\#7162](https://github.com/matrix-org/matrix-react-sdk/pull/7162)). Fixes vector-im/element-web#19793.
 * Remove chevrons from RoomSummaryCard_Button ([\#7137](https://github.com/matrix-org/matrix-react-sdk/pull/7137)). Fixes vector-im/element-web#19644.
 * Disable op/deop commands where user has no permissions ([\#7161](https://github.com/matrix-org/matrix-react-sdk/pull/7161)). Fixes vector-im/element-web#15390.
 * Add option to change the size of images/videos in the timeline ([\#7017](https://github.com/matrix-org/matrix-react-sdk/pull/7017)). Fixes vector-im/element-meta#49 vector-im/element-web#1520 and vector-im/element-web#19498.

## 🐛 Bug Fixes
 * Fix left panel glow in Safari ([\#7236](https://github.com/matrix-org/matrix-react-sdk/pull/7236)). Fixes vector-im/element-web#19863.
 * Fix newline on edit messages with quotes ([\#7227](https://github.com/matrix-org/matrix-react-sdk/pull/7227)). Fixes vector-im/element-web#12535. Contributed by @renancleyson-dev.
 * Guard against null refs in findSiblingElement ([\#7228](https://github.com/matrix-org/matrix-react-sdk/pull/7228)).
 * Tweak bottom of space panel buttons in expanded state ([\#7213](https://github.com/matrix-org/matrix-react-sdk/pull/7213)). Fixes vector-im/element-web#19921.
 * Fix multiline paragraph rendering as single line ([\#7210](https://github.com/matrix-org/matrix-react-sdk/pull/7210)). Fixes vector-im/element-web#8786. Contributed by @renancleyson-dev.
 * Improve room list message previews ([\#7224](https://github.com/matrix-org/matrix-react-sdk/pull/7224)). Fixes vector-im/element-web#17101 and vector-im/element-web#16169.
 * Fix EmojiPicker lazy loaded rendering bug ([\#7225](https://github.com/matrix-org/matrix-react-sdk/pull/7225)). Fixes vector-im/element-web#15341.
 * Prevent default avatar in UserInfo having pointer cursor ([\#7218](https://github.com/matrix-org/matrix-react-sdk/pull/7218)). Fixes vector-im/element-web#13872.
 * Prevent duplicate avatars in Event List Summaries ([\#7222](https://github.com/matrix-org/matrix-react-sdk/pull/7222)). Fixes vector-im/element-web#17706.
 * Respect the home page as a context for the Home space ([\#7216](https://github.com/matrix-org/matrix-react-sdk/pull/7216)). Fixes vector-im/element-web#19554.
 * Fix RoomUpgradeWarningBar exploding ([\#7214](https://github.com/matrix-org/matrix-react-sdk/pull/7214)). Fixes vector-im/element-web#19920.
 * Polish threads misalignments and UI diversion ([\#7209](https://github.com/matrix-org/matrix-react-sdk/pull/7209)). Fixes vector-im/element-web#19772, vector-im/element-web#19710 vector-im/element-web#19629 and vector-im/element-web#19711.
 * Fix Manage Restricted Join Rule Dialog for Spaces ([\#7208](https://github.com/matrix-org/matrix-react-sdk/pull/7208)). Fixes vector-im/element-web#19610.
 * Fix wrongly showing unpin in pinned messages tile with no perms ([\#7197](https://github.com/matrix-org/matrix-react-sdk/pull/7197)). Fixes vector-im/element-web#19886.
 * Make image size constrained by height when using the ImageSize.Large option ([\#7171](https://github.com/matrix-org/matrix-react-sdk/pull/7171)). Fixes vector-im/element-web#19788.
 * Prevent programmatic scrolling within truncated room sublists ([\#7191](https://github.com/matrix-org/matrix-react-sdk/pull/7191)).
 * Remove leading slash from /addwidget Jitsi confs ([\#7175](https://github.com/matrix-org/matrix-react-sdk/pull/7175)). Fixes vector-im/element-web#19839. Contributed by @AndrewFerr.
 * Fix automatic composer focus, regressed by threads work ([\#7167](https://github.com/matrix-org/matrix-react-sdk/pull/7167)). Fixes vector-im/element-web#19479.
 * Show space members when not invited even if summary didn't fail ([\#7153](https://github.com/matrix-org/matrix-react-sdk/pull/7153)). Fixes vector-im/element-web#19781.
 * Prevent custom power levels from breaking roles & permissions tab ([\#7160](https://github.com/matrix-org/matrix-react-sdk/pull/7160)). Fixes vector-im/element-web#19812.
 * Room Context Menu should respond to tag changes ([\#7154](https://github.com/matrix-org/matrix-react-sdk/pull/7154)). Fixes vector-im/element-web#19776.
 * Fix an edge case when trying to join an upgraded room ([\#7159](https://github.com/matrix-org/matrix-react-sdk/pull/7159)).

Changes in [1.9.5](https://github.com/vector-im/element-desktop/releases/tag/v1.9.5) (2021-11-22)
=================================================================================================

## ✨ Features
 * Make double-clicking the PiP take you to the call room ([\#7142](https://github.com/matrix-org/matrix-react-sdk/pull/7142)). Fixes vector-im/element-web#18421 vector-im/element-web#15920 and vector-im/element-web#18421. Contributed by @SimonBrandner.
 * Add maximise widget functionality ([\#7098](https://github.com/matrix-org/matrix-react-sdk/pull/7098)). Fixes vector-im/element-web#19619, vector-im/element-web#19621 vector-im/element-web#19760 and vector-im/element-web#19619.
 * Add rainfall effect ([\#7086](https://github.com/matrix-org/matrix-react-sdk/pull/7086)). Contributed by @justjosias.
 * Add root folder to zip file created by export chat feature ([\#7097](https://github.com/matrix-org/matrix-react-sdk/pull/7097)). Fixes vector-im/element-web#19653 and vector-im/element-web#19653. Contributed by @aaronraimist.
 * Improve VoIP UI/UX ([\#7048](https://github.com/matrix-org/matrix-react-sdk/pull/7048)). Fixes vector-im/element-web#19513 and vector-im/element-web#19513. Contributed by @SimonBrandner.
 * Unified room context menus ([\#7072](https://github.com/matrix-org/matrix-react-sdk/pull/7072)). Fixes vector-im/element-web#19527 and vector-im/element-web#19527.
 * In forgot password screen, show validation errors inline in the form, instead of in modals ([\#7113](https://github.com/matrix-org/matrix-react-sdk/pull/7113)). Contributed by @psrpinto.
 * Implement more meta-spaces ([\#7077](https://github.com/matrix-org/matrix-react-sdk/pull/7077)). Fixes vector-im/element-web#18634 vector-im/element-web#17295 and vector-im/element-web#18634.
 * Expose power level control for m.space.child ([\#7120](https://github.com/matrix-org/matrix-react-sdk/pull/7120)).
 * Forget member-list query when switching out of a room ([\#7093](https://github.com/matrix-org/matrix-react-sdk/pull/7093)). Fixes vector-im/element-web#19432 and vector-im/element-web#19432. Contributed by @SimonBrandner.
 * Do pre-submit availability check on username during registration ([\#6978](https://github.com/matrix-org/matrix-react-sdk/pull/6978)). Fixes vector-im/element-web#9545 and vector-im/element-web#9545.

## 🐛 Bug Fixes
 * Adjust recovery key button sizes depending on text width ([\#7134](https://github.com/matrix-org/matrix-react-sdk/pull/7134)). Fixes vector-im/element-web#19511 and vector-im/element-web#19511. Contributed by @weeman1337.
 * Fix bulk invite button getting a negative count ([\#7122](https://github.com/matrix-org/matrix-react-sdk/pull/7122)). Fixes vector-im/element-web#19466 and vector-im/element-web#19466. Contributed by @renancleyson-dev.
 * Fix maximised / pinned widget state being loaded correctly ([\#7146](https://github.com/matrix-org/matrix-react-sdk/pull/7146)). Fixes vector-im/element-web#19768 and vector-im/element-web#19768.
 * Don't reload the page when user hits enter when entering ban reason ([\#7145](https://github.com/matrix-org/matrix-react-sdk/pull/7145)). Fixes vector-im/element-web#19763 and vector-im/element-web#19763.
 * Fix timeline text when sharing room layout ([\#7140](https://github.com/matrix-org/matrix-react-sdk/pull/7140)). Fixes vector-im/element-web#19622 and vector-im/element-web#19622.
 * Fix look of emoji verification ([\#7133](https://github.com/matrix-org/matrix-react-sdk/pull/7133)). Fixes vector-im/element-web#19740 and vector-im/element-web#19740. Contributed by @SimonBrandner.
 * Fixes element not remembering widget hidden state per room ([\#7136](https://github.com/matrix-org/matrix-react-sdk/pull/7136)). Fixes vector-im/element-web#16672, matrix-org/element-web-rageshakes#4407, vector-im/element-web#15718 vector-im/element-web#15768 and vector-im/element-web#16672.
 * Don't keep spinning if joining space child failed ([\#7129](https://github.com/matrix-org/matrix-react-sdk/pull/7129)). Fixes matrix-org/element-web-rageshakes#6813 and matrix-org/element-web-rageshakes#6813.
 * Guard around SpaceStore onAccountData handler prevEvent ([\#7123](https://github.com/matrix-org/matrix-react-sdk/pull/7123)). Fixes vector-im/element-web#19705 and vector-im/element-web#19705.
 * Fix missing spaces in threads copy ([\#7119](https://github.com/matrix-org/matrix-react-sdk/pull/7119)). Fixes vector-im/element-web#19702 and vector-im/element-web#19702.
 * Fix hover tile border ([\#7117](https://github.com/matrix-org/matrix-react-sdk/pull/7117)). Fixes vector-im/element-web#19698 and vector-im/element-web#19698. Contributed by @SimonBrandner.
 * Fix quote button ([\#7096](https://github.com/matrix-org/matrix-react-sdk/pull/7096)). Fixes vector-im/element-web#19659 and vector-im/element-web#19659. Contributed by @SimonBrandner.
 * Fix space panel layout edge cases ([\#7101](https://github.com/matrix-org/matrix-react-sdk/pull/7101)). Fixes vector-im/element-web#19668 and vector-im/element-web#19668.
 * Update powerlevel/role when the user changes in the user info panel ([\#7099](https://github.com/matrix-org/matrix-react-sdk/pull/7099)). Fixes vector-im/element-web#19666 and vector-im/element-web#19666. Contributed by @SimonBrandner.
 * Fix avatar disappearing when setting a room topic ([\#7092](https://github.com/matrix-org/matrix-react-sdk/pull/7092)). Fixes vector-im/element-web#19226 and vector-im/element-web#19226. Contributed by @SimonBrandner.
 * Fix possible infinite loop on widget start ([\#7071](https://github.com/matrix-org/matrix-react-sdk/pull/7071)). Fixes vector-im/element-web#15494 and vector-im/element-web#15494.
 * Use device IDs for nameless devices in device list ([\#7081](https://github.com/matrix-org/matrix-react-sdk/pull/7081)). Fixes vector-im/element-web#19608 and vector-im/element-web#19608.
 * Don't re-sort rooms on no-op RoomUpdateCause.PossibleTagChange ([\#7053](https://github.com/matrix-org/matrix-react-sdk/pull/7053)). Contributed by @bradtgmurray.

Changes in [1.9.4](https://github.com/vector-im/element-desktop/releases/tag/v1.9.4) (2021-11-08)
=================================================================================================

## ✨ Features
 * Improve the look of tooltips ([\#7049](https://github.com/matrix-org/matrix-react-sdk/pull/7049)). Contributed by @SimonBrandner.
 * Improve the look of the spinner ([\#6083](https://github.com/matrix-org/matrix-react-sdk/pull/6083)). Contributed by @SimonBrandner.
 * Polls: Creation form & start event ([\#7001](https://github.com/matrix-org/matrix-react-sdk/pull/7001)).
 * Show a gray shield when encrypted by deleted session ([\#6119](https://github.com/matrix-org/matrix-react-sdk/pull/6119)). Contributed by @SimonBrandner.
 * Silence some widgets for better screen reader presentation. ([\#7057](https://github.com/matrix-org/matrix-react-sdk/pull/7057)). Contributed by @ndarilek.
 * Make message separator more accessible. ([\#7056](https://github.com/matrix-org/matrix-react-sdk/pull/7056)). Contributed by @ndarilek.
 * Give each room directory entry the `listitem` role to correspond with the containing `list`. ([\#7035](https://github.com/matrix-org/matrix-react-sdk/pull/7035)). Contributed by @ndarilek.
 * Implement RequiresClient capability for widgets ([\#7005](https://github.com/matrix-org/matrix-react-sdk/pull/7005)). Fixes vector-im/element-web#15744 and vector-im/element-web#15744.
 * Respect the system high contrast setting when using system theme ([\#7043](https://github.com/matrix-org/matrix-react-sdk/pull/7043)).
 * Remove redundant duplicate mimetype field which doesn't conform to spec ([\#7045](https://github.com/matrix-org/matrix-react-sdk/pull/7045)). Fixes vector-im/element-web#17145 and vector-im/element-web#17145.
 * Make join button on space hierarchy action in the background ([\#7041](https://github.com/matrix-org/matrix-react-sdk/pull/7041)). Fixes vector-im/element-web#17388 and vector-im/element-web#17388.
 * Add a high contrast theme (a variant of the light theme) ([\#7036](https://github.com/matrix-org/matrix-react-sdk/pull/7036)).
 * Improve timeline message for restricted join rule changes ([\#6984](https://github.com/matrix-org/matrix-react-sdk/pull/6984)). Fixes vector-im/element-web#18980 and vector-im/element-web#18980.
 * Improve the appearance of the font size slider ([\#7038](https://github.com/matrix-org/matrix-react-sdk/pull/7038)).
 * Improve RovingTabIndex & Room List filtering performance ([\#6987](https://github.com/matrix-org/matrix-react-sdk/pull/6987)). Fixes vector-im/element-web#17864 and vector-im/element-web#17864.
 * Remove outdated Spaces restricted rooms warning ([\#6927](https://github.com/matrix-org/matrix-react-sdk/pull/6927)).
 * Make /msg <message> param optional for more flexibility ([\#7028](https://github.com/matrix-org/matrix-react-sdk/pull/7028)). Fixes vector-im/element-web#19481 and vector-im/element-web#19481.
 * Add decoration to space hierarchy for tiles which have already been j… ([\#6969](https://github.com/matrix-org/matrix-react-sdk/pull/6969)). Fixes vector-im/element-web#18755 and vector-im/element-web#18755.
 * Add insert link button to the format bar ([\#5879](https://github.com/matrix-org/matrix-react-sdk/pull/5879)). Contributed by @SimonBrandner.
 * Improve visibility of font size chooser ([\#6988](https://github.com/matrix-org/matrix-react-sdk/pull/6988)).
 * Soften border-radius on selected/hovered messages ([\#6525](https://github.com/matrix-org/matrix-react-sdk/pull/6525)). Fixes vector-im/element-web#18108. Contributed by @SimonBrandner.
 * Add a developer mode flag and use it for accessing space timelines ([\#6994](https://github.com/matrix-org/matrix-react-sdk/pull/6994)). Fixes vector-im/element-web#19416 and vector-im/element-web#19416.
 * Position toggle switch more clearly ([\#6914](https://github.com/matrix-org/matrix-react-sdk/pull/6914)). Contributed by @CicadaCinema.
 * Validate email address in forgot password dialog ([\#6983](https://github.com/matrix-org/matrix-react-sdk/pull/6983)). Fixes vector-im/element-web#9978 and vector-im/element-web#9978. Contributed by @psrpinto.
 * Handle and i18n M_THREEPID_IN_USE during registration ([\#6986](https://github.com/matrix-org/matrix-react-sdk/pull/6986)). Fixes vector-im/element-web#13767 and vector-im/element-web#13767.
 * For space invite previews, use room summary API to get the right member count ([\#6982](https://github.com/matrix-org/matrix-react-sdk/pull/6982)). Fixes vector-im/element-web#19123 and vector-im/element-web#19123.
 * Simplify Space Panel notification badge layout ([\#6977](https://github.com/matrix-org/matrix-react-sdk/pull/6977)). Fixes vector-im/element-web#18527 and vector-im/element-web#18527.
 * Use prettier hsName during 3pid registration where possible ([\#6980](https://github.com/matrix-org/matrix-react-sdk/pull/6980)). Fixes vector-im/element-web#19162 and vector-im/element-web#19162.

## 🐛 Bug Fixes
 * Add a condition to only activate the resizer which belongs to the clicked handle ([\#7055](https://github.com/matrix-org/matrix-react-sdk/pull/7055)). Fixes vector-im/element-web#19521 and vector-im/element-web#19521.
 * Restore composer focus after event edit ([\#7065](https://github.com/matrix-org/matrix-react-sdk/pull/7065)). Fixes vector-im/element-web#19469 and vector-im/element-web#19469.
 * Don't apply message bubble visual style to media messages ([\#7040](https://github.com/matrix-org/matrix-react-sdk/pull/7040)).
 * Handle no selected screen when screen-sharing ([\#7018](https://github.com/matrix-org/matrix-react-sdk/pull/7018)). Fixes vector-im/element-web#19460 and vector-im/element-web#19460. Contributed by @SimonBrandner.
 * Add history entry before completing emoji ([\#7007](https://github.com/matrix-org/matrix-react-sdk/pull/7007)). Fixes vector-im/element-web#19177 and vector-im/element-web#19177. Contributed by @RafaelGoncalves8.
 * Add padding between controls on edit form in message bubbles ([\#7039](https://github.com/matrix-org/matrix-react-sdk/pull/7039)).
 * Respect the roomState right container request for the Jitsi widget ([\#7033](https://github.com/matrix-org/matrix-react-sdk/pull/7033)). Fixes vector-im/element-web#16552 and vector-im/element-web#16552.
 * Fix cannot read length of undefined for room upgrades ([\#7037](https://github.com/matrix-org/matrix-react-sdk/pull/7037)). Fixes vector-im/element-web#19509 and vector-im/element-web#19509.
 * Cleanup re-dispatching around timelines and composers ([\#7023](https://github.com/matrix-org/matrix-react-sdk/pull/7023)). Fixes vector-im/element-web#19491 and vector-im/element-web#19491. Contributed by @SimonBrandner.
 * Fix removing a room from a Space and interaction with `m.space.parent` ([\#6944](https://github.com/matrix-org/matrix-react-sdk/pull/6944)). Fixes vector-im/element-web#19363 and vector-im/element-web#19363.
 * Fix recent css regression ([\#7022](https://github.com/matrix-org/matrix-react-sdk/pull/7022)). Fixes vector-im/element-web#19470 and vector-im/element-web#19470. Contributed by @CicadaCinema.
 * Fix ModalManager reRender racing with itself ([\#7027](https://github.com/matrix-org/matrix-react-sdk/pull/7027)). Fixes vector-im/element-web#19489 and vector-im/element-web#19489.
 * Fix fullscreening a call while connecting ([\#7019](https://github.com/matrix-org/matrix-react-sdk/pull/7019)). Fixes vector-im/element-web#19309 and vector-im/element-web#19309. Contributed by @SimonBrandner.
 * Allow scrolling right in reply-quoted code block ([\#7024](https://github.com/matrix-org/matrix-react-sdk/pull/7024)). Fixes vector-im/element-web#19487 and vector-im/element-web#19487. Contributed by @SimonBrandner.
 * Fix dark theme codeblock colors ([\#6384](https://github.com/matrix-org/matrix-react-sdk/pull/6384)). Fixes vector-im/element-web#17998. Contributed by @SimonBrandner.
 * Show passphrase input label ([\#6992](https://github.com/matrix-org/matrix-react-sdk/pull/6992)). Fixes vector-im/element-web#19428 and vector-im/element-web#19428. Contributed by @RafaelGoncalves8.
 * Always render disabled settings as disabled ([\#7014](https://github.com/matrix-org/matrix-react-sdk/pull/7014)).
 * Make "Security Phrase" placeholder look consistent cross-browser ([\#6870](https://github.com/matrix-org/matrix-react-sdk/pull/6870)). Fixes vector-im/element-web#19006 and vector-im/element-web#19006. Contributed by @neer17.
 * Fix direction override characters breaking member event text direction ([\#6999](https://github.com/matrix-org/matrix-react-sdk/pull/6999)).
 * Remove redundant text in verification dialogs ([\#6993](https://github.com/matrix-org/matrix-react-sdk/pull/6993)). Fixes vector-im/element-web#19290 and vector-im/element-web#19290. Contributed by @RafaelGoncalves8.
 * Fix space panel name overflowing ([\#6995](https://github.com/matrix-org/matrix-react-sdk/pull/6995)). Fixes vector-im/element-web#19455 and vector-im/element-web#19455.
 * Fix conflicting CSS on syntax highlighted blocks ([\#6991](https://github.com/matrix-org/matrix-react-sdk/pull/6991)). Fixes vector-im/element-web#19445 and vector-im/element-web#19445.

Changes in [1.9.3](https://github.com/vector-im/element-desktop/releases/tag/v1.9.3) (2021-10-25)
=================================================================================================

## ✨ Features
 * Convert the "Cryptography" settings panel to an HTML table to assist screen reader users. ([\#6968](https://github.com/matrix-org/matrix-react-sdk/pull/6968)). Contributed by [andybalaam](https://github.com/andybalaam).
 * Swap order of private space creation and tweak copy ([\#6967](https://github.com/matrix-org/matrix-react-sdk/pull/6967)). Fixes vector-im/element-web#18768 and vector-im/element-web#18768.
 * Add spacing to Room settings - Notifications subsection ([\#6962](https://github.com/matrix-org/matrix-react-sdk/pull/6962)). Contributed by [CicadaCinema](https://github.com/CicadaCinema).
 * Use HTML tables for some tabular user interface areas, to assist with screen reader use ([\#6955](https://github.com/matrix-org/matrix-react-sdk/pull/6955)). Contributed by [andybalaam](https://github.com/andybalaam).
 * Fix space invite edge cases ([\#6884](https://github.com/matrix-org/matrix-react-sdk/pull/6884)). Fixes vector-im/element-web#19010 vector-im/element-web#17345 and vector-im/element-web#19010.
 * Allow options to cascade kicks/bans throughout spaces ([\#6829](https://github.com/matrix-org/matrix-react-sdk/pull/6829)). Fixes vector-im/element-web#18969 and vector-im/element-web#18969.
 * Make public space alias field mandatory again ([\#6921](https://github.com/matrix-org/matrix-react-sdk/pull/6921)). Fixes vector-im/element-web#19003 and vector-im/element-web#19003.
 * Add progress bar to restricted room upgrade dialog ([\#6919](https://github.com/matrix-org/matrix-react-sdk/pull/6919)). Fixes vector-im/element-web#19146 and vector-im/element-web#19146.
 * Add customisation point for visibility of invites and room creation ([\#6922](https://github.com/matrix-org/matrix-react-sdk/pull/6922)). Fixes vector-im/element-web#19331 and vector-im/element-web#19331.
 * Inhibit `Unable to get validated threepid` error during UIA ([\#6928](https://github.com/matrix-org/matrix-react-sdk/pull/6928)). Fixes vector-im/element-web#18883 and vector-im/element-web#18883.
 * Tweak room list skeleton UI height and behaviour ([\#6926](https://github.com/matrix-org/matrix-react-sdk/pull/6926)). Fixes vector-im/element-web#18231 vector-im/element-web#16581 and vector-im/element-web#18231.
 * If public room creation fails, retry without publishing it ([\#6872](https://github.com/matrix-org/matrix-react-sdk/pull/6872)). Fixes vector-im/element-web#19194 and vector-im/element-web#19194. Contributed by [AndrewFerr](https://github.com/AndrewFerr).
 * Iterate invite your teammates to Space view ([\#6925](https://github.com/matrix-org/matrix-react-sdk/pull/6925)). Fixes vector-im/element-web#18772 and vector-im/element-web#18772.
 * Make placeholder more grey when no input ([\#6840](https://github.com/matrix-org/matrix-react-sdk/pull/6840)). Fixes vector-im/element-web#17243 and vector-im/element-web#17243. Contributed by [wlach](https://github.com/wlach).
 * Respect tombstones in locally known rooms for Space children ([\#6906](https://github.com/matrix-org/matrix-react-sdk/pull/6906)). Fixes vector-im/element-web#19246 vector-im/element-web#19256 and vector-im/element-web#19246.
 * Improve emoji shortcodes generated from annotations ([\#6907](https://github.com/matrix-org/matrix-react-sdk/pull/6907)). Fixes vector-im/element-web#19304 and vector-im/element-web#19304.
 * Hide kick & ban options in UserInfo when looking at own profile ([\#6911](https://github.com/matrix-org/matrix-react-sdk/pull/6911)). Fixes vector-im/element-web#19066 and vector-im/element-web#19066.
 * Add progress bar to Community to Space migration tool ([\#6887](https://github.com/matrix-org/matrix-react-sdk/pull/6887)). Fixes vector-im/element-web#19216 and vector-im/element-web#19216.

## 🐛 Bug Fixes
 * Fix leave space cancel button exploding ([\#6966](https://github.com/matrix-org/matrix-react-sdk/pull/6966)).
 * Fix edge case behaviour of the space join spinner for guests ([\#6972](https://github.com/matrix-org/matrix-react-sdk/pull/6972)). Fixes vector-im/element-web#19359 and vector-im/element-web#19359.
 * Convert emoticon to emoji at the end of a line on send even if the cursor isn't there ([\#6965](https://github.com/matrix-org/matrix-react-sdk/pull/6965)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix text overflows button on Home page ([\#6898](https://github.com/matrix-org/matrix-react-sdk/pull/6898)). Fixes vector-im/element-web#19180 and vector-im/element-web#19180. Contributed by [oliver-pham](https://github.com/oliver-pham).
 * Space Room View should react to join rule changes down /sync ([\#6945](https://github.com/matrix-org/matrix-react-sdk/pull/6945)). Fixes vector-im/element-web#19390 and vector-im/element-web#19390.
 * Hide leave section button if user isn't in the room e.g peeking ([\#6920](https://github.com/matrix-org/matrix-react-sdk/pull/6920)). Fixes vector-im/element-web#17410 and vector-im/element-web#17410.
 * Fix bug where room list would get stuck showing no rooms ([\#6939](https://github.com/matrix-org/matrix-react-sdk/pull/6939)). Fixes vector-im/element-web#19373 and vector-im/element-web#19373.
 * Update room settings dialog title when room name changes ([\#6916](https://github.com/matrix-org/matrix-react-sdk/pull/6916)). Fixes vector-im/element-web#17480 and vector-im/element-web#17480. Contributed by [psrpinto](https://github.com/psrpinto).
 * Fix editing losing emote-ness and rainbow-ness of messages ([\#6931](https://github.com/matrix-org/matrix-react-sdk/pull/6931)). Fixes vector-im/element-web#19350 and vector-im/element-web#19350.
 * Remove semicolon from notifications panel ([\#6930](https://github.com/matrix-org/matrix-react-sdk/pull/6930)). Contributed by [robintown](https://github.com/robintown).
 * Prevent profile image in left panel's backdrop from being selected ([\#6924](https://github.com/matrix-org/matrix-react-sdk/pull/6924)). Contributed by [rom4nik](https://github.com/rom4nik).
 * Validate that the phone number verification field is filled before allowing user to submit ([\#6918](https://github.com/matrix-org/matrix-react-sdk/pull/6918)). Fixes vector-im/element-web#19316 and vector-im/element-web#19316. Contributed by [VFermat](https://github.com/VFermat).
 * Updated how save button becomes disabled in room settings to listen for all fields instead of the most recent ([\#6917](https://github.com/matrix-org/matrix-react-sdk/pull/6917)). Contributed by [LoganArnett](https://github.com/LoganArnett).
 * Use FocusLock around ContextMenus to simplify focus management ([\#6311](https://github.com/matrix-org/matrix-react-sdk/pull/6311)). Fixes vector-im/element-web#19259 and vector-im/element-web#19259.
 * Fix space hierarchy pagination ([\#6908](https://github.com/matrix-org/matrix-react-sdk/pull/6908)). Fixes vector-im/element-web#19276 and vector-im/element-web#19276.
 * Fix spaces keyboard shortcuts not working for last space ([\#6909](https://github.com/matrix-org/matrix-react-sdk/pull/6909)). Fixes vector-im/element-web#19255 and vector-im/element-web#19255.
 * Use fallback avatar only for DMs with 2 people. ([\#6895](https://github.com/matrix-org/matrix-react-sdk/pull/6895)). Fixes vector-im/element-web#18747 and vector-im/element-web#18747. Contributed by [andybalaam](https://github.com/andybalaam).

Changes in [1.9.2](https://github.com/vector-im/element-desktop/releases/tag/v1.9.2) (2021-10-12)
=================================================================================================

## 🐛 Bug Fixes
 * Upgrade to matrix-js-sdk#14.0.1

Changes in [1.9.1](https://github.com/vector-im/element-desktop/releases/tag/v1.9.1) (2021-10-11)
=================================================================================================

## ✨ Features
 * Decrease profile button touch target ([\#6900](https://github.com/matrix-org/matrix-react-sdk/pull/6900)). Contributed by [ColonisationCaptain](https://github.com/ColonisationCaptain).
 * Don't let click events propagate out of context menus ([\#6892](https://github.com/matrix-org/matrix-react-sdk/pull/6892)).
 * Allow closing Dropdown via its chevron ([\#6885](https://github.com/matrix-org/matrix-react-sdk/pull/6885)). Fixes vector-im/element-web#19030 and vector-im/element-web#19030.
 * Improve AUX panel behaviour ([\#6699](https://github.com/matrix-org/matrix-react-sdk/pull/6699)). Fixes vector-im/element-web#18787 and vector-im/element-web#18787. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * A nicer opening animation for the Image View ([\#6454](https://github.com/matrix-org/matrix-react-sdk/pull/6454)). Fixes vector-im/element-web#18186 and vector-im/element-web#18186. Contributed by [SimonBrandner](https://github.com/SimonBrandner).

## 🐛 Bug Fixes
 * [Release] Fix space hierarchy pagination ([\#6910](https://github.com/matrix-org/matrix-react-sdk/pull/6910)).
 * Fix leaving space via other client leaving you in undefined-land ([\#6891](https://github.com/matrix-org/matrix-react-sdk/pull/6891)). Fixes vector-im/element-web#18455 and vector-im/element-web#18455.
 * Handle newer voice message encrypted event format for chat export ([\#6893](https://github.com/matrix-org/matrix-react-sdk/pull/6893)). Contributed by [jaiwanth-v](https://github.com/jaiwanth-v).
 * Fix pagination when filtering space hierarchy ([\#6876](https://github.com/matrix-org/matrix-react-sdk/pull/6876)). Fixes vector-im/element-web#19235 and vector-im/element-web#19235.
 * Fix spaces null-guard breaking the dispatcher settings watching ([\#6886](https://github.com/matrix-org/matrix-react-sdk/pull/6886)). Fixes vector-im/element-web#19223 and vector-im/element-web#19223.
 * Fix space children without specific `order` being sorted after those with one ([\#6878](https://github.com/matrix-org/matrix-react-sdk/pull/6878)). Fixes vector-im/element-web#19192 and vector-im/element-web#19192.
 * Ensure that sub-spaces aren't considered for notification badges ([\#6881](https://github.com/matrix-org/matrix-react-sdk/pull/6881)). Fixes vector-im/element-web#18975 and vector-im/element-web#18975.
 * Fix timeline autoscroll with non-standard DPI settings. ([\#6880](https://github.com/matrix-org/matrix-react-sdk/pull/6880)). Fixes vector-im/element-web#18984 and vector-im/element-web#18984.
 * Pluck out JoinRuleSettings styles so they apply in space settings too ([\#6879](https://github.com/matrix-org/matrix-react-sdk/pull/6879)). Fixes vector-im/element-web#19164 and vector-im/element-web#19164.
 * Null guard around the matrixClient in SpaceStore ([\#6874](https://github.com/matrix-org/matrix-react-sdk/pull/6874)).
 * Fix issue (https ([\#6871](https://github.com/matrix-org/matrix-react-sdk/pull/6871)). Fixes vector-im/element-web#19138 and vector-im/element-web#19138. Contributed by [psrpinto](https://github.com/psrpinto).
 * Fix pills being cut off in message bubble layout ([\#6865](https://github.com/matrix-org/matrix-react-sdk/pull/6865)). Fixes vector-im/element-web#18627 and vector-im/element-web#18627. Contributed by [robintown](https://github.com/robintown).
 * Fix space admin check false positive on multiple admins ([\#6824](https://github.com/matrix-org/matrix-react-sdk/pull/6824)).
 * Fix the User View ([\#6860](https://github.com/matrix-org/matrix-react-sdk/pull/6860)). Fixes vector-im/element-web#19158 and vector-im/element-web#19158.
 * Fix spacing for message composer buttons ([\#6852](https://github.com/matrix-org/matrix-react-sdk/pull/6852)). Fixes vector-im/element-web#18999 and vector-im/element-web#18999.
 * Always show root event of a thread in room's timeline ([\#6842](https://github.com/matrix-org/matrix-react-sdk/pull/6842)). Fixes vector-im/element-web#19016 and vector-im/element-web#19016.

Changes in [1.9.0](https://github.com/vector-im/element-desktop/releases/tag/v1.9.0) (2021-09-27)
=================================================================================================

## ✨ Features
 * Fix space keyboard shortcuts conflicting with native zoom shortcuts ([\#19037](https://github.com/vector-im/element-web/pull/19037)). Fixes vector-im/element-web#18481 and undefined/element-web#18481.
 * Say Joining space instead of Joining room where we know its a space ([\#6818](https://github.com/matrix-org/matrix-react-sdk/pull/6818)). Fixes vector-im/element-web#19064 and vector-im/element-web#19064.
 * Add warning that some spaces may not be relinked to the newly upgraded room ([\#6805](https://github.com/matrix-org/matrix-react-sdk/pull/6805)). Fixes vector-im/element-web#18858 and vector-im/element-web#18858.
 * Delabs Spaces, iterate some copy and move communities/space toggle to preferences ([\#6594](https://github.com/matrix-org/matrix-react-sdk/pull/6594)). Fixes vector-im/element-web#18088, vector-im/element-web#18524 vector-im/element-web#18088 and vector-im/element-web#18088.
 * Show "Message" in the user info panel instead of "Start chat" ([\#6319](https://github.com/matrix-org/matrix-react-sdk/pull/6319)). Fixes vector-im/element-web#17877 and vector-im/element-web#17877. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix space keyboard shortcuts conflicting with native zoom shortcuts ([\#6804](https://github.com/matrix-org/matrix-react-sdk/pull/6804)).
 * Replace plain text emoji at the end of a line ([\#6784](https://github.com/matrix-org/matrix-react-sdk/pull/6784)). Fixes vector-im/element-web#18833 and vector-im/element-web#18833. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Simplify Space Panel layout and fix some edge cases ([\#6800](https://github.com/matrix-org/matrix-react-sdk/pull/6800)). Fixes vector-im/element-web#18694 and vector-im/element-web#18694.
 * Show unsent message warning on Space Panel buttons ([\#6778](https://github.com/matrix-org/matrix-react-sdk/pull/6778)). Fixes vector-im/element-web#18891 and vector-im/element-web#18891.
 * Hide mute/unmute button in UserInfo for Spaces as it makes no sense ([\#6790](https://github.com/matrix-org/matrix-react-sdk/pull/6790)). Fixes vector-im/element-web#19007 and vector-im/element-web#19007.
 * Fix automatic field population in space create menu not validating ([\#6792](https://github.com/matrix-org/matrix-react-sdk/pull/6792)). Fixes vector-im/element-web#19005 and vector-im/element-web#19005.
 * Optimize input label transition on focus ([\#6783](https://github.com/matrix-org/matrix-react-sdk/pull/6783)). Fixes vector-im/element-web#12876 and vector-im/element-web#12876. Contributed by [MadLittleMods](https://github.com/MadLittleMods).
 * Adapt and re-use the RolesRoomSettingsTab for Spaces ([\#6779](https://github.com/matrix-org/matrix-react-sdk/pull/6779)). Fixes vector-im/element-web#18908 vector-im/element-web#18909 and vector-im/element-web#18908.
 * Deduplicate join rule management between rooms and spaces ([\#6724](https://github.com/matrix-org/matrix-react-sdk/pull/6724)). Fixes vector-im/element-web#18798 and vector-im/element-web#18798.
 * Add config option to turn on in-room event sending timing metrics ([\#6766](https://github.com/matrix-org/matrix-react-sdk/pull/6766)).
 * Improve the upgrade for restricted user experience ([\#6764](https://github.com/matrix-org/matrix-react-sdk/pull/6764)). Fixes vector-im/element-web#18677 and vector-im/element-web#18677.
 * Improve tooltips on space quick actions and explore button ([\#6760](https://github.com/matrix-org/matrix-react-sdk/pull/6760)). Fixes vector-im/element-web#18528 and vector-im/element-web#18528.
 * Make space members and user info behave more expectedly ([\#6765](https://github.com/matrix-org/matrix-react-sdk/pull/6765)). Fixes vector-im/element-web#17018 and vector-im/element-web#17018.
 * hide no-op m.room.encryption events and better word param changes ([\#6747](https://github.com/matrix-org/matrix-react-sdk/pull/6747)). Fixes vector-im/element-web#18597 and vector-im/element-web#18597.
 * Respect m.space.parent relations if they hold valid permissions ([\#6746](https://github.com/matrix-org/matrix-react-sdk/pull/6746)). Fixes vector-im/element-web#10935 and vector-im/element-web#10935.
 * Space panel accessibility improvements ([\#6744](https://github.com/matrix-org/matrix-react-sdk/pull/6744)). Fixes vector-im/element-web#18892 and vector-im/element-web#18892.

## 🐛 Bug Fixes
 * Fix spacing for message composer buttons ([\#6854](https://github.com/matrix-org/matrix-react-sdk/pull/6854)).
 * Fix accessing field on oobData which may be undefined ([\#6830](https://github.com/matrix-org/matrix-react-sdk/pull/6830)). Fixes vector-im/element-web#19085 and vector-im/element-web#19085.
 * Fix reactions aria-label not being a string and thus being read as [Object object] ([\#6828](https://github.com/matrix-org/matrix-react-sdk/pull/6828)).
 * Fix missing null guard in space hierarchy pagination ([\#6821](https://github.com/matrix-org/matrix-react-sdk/pull/6821)). Fixes matrix-org/element-web-rageshakes#6299 and matrix-org/element-web-rageshakes#6299.
 * Fix checks to show prompt to start new chats ([\#6812](https://github.com/matrix-org/matrix-react-sdk/pull/6812)).
 * Fix room list scroll jumps ([\#6777](https://github.com/matrix-org/matrix-react-sdk/pull/6777)). Fixes vector-im/element-web#17460 vector-im/element-web#18440 and vector-im/element-web#17460. Contributed by [robintown](https://github.com/robintown).
 * Fix various message bubble alignment issues ([\#6785](https://github.com/matrix-org/matrix-react-sdk/pull/6785)). Fixes vector-im/element-web#18293, vector-im/element-web#18294 vector-im/element-web#18305 and vector-im/element-web#18293. Contributed by [robintown](https://github.com/robintown).
 * Make message bubble font size consistent ([\#6795](https://github.com/matrix-org/matrix-react-sdk/pull/6795)). Contributed by [robintown](https://github.com/robintown).
 * Fix edge cases around joining new room which does not belong to active space ([\#6797](https://github.com/matrix-org/matrix-react-sdk/pull/6797)). Fixes vector-im/element-web#19025 and vector-im/element-web#19025.
 * Fix edge case space issues around creation and initial view ([\#6798](https://github.com/matrix-org/matrix-react-sdk/pull/6798)). Fixes vector-im/element-web#19023 and vector-im/element-web#19023.
 * Stop spinner on space preview if the join fails ([\#6803](https://github.com/matrix-org/matrix-react-sdk/pull/6803)). Fixes vector-im/element-web#19034 and vector-im/element-web#19034.
 * Fix emoji picker and stickerpicker not appearing correctly when opened ([\#6793](https://github.com/matrix-org/matrix-react-sdk/pull/6793)). Fixes vector-im/element-web#19012 and vector-im/element-web#19012. Contributed by [Palid](https://github.com/Palid).
 * Fix autocomplete not having y-scroll ([\#6794](https://github.com/matrix-org/matrix-react-sdk/pull/6794)). Fixes vector-im/element-web#18997 and vector-im/element-web#18997. Contributed by [Palid](https://github.com/Palid).
 * Fix broken edge case with public space creation with no alias ([\#6791](https://github.com/matrix-org/matrix-react-sdk/pull/6791)). Fixes vector-im/element-web#19003 and vector-im/element-web#19003.
 * Redirect from /#/welcome to /#/home if already logged in ([\#6786](https://github.com/matrix-org/matrix-react-sdk/pull/6786)). Fixes vector-im/element-web#18990 and vector-im/element-web#18990. Contributed by [aaronraimist](https://github.com/aaronraimist).
 * Fix build issues from two conflicting PRs landing without merge conflict ([\#6780](https://github.com/matrix-org/matrix-react-sdk/pull/6780)).
 * Render guest settings only in public rooms/spaces ([\#6693](https://github.com/matrix-org/matrix-react-sdk/pull/6693)). Fixes vector-im/element-web#18776 and vector-im/element-web#18776. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix message bubble corners being wrong in the presence of hidden events ([\#6776](https://github.com/matrix-org/matrix-react-sdk/pull/6776)). Fixes vector-im/element-web#18124 and vector-im/element-web#18124. Contributed by [robintown](https://github.com/robintown).
 * Debounce read marker update on scroll ([\#6771](https://github.com/matrix-org/matrix-react-sdk/pull/6771)). Fixes vector-im/element-web#18961 and vector-im/element-web#18961.
 * Use cursor:pointer on space panel buttons ([\#6770](https://github.com/matrix-org/matrix-react-sdk/pull/6770)). Fixes vector-im/element-web#18951 and vector-im/element-web#18951.
 * Fix regressed tab view buttons in space update toast ([\#6761](https://github.com/matrix-org/matrix-react-sdk/pull/6761)). Fixes vector-im/element-web#18781 and vector-im/element-web#18781.

Changes in [1.8.5](https://github.com/vector-im/element-desktop/releases/tag/v1.8.5) (2021-09-14)
=================================================================================================

## ✨ Features
 * Add bubble highlight styling ([\#6582](https://github.com/matrix-org/matrix-react-sdk/pull/6582)). Fixes #18295 and #18295. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Create narrow mode for Composer ([\#6682](https://github.com/matrix-org/matrix-react-sdk/pull/6682)). Fixes #18533 and #18533.
 * Prefer matrix.to alias links over room id in spaces & share ([\#6745](https://github.com/matrix-org/matrix-react-sdk/pull/6745)). Fixes #18796 and #18796.
 * Stop automatic playback of voice messages if a non-voice message is encountered ([\#6728](https://github.com/matrix-org/matrix-react-sdk/pull/6728)). Fixes #18850 and #18850.
 * Show call length during a call ([\#6700](https://github.com/matrix-org/matrix-react-sdk/pull/6700)). Fixes #18566 and #18566. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Serialize and retry mass-leave when leaving space ([\#6737](https://github.com/matrix-org/matrix-react-sdk/pull/6737)). Fixes #18789 and #18789.
 * Improve form handling in and around space creation ([\#6739](https://github.com/matrix-org/matrix-react-sdk/pull/6739)). Fixes #18775 and #18775.
 * Split autoplay GIFs and videos into different settings ([\#6726](https://github.com/matrix-org/matrix-react-sdk/pull/6726)). Fixes #5771 and #5771. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Add autoplay for voice messages ([\#6710](https://github.com/matrix-org/matrix-react-sdk/pull/6710)). Fixes #18804, #18715, #18714 #17961 and #18804.
 * Allow to use basic html to format invite messages ([\#6703](https://github.com/matrix-org/matrix-react-sdk/pull/6703)). Fixes #15738 and #15738. Contributed by [skolmer](https://github.com/skolmer).
 * Allow widgets, when eligible, to interact with more rooms as per MSC2762 ([\#6684](https://github.com/matrix-org/matrix-react-sdk/pull/6684)).
 * Remove arbitrary limits from send/receive events for widgets ([\#6719](https://github.com/matrix-org/matrix-react-sdk/pull/6719)). Fixes #17994 and #17994.
 * Reload suggested rooms if we see the state change down /sync ([\#6715](https://github.com/matrix-org/matrix-react-sdk/pull/6715)). Fixes #18761 and #18761.
 * When creating private spaces, make the initial rooms restricted if supported ([\#6721](https://github.com/matrix-org/matrix-react-sdk/pull/6721)). Fixes #18722 and #18722.
 * Threading exploration work ([\#6658](https://github.com/matrix-org/matrix-react-sdk/pull/6658)). Fixes #18532 and #18532.
 * Default to `Don't leave any` when leaving a space ([\#6697](https://github.com/matrix-org/matrix-react-sdk/pull/6697)). Fixes #18592 and #18592. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Special case redaction event sending from widgets per MSC2762 ([\#6686](https://github.com/matrix-org/matrix-react-sdk/pull/6686)). Fixes #18573 and #18573.
 * Add active speaker indicators ([\#6639](https://github.com/matrix-org/matrix-react-sdk/pull/6639)). Fixes #17627 and #17627. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Increase general app performance by optimizing layers ([\#6644](https://github.com/matrix-org/matrix-react-sdk/pull/6644)). Fixes #18730 and #18730. Contributed by [Palid](https://github.com/Palid).

## 🐛 Bug Fixes
 * Fix autocomplete not having y-scroll ([\#6802](https://github.com/matrix-org/matrix-react-sdk/pull/6802)).
 * Fix emoji picker and stickerpicker not appearing correctly when opened ([\#6801](https://github.com/matrix-org/matrix-react-sdk/pull/6801)).
 * Debounce read marker update on scroll ([\#6774](https://github.com/matrix-org/matrix-react-sdk/pull/6774)).
 * Fix Space creation wizard go to my first room button behaviour ([\#6748](https://github.com/matrix-org/matrix-react-sdk/pull/6748)). Fixes #18764 and #18764.
 * Fix scroll being stuck at bottom ([\#6751](https://github.com/matrix-org/matrix-react-sdk/pull/6751)). Fixes #18903 and #18903.
 * Fix widgets not remembering identity verification when asked to. ([\#6742](https://github.com/matrix-org/matrix-react-sdk/pull/6742)). Fixes #15631 and #15631.
 * Add missing pluralisation i18n strings for Spaces ([\#6738](https://github.com/matrix-org/matrix-react-sdk/pull/6738)). Fixes #18780 and #18780.
 * Make ForgotPassword UX slightly more user friendly ([\#6636](https://github.com/matrix-org/matrix-react-sdk/pull/6636)). Fixes #11531 and #11531. Contributed by [Palid](https://github.com/Palid).
 * Don't context switch room on SpaceStore ready as it can break permalinks ([\#6730](https://github.com/matrix-org/matrix-react-sdk/pull/6730)). Fixes #17974 and #17974.
 * Fix explore rooms button not working during space creation wizard ([\#6729](https://github.com/matrix-org/matrix-react-sdk/pull/6729)). Fixes #18762 and #18762.
 * Fix bug where one party's media would sometimes not be shown ([\#6731](https://github.com/matrix-org/matrix-react-sdk/pull/6731)).
 * Only make the initial space rooms suggested by default ([\#6714](https://github.com/matrix-org/matrix-react-sdk/pull/6714)). Fixes #18760 and #18760.
 * Replace fake username in EventTilePreview with a proper loading state ([\#6702](https://github.com/matrix-org/matrix-react-sdk/pull/6702)). Fixes #15897 and #15897. Contributed by [skolmer](https://github.com/skolmer).
 * Don't send prehistorical events to widgets during decryption at startup ([\#6695](https://github.com/matrix-org/matrix-react-sdk/pull/6695)). Fixes #18060 and #18060.
 * When creating subspaces properly set restricted join rule ([\#6725](https://github.com/matrix-org/matrix-react-sdk/pull/6725)). Fixes #18797 and #18797.
 * Fix the Image View not openning for some pinned messages ([\#6723](https://github.com/matrix-org/matrix-react-sdk/pull/6723)). Fixes #18422 and #18422. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Show autocomplete sections vertically ([\#6722](https://github.com/matrix-org/matrix-react-sdk/pull/6722)). Fixes #18860 and #18860. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix EmojiPicker filtering to lower case emojibase data strings ([\#6717](https://github.com/matrix-org/matrix-react-sdk/pull/6717)). Fixes #18686 and #18686.
 * Clear currentRoomId when viewing home page, fixing document title ([\#6716](https://github.com/matrix-org/matrix-react-sdk/pull/6716)). Fixes #18668 and #18668.
 * Fix membership updates to Spaces not applying in real-time ([\#6713](https://github.com/matrix-org/matrix-react-sdk/pull/6713)). Fixes #18737 and #18737.
 * Don't show a double stacked invite modals when inviting to Spaces ([\#6698](https://github.com/matrix-org/matrix-react-sdk/pull/6698)). Fixes #18745 and #18745. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Remove non-functional DuckDuckGo Autocomplete Provider ([\#6712](https://github.com/matrix-org/matrix-react-sdk/pull/6712)). Fixes #18778 and #18778.
 * Filter members on `MemberList` load ([\#6708](https://github.com/matrix-org/matrix-react-sdk/pull/6708)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix improper voice messages being produced in Firefox and sometimes other browsers. ([\#6696](https://github.com/matrix-org/matrix-react-sdk/pull/6696)). Fixes #18587 and #18587.
 * Fix client forgetting which capabilities a widget was approved for ([\#6685](https://github.com/matrix-org/matrix-react-sdk/pull/6685)). Fixes #18786 and #18786.

Changes in [1.8.4](https://github.com/vector-im/element-desktop/releases/tag/v1.8.4) (2021-09-13)
=================================================================================================

## 🔒 SECURITY FIXES
 * Fix a security issue with message key sharing. See https://matrix.org/blog/2021/09/13/vulnerability-disclosure-key-sharing
   for details.

Changes in [1.8.2](https://github.com/vector-im/element-desktop/releases/tag/v1.8.2) (2021-08-31)
=================================================================================================

## ✨ Features
 * Enable Pipewire support for Wayland screen-sharing ([\#256](https://github.com/vector-im/element-desktop/pull/256)). Fixes vector-im/element-web#18607 and vector-im/element-web#18607. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Documentation for sentry config ([\#18608](https://github.com/vector-im/element-web/pull/18608)). Contributed by [novocaine](https://github.com/novocaine).
 * [Release]Increase general app performance by optimizing layers ([\#6672](https://github.com/matrix-org/matrix-react-sdk/pull/6672)). Fixes vector-im/element-web#18730 and vector-im/element-web#18730. Contributed by [Palid](https://github.com/Palid).
 * Add a warning on E2EE rooms if you try to make them public ([\#5698](https://github.com/matrix-org/matrix-react-sdk/pull/5698)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Allow pagination of the space hierarchy and use new APIs ([\#6507](https://github.com/matrix-org/matrix-react-sdk/pull/6507)). Fixes vector-im/element-web#18089 and vector-im/element-web#18427.
 * Improve emoji in composer ([\#6650](https://github.com/matrix-org/matrix-react-sdk/pull/6650)). Fixes vector-im/element-web#18593 and vector-im/element-web#18593. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Allow playback of replied-to voice message ([\#6629](https://github.com/matrix-org/matrix-react-sdk/pull/6629)). Fixes vector-im/element-web#18599 and vector-im/element-web#18599. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Format autocomplete suggestions vertically ([\#6620](https://github.com/matrix-org/matrix-react-sdk/pull/6620)). Fixes vector-im/element-web#17574 and vector-im/element-web#17574. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Remember last `MemberList` search query per-room ([\#6640](https://github.com/matrix-org/matrix-react-sdk/pull/6640)). Fixes vector-im/element-web#18613 and vector-im/element-web#18613. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Sentry rageshakes ([\#6597](https://github.com/matrix-org/matrix-react-sdk/pull/6597)). Fixes vector-im/element-web#11111 and vector-im/element-web#11111. Contributed by [novocaine](https://github.com/novocaine).
 * Autocomplete has been updated to match modern accessibility standards. Navigate via up/down arrows rather than Tab. Enter or Tab to confirm a suggestion. This should be familiar to Slack & Discord users. You can now use Tab to navigate around the application and do more without touching your mouse. No more accidentally sending half of people's names because the completion didn't fire on Enter! ([\#5659](https://github.com/matrix-org/matrix-react-sdk/pull/5659)). Fixes vector-im/element-web#4872, vector-im/element-web#11071, vector-im/element-web#17171, vector-im/element-web#15646 vector-im/element-web#4872 and vector-im/element-web#4872.
 * Add new call tile states ([\#6610](https://github.com/matrix-org/matrix-react-sdk/pull/6610)). Fixes vector-im/element-web#18521 and vector-im/element-web#18521. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Left align call tiles ([\#6609](https://github.com/matrix-org/matrix-react-sdk/pull/6609)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Make loading encrypted images look snappier ([\#6590](https://github.com/matrix-org/matrix-react-sdk/pull/6590)). Fixes vector-im/element-web#17878 and vector-im/element-web#17862. Contributed by [Palid](https://github.com/Palid).
 * Offer a way to create a space based on existing community ([\#6543](https://github.com/matrix-org/matrix-react-sdk/pull/6543)). Fixes vector-im/element-web#18092.
 * Accessibility improvements in and around Spaces ([\#6569](https://github.com/matrix-org/matrix-react-sdk/pull/6569)). Fixes vector-im/element-web#18094 and vector-im/element-web#18094.

## 🐛 Bug Fixes
 * [Release] Fix commit edit history ([\#6690](https://github.com/matrix-org/matrix-react-sdk/pull/6690)). Fixes vector-im/element-web#18742 and vector-im/element-web#18742. Contributed by [Palid](https://github.com/Palid).
 * Fix images not rendering when sent from other clients. ([\#6661](https://github.com/matrix-org/matrix-react-sdk/pull/6661)). Fixes vector-im/element-web#18702 and vector-im/element-web#18702.
 * Fix autocomplete scrollbar and make the autocomplete a little smaller ([\#6655](https://github.com/matrix-org/matrix-react-sdk/pull/6655)). Fixes vector-im/element-web#18682 and vector-im/element-web#18682. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix replies on the bubble layout ([\#6451](https://github.com/matrix-org/matrix-react-sdk/pull/6451)). Fixes vector-im/element-web#18184. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Show "Enable encryption in settings" only when the user can do that ([\#6646](https://github.com/matrix-org/matrix-react-sdk/pull/6646)). Fixes vector-im/element-web#18646 and vector-im/element-web#18646. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix cross signing setup from settings screen ([\#6633](https://github.com/matrix-org/matrix-react-sdk/pull/6633)). Fixes vector-im/element-web#17761 and vector-im/element-web#17761.
 * Fix call tiles on the bubble layout ([\#6647](https://github.com/matrix-org/matrix-react-sdk/pull/6647)). Fixes vector-im/element-web#18648 and vector-im/element-web#18648. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix error on accessing encrypted media without encryption keys ([\#6625](https://github.com/matrix-org/matrix-react-sdk/pull/6625)). Contributed by [Palid](https://github.com/Palid).
 * Fix jitsi widget sometimes being permanently stuck in the bottom-right corner ([\#6632](https://github.com/matrix-org/matrix-react-sdk/pull/6632)). Fixes vector-im/element-web#17226 and vector-im/element-web#17226. Contributed by [Palid](https://github.com/Palid).
 * Fix FilePanel pagination in E2EE rooms ([\#6630](https://github.com/matrix-org/matrix-react-sdk/pull/6630)). Fixes vector-im/element-web#18415 and vector-im/element-web#18415. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix call tile buttons ([\#6624](https://github.com/matrix-org/matrix-react-sdk/pull/6624)). Fixes vector-im/element-web#18565 and vector-im/element-web#18565. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix vertical call tile spacing issues ([\#6621](https://github.com/matrix-org/matrix-react-sdk/pull/6621)). Fixes vector-im/element-web#18558 and vector-im/element-web#18558. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix long display names in call tiles ([\#6618](https://github.com/matrix-org/matrix-react-sdk/pull/6618)). Fixes vector-im/element-web#18562 and vector-im/element-web#18562. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Avoid access token overflow ([\#6616](https://github.com/matrix-org/matrix-react-sdk/pull/6616)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Properly handle media errors  ([\#6615](https://github.com/matrix-org/matrix-react-sdk/pull/6615)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix glare related regressions ([\#6614](https://github.com/matrix-org/matrix-react-sdk/pull/6614)). Fixes vector-im/element-web#18538 and vector-im/element-web#18538. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix long display names in call toasts ([\#6617](https://github.com/matrix-org/matrix-react-sdk/pull/6617)). Fixes vector-im/element-web#18557 and vector-im/element-web#18557. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix PiP of held calls ([\#6611](https://github.com/matrix-org/matrix-react-sdk/pull/6611)). Fixes vector-im/element-web#18539 and vector-im/element-web#18539. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix call tile behaviour on narrow layouts ([\#6556](https://github.com/matrix-org/matrix-react-sdk/pull/6556)). Fixes vector-im/element-web#18398. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix video call persisting when widget removed ([\#6608](https://github.com/matrix-org/matrix-react-sdk/pull/6608)). Fixes vector-im/element-web#15703 and vector-im/element-web#15703.
 * Fix toast colors ([\#6606](https://github.com/matrix-org/matrix-react-sdk/pull/6606)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Remove tiny scrollbar dot from code blocks ([\#6596](https://github.com/matrix-org/matrix-react-sdk/pull/6596)). Fixes vector-im/element-web#18474. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Improve handling of pills in the composer ([\#6353](https://github.com/matrix-org/matrix-react-sdk/pull/6353)). Fixes vector-im/element-web#10134 vector-im/element-web#10896 and vector-im/element-web#15037. Contributed by [SimonBrandner](https://github.com/SimonBrandner).

Changes in [1.8.1](https://github.com/vector-im/element-desktop/releases/tag/v1.8.1) (2021-08-17)
=================================================================================================

## 🐛 Bug Fixes
 * Fix multiple VoIP regressions ([matrix-org/matrix-js-sdk#1860](https://github.com/matrix-org/matrix-js-sdk/pull/1860)).

Changes in [1.8.0](https://github.com/vector-im/element-desktop/releases/tag/v1.8.0) (2021-08-16)
=================================================================================================

## ✨ Features
 * Show how long a call was on call tiles ([\#6570](https://github.com/matrix-org/matrix-react-sdk/pull/6570)). Fixes vector-im/element-web#18405. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Add regional indicators to emoji picker ([\#6490](https://github.com/matrix-org/matrix-react-sdk/pull/6490)). Fixes vector-im/element-web#14963. Contributed by [robintown](https://github.com/robintown).
 * Make call control buttons accessible to screen reader users ([\#6181](https://github.com/matrix-org/matrix-react-sdk/pull/6181)). Fixes vector-im/element-web#18358. Contributed by [pvagner](https://github.com/pvagner).
 * Skip sending a thumbnail if it is not a sufficient saving over the original ([\#6559](https://github.com/matrix-org/matrix-react-sdk/pull/6559)). Fixes vector-im/element-web#17906.
 * Increase PiP snapping speed ([\#6539](https://github.com/matrix-org/matrix-react-sdk/pull/6539)). Fixes vector-im/element-web#18371. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Improve and move the incoming call toast ([\#6470](https://github.com/matrix-org/matrix-react-sdk/pull/6470)). Fixes vector-im/element-web#17912. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Allow all of the URL schemes that Firefox allows ([\#6457](https://github.com/matrix-org/matrix-react-sdk/pull/6457)). Contributed by [aaronraimist](https://github.com/aaronraimist).
 * Improve bubble layout colors ([\#6452](https://github.com/matrix-org/matrix-react-sdk/pull/6452)). Fixes vector-im/element-web#18081. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Spaces let users switch between Home and All Rooms behaviours ([\#6497](https://github.com/matrix-org/matrix-react-sdk/pull/6497)). Fixes vector-im/element-web#18093.
 * Support for MSC2285 (hidden read receipts) ([\#6390](https://github.com/matrix-org/matrix-react-sdk/pull/6390)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Group pinned message events with MELS ([\#6349](https://github.com/matrix-org/matrix-react-sdk/pull/6349)). Fixes vector-im/element-web#17938. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Make version copiable ([\#6227](https://github.com/matrix-org/matrix-react-sdk/pull/6227)). Fixes vector-im/element-web#17603 and vector-im/element-web#18329. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Improve voice messages uploading state ([\#6530](https://github.com/matrix-org/matrix-react-sdk/pull/6530)). Fixes vector-im/element-web#18226 and vector-im/element-web#18224.
 * Add surround with feature ([\#5510](https://github.com/matrix-org/matrix-react-sdk/pull/5510)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Improve call event tile wording ([\#6545](https://github.com/matrix-org/matrix-react-sdk/pull/6545)). Fixes vector-im/element-web#18376. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Show an avatar/a turned off microphone icon for muted users ([\#6486](https://github.com/matrix-org/matrix-react-sdk/pull/6486)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Prompt user to leave rooms/subspaces in a space when leaving space ([\#6424](https://github.com/matrix-org/matrix-react-sdk/pull/6424)). Fixes vector-im/element-web#18071.
 * Add customisation point to override widget variables ([\#6455](https://github.com/matrix-org/matrix-react-sdk/pull/6455)). Fixes vector-im/element-web#18035.
 * Add support for screen sharing in 1:1 calls ([\#5992](https://github.com/matrix-org/matrix-react-sdk/pull/5992)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).

## 🐛 Bug Fixes
 * Dismiss electron download toast when clicking Open ([\#18267](https://github.com/vector-im/element-web/pull/18267)). Fixes vector-im/element-web#18266.
 * [Release] Fix glare related regressions ([\#6622](https://github.com/matrix-org/matrix-react-sdk/pull/6622)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * [Release] Fix PiP of held calls ([\#6612](https://github.com/matrix-org/matrix-react-sdk/pull/6612)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * [Release] Fix toast colors ([\#6607](https://github.com/matrix-org/matrix-react-sdk/pull/6607)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix [object Object] in Widget Permissions ([\#6560](https://github.com/matrix-org/matrix-react-sdk/pull/6560)). Fixes vector-im/element-web#18384. Contributed by [Palid](https://github.com/Palid).
 * Fix right margin for events on IRC layout ([\#6542](https://github.com/matrix-org/matrix-react-sdk/pull/6542)). Fixes vector-im/element-web#18354.
 * Mirror only usermedia feeds ([\#6512](https://github.com/matrix-org/matrix-react-sdk/pull/6512)). Fixes vector-im/element-web#5633. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix LogoutDialog warning + TypeScript migration ([\#6533](https://github.com/matrix-org/matrix-react-sdk/pull/6533)).
 * Fix the wrong font being used in the room topic field ([\#6527](https://github.com/matrix-org/matrix-react-sdk/pull/6527)). Fixes vector-im/element-web#18339. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix inconsistent styling for links on hover ([\#6513](https://github.com/matrix-org/matrix-react-sdk/pull/6513)). Contributed by [janogarcia](https://github.com/janogarcia).
 * Fix incorrect height for encoded placeholder images ([\#6514](https://github.com/matrix-org/matrix-react-sdk/pull/6514)). Contributed by [Palid](https://github.com/Palid).
 * Fix call events layout for message bubble ([\#6465](https://github.com/matrix-org/matrix-react-sdk/pull/6465)). Fixes vector-im/element-web#18144.
 * Improve subspaces and some utilities around room/space creation ([\#6458](https://github.com/matrix-org/matrix-react-sdk/pull/6458)). Fixes vector-im/element-web#18090 vector-im/element-web#18091 and vector-im/element-web#17256.
 * Restore pointer cursor for SenderProfile in message bubbles ([\#6501](https://github.com/matrix-org/matrix-react-sdk/pull/6501)). Fixes vector-im/element-web#18249.
 * Fix issues with the Call View ([\#6472](https://github.com/matrix-org/matrix-react-sdk/pull/6472)). Fixes vector-im/element-web#18221. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Align event list summary read receipts when using message bubbles ([\#6500](https://github.com/matrix-org/matrix-react-sdk/pull/6500)). Fixes vector-im/element-web#18143.
 * Better positioning for unbubbled events in timeline ([\#6477](https://github.com/matrix-org/matrix-react-sdk/pull/6477)). Fixes vector-im/element-web#18132.
 * Realign reactions row with messages in modern layout ([\#6491](https://github.com/matrix-org/matrix-react-sdk/pull/6491)). Fixes vector-im/element-web#18118. Contributed by [robintown](https://github.com/robintown).
 * Fix CreateRoomDialog exploding when making public room outside of a space ([\#6492](https://github.com/matrix-org/matrix-react-sdk/pull/6492)). Fixes vector-im/element-web#18275.
 * Fix call crashing because `element` was undefined ([\#6488](https://github.com/matrix-org/matrix-react-sdk/pull/6488)). Fixes vector-im/element-web#18270. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Upscale thumbnails to the container size ([\#6589](https://github.com/matrix-org/matrix-react-sdk/pull/6589)). Fixes vector-im/element-web#18307.
 * Fix create room dialog in spaces no longer adding to the space ([\#6587](https://github.com/matrix-org/matrix-react-sdk/pull/6587)). Fixes vector-im/element-web#18465.
 * Don't show a modal on call reject/user hangup ([\#6580](https://github.com/matrix-org/matrix-react-sdk/pull/6580)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fade Call View Buttons after `componentDidMount` ([\#6581](https://github.com/matrix-org/matrix-react-sdk/pull/6581)). Fixes vector-im/element-web#18439. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix missing expand button on codeblocks ([\#6565](https://github.com/matrix-org/matrix-react-sdk/pull/6565)). Fixes vector-im/element-web#18388. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * allow customizing the bubble layout colors ([\#6568](https://github.com/matrix-org/matrix-react-sdk/pull/6568)). Fixes vector-im/element-web#18408. Contributed by [benneti](https://github.com/benneti).
 * Don't flash "Missed call" when accepting a call ([\#6567](https://github.com/matrix-org/matrix-react-sdk/pull/6567)). Fixes vector-im/element-web#18404. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix clicking whitespaces on replies ([\#6571](https://github.com/matrix-org/matrix-react-sdk/pull/6571)). Fixes vector-im/element-web#18327. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix disabled state for voice messages + send button tooltip ([\#6562](https://github.com/matrix-org/matrix-react-sdk/pull/6562)). Fixes vector-im/element-web#18413.
 * Fix voice feed being cut-off ([\#6550](https://github.com/matrix-org/matrix-react-sdk/pull/6550)). Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix sizing issues of the screen picker ([\#6498](https://github.com/matrix-org/matrix-react-sdk/pull/6498)). Fixes vector-im/element-web#18281. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Stop voice messages that are playing when starting a recording ([\#6563](https://github.com/matrix-org/matrix-react-sdk/pull/6563)). Fixes vector-im/element-web#18410.
 * Properly set style attribute on shared usercontent iframe ([\#6561](https://github.com/matrix-org/matrix-react-sdk/pull/6561)). Fixes vector-im/element-web#18414.
 * Null guard space inviter to prevent the app exploding ([\#6558](https://github.com/matrix-org/matrix-react-sdk/pull/6558)).
 * Make the ringing sound mutable/disablable ([\#6534](https://github.com/matrix-org/matrix-react-sdk/pull/6534)). Fixes vector-im/element-web#15591. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix wrong cursor being used in PiP ([\#6551](https://github.com/matrix-org/matrix-react-sdk/pull/6551)). Fixes vector-im/element-web#18383. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Re-pin Jitsi if the widget already exists ([\#6226](https://github.com/matrix-org/matrix-react-sdk/pull/6226)). Fixes vector-im/element-web#17679. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix broken call notification regression ([\#6526](https://github.com/matrix-org/matrix-react-sdk/pull/6526)). Fixes vector-im/element-web#18335. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * createRoom, only send join rule event if we have a join rule to put in it ([\#6516](https://github.com/matrix-org/matrix-react-sdk/pull/6516)). Fixes vector-im/element-web#18301.
 * Fix clicking pills inside replies ([\#6508](https://github.com/matrix-org/matrix-react-sdk/pull/6508)). Fixes vector-im/element-web#18283. Contributed by [SimonBrandner](https://github.com/SimonBrandner).
 * Fix grecaptcha regression ([\#6503](https://github.com/matrix-org/matrix-react-sdk/pull/6503)). Fixes vector-im/element-web#18284. Contributed by [Palid](https://github.com/Palid).

Changes in [1.7.34](https://github.com/vector-im/element-desktop/releases/tag/v1.7.34) (2021-08-02)
===================================================================================================

## 🔒 SECURITY FIXES
 * Sanitize untrusted variables from message previews before translation
   Fixes vector-im/element-web#18314

## ✨ Features
 * Fix editing of `<sub>` & `<sup`> & `<u>`
   [\#6469](https://github.com/matrix-org/matrix-react-sdk/pull/6469)
   Fixes vector-im/element-web#18211
 * Zoom images in lightbox to where the cursor points
   [\#6418](https://github.com/matrix-org/matrix-react-sdk/pull/6418)
   Fixes vector-im/element-web#17870
 * Avoid hitting the settings store from TextForEvent
   [\#6205](https://github.com/matrix-org/matrix-react-sdk/pull/6205)
   Fixes vector-im/element-web#17650
 * Initial MSC3083 + MSC3244 support
   [\#6212](https://github.com/matrix-org/matrix-react-sdk/pull/6212)
   Fixes vector-im/element-web#17686 and vector-im/element-web#17661
 * Navigate to the first room with notifications when clicked on space notification dot
   [\#5974](https://github.com/matrix-org/matrix-react-sdk/pull/5974)
 * Add matrix: to the list of permitted URL schemes
   [\#6388](https://github.com/matrix-org/matrix-react-sdk/pull/6388)
 * Add "Copy Link" to room context menu
   [\#6374](https://github.com/matrix-org/matrix-react-sdk/pull/6374)
 * 💭 Message bubble layout
   [\#6291](https://github.com/matrix-org/matrix-react-sdk/pull/6291)
   Fixes vector-im/element-web#4635, vector-im/element-web#17773 vector-im/element-web#16220 and vector-im/element-web#7687
 * Play only one audio file at a time
   [\#6417](https://github.com/matrix-org/matrix-react-sdk/pull/6417)
   Fixes vector-im/element-web#17439
 * Move download button for media to the action bar
   [\#6386](https://github.com/matrix-org/matrix-react-sdk/pull/6386)
   Fixes vector-im/element-web#17943
 * Improved display of one-to-one call history with summary boxes for each call
   [\#6121](https://github.com/matrix-org/matrix-react-sdk/pull/6121)
   Fixes vector-im/element-web#16409
 * Notification settings UI refresh
   [\#6352](https://github.com/matrix-org/matrix-react-sdk/pull/6352)
   Fixes vector-im/element-web#17782
 * Fix EventIndex double handling events and erroring
   [\#6385](https://github.com/matrix-org/matrix-react-sdk/pull/6385)
   Fixes vector-im/element-web#18008
 * Improve reply rendering
   [\#3553](https://github.com/matrix-org/matrix-react-sdk/pull/3553)
   Fixes vector-im/riot-web#9217, vector-im/riot-web#7633, vector-im/riot-web#7530, vector-im/riot-web#7169, vector-im/riot-web#7151, vector-im/riot-web#6692 vector-im/riot-web#6579 and vector-im/element-web#17440

## 🐛 Bug Fixes
 * Fix browser history getting stuck looping back to the same room
   [\#18053](https://github.com/vector-im/element-web/pull/18053)
 * Fix space shortcuts on layouts with non-English keys in the places of numbers
   [\#17780](https://github.com/vector-im/element-web/pull/17780)
   Fixes vector-im/element-web#17776
 * Fix CreateRoomDialog exploding when making public room outside of a space
   [\#6493](https://github.com/matrix-org/matrix-react-sdk/pull/6493)
 * Fix regression where registration would soft-crash on captcha
   [\#6505](https://github.com/matrix-org/matrix-react-sdk/pull/6505)
   Fixes vector-im/element-web#18284
 * only send join rule event if we have a join rule to put in it
   [\#6517](https://github.com/matrix-org/matrix-react-sdk/pull/6517)
 * Improve the new download button's discoverability and interactions.
   [\#6510](https://github.com/matrix-org/matrix-react-sdk/pull/6510)
 * Fix voice recording UI looking broken while microphone permissions are being requested.
   [\#6479](https://github.com/matrix-org/matrix-react-sdk/pull/6479)
   Fixes vector-im/element-web#18223
 * Match colors of room and user avatars in DMs
   [\#6393](https://github.com/matrix-org/matrix-react-sdk/pull/6393)
   Fixes vector-im/element-web#2449
 * Fix onPaste handler to work with copying files from Finder
   [\#5389](https://github.com/matrix-org/matrix-react-sdk/pull/5389)
   Fixes vector-im/element-web#15536 and vector-im/element-web#16255
 * Fix infinite pagination loop when offline
   [\#6478](https://github.com/matrix-org/matrix-react-sdk/pull/6478)
   Fixes vector-im/element-web#18242
 * Fix blurhash rounded corners missing regression
   [\#6467](https://github.com/matrix-org/matrix-react-sdk/pull/6467)
   Fixes vector-im/element-web#18110
 * Fix position of the space hierarchy spinner
   [\#6462](https://github.com/matrix-org/matrix-react-sdk/pull/6462)
   Fixes vector-im/element-web#18182
 * Fix display of image messages that lack thumbnails
   [\#6456](https://github.com/matrix-org/matrix-react-sdk/pull/6456)
   Fixes vector-im/element-web#18175
 * Fix crash with large audio files.
   [\#6436](https://github.com/matrix-org/matrix-react-sdk/pull/6436)
   Fixes vector-im/element-web#18149
 * Make diff colors in codeblocks more pleasant
   [\#6355](https://github.com/matrix-org/matrix-react-sdk/pull/6355)
   Fixes vector-im/element-web#17939
 * Show the correct audio file duration while loading the file.
   [\#6435](https://github.com/matrix-org/matrix-react-sdk/pull/6435)
   Fixes vector-im/element-web#18160
 * Fix various timeline settings not applying immediately.
   [\#6261](https://github.com/matrix-org/matrix-react-sdk/pull/6261)
   Fixes vector-im/element-web#17748
 * Fix issues with room list duplication
   [\#6391](https://github.com/matrix-org/matrix-react-sdk/pull/6391)
   Fixes vector-im/element-web#14508
 * Fix grecaptcha throwing useless error sometimes
   [\#6401](https://github.com/matrix-org/matrix-react-sdk/pull/6401)
   Fixes vector-im/element-web#15142
 * Update Emojibase and Twemoji and switch to IamCal (Slack-style) shortcodes
   [\#6347](https://github.com/matrix-org/matrix-react-sdk/pull/6347)
   Fixes vector-im/element-web#13857 and vector-im/element-web#13334
 * Respect compound emojis in default avatar initial generation
   [\#6397](https://github.com/matrix-org/matrix-react-sdk/pull/6397)
   Fixes vector-im/element-web#18040
 * Fix bug where the 'other homeserver' field in the server selection dialog would become briefly focus and then unfocus when clicked.
   [\#6394](https://github.com/matrix-org/matrix-react-sdk/pull/6394)
   Fixes vector-im/element-web#18031
 * Standardise spelling and casing of homeserver, identity server, and integration manager 
   [\#6365](https://github.com/matrix-org/matrix-react-sdk/pull/6365)
 * Fix widgets not receiving decrypted events when they have permission.
   [\#6371](https://github.com/matrix-org/matrix-react-sdk/pull/6371)
   Fixes vector-im/element-web#17615
 * Prevent client hangs when calculating blurhashes
   [\#6366](https://github.com/matrix-org/matrix-react-sdk/pull/6366)
   Fixes vector-im/element-web#17945
 * Exclude state events from widgets reading room events
   [\#6378](https://github.com/matrix-org/matrix-react-sdk/pull/6378)
 * Cache feature_spaces\* flags to improve performance
   [\#6381](https://github.com/matrix-org/matrix-react-sdk/pull/6381)

Changes in [1.7.33](https://github.com/vector-im/element-desktop/releases/tag/v1.7.33) (2021-07-19)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.32...v1.7.33)

 * Translations update from Weblate
   [\#232](https://github.com/vector-im/element-desktop/pull/232)
 * Add VS Code to gitignore
   [\#231](https://github.com/vector-im/element-desktop/pull/231)
 * Use the target-specific build dir for sqlcipher / openssl
   [\#230](https://github.com/vector-im/element-desktop/pull/230)
 * Fix not specifying a target
   [\#229](https://github.com/vector-im/element-desktop/pull/229)
 * Do not generate a lockfile when running in CI
   [\#227](https://github.com/vector-im/element-desktop/pull/227)
 * Use double quotes in readme
   [\#228](https://github.com/vector-im/element-desktop/pull/228)
 * Support universal builds
   [\#226](https://github.com/vector-im/element-desktop/pull/226)
 * Check target with rustc directly
   [\#225](https://github.com/vector-im/element-desktop/pull/225)

Changes in [1.7.32](https://github.com/vector-im/element-desktop/releases/tag/v1.7.32) (2021-07-05)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.31...v1.7.32)

 * Fix the build: make the rootDir correct
   [\#224](https://github.com/vector-im/element-desktop/pull/224)
 * Fix i18n in Element Desktop
   [\#223](https://github.com/vector-im/element-desktop/pull/223)
 * Convert preload.js to Typescript so that it gets copied to `lib`
   [\#222](https://github.com/vector-im/element-desktop/pull/222)
 * Bundle the `lib` dir now, not `src`
   [\#221](https://github.com/vector-im/element-desktop/pull/221)
 * Initial Typescripting for Element Desktop
   [\#219](https://github.com/vector-im/element-desktop/pull/219)
 * Translations update from Weblate
   [\#220](https://github.com/vector-im/element-desktop/pull/220)
 * Fix Windows target arch in native build
   [\#218](https://github.com/vector-im/element-desktop/pull/218)
 * Add libera.chat to default room directory
   [\#217](https://github.com/vector-im/element-desktop/pull/217)
 * Add update and native build support for Apple silicon
   [\#216](https://github.com/vector-im/element-desktop/pull/216)
 * Add numpad accelerators for zooming
   [\#203](https://github.com/vector-im/element-desktop/pull/203)
 * Add warning dialog when custom config.json is invalid
   [\#201](https://github.com/vector-im/element-desktop/pull/201)
 * Don't show Quit warning on keyUp residual event
   [\#215](https://github.com/vector-im/element-desktop/pull/215)
 * Fix accelerator for save-image-as clashing with copy-link-address
   [\#213](https://github.com/vector-im/element-desktop/pull/213)

Changes in [1.7.31](https://github.com/vector-im/element-desktop/releases/tag/v1.7.31) (2021-06-21)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.31-rc.1...v1.7.31)

 * No changes since rc.1

Changes in [1.7.31-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.31-rc.1) (2021-06-15)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.30...v1.7.31-rc.1)

 * Upgrade to Electron 12.0.11
   [\#211](https://github.com/vector-im/element-desktop/pull/211)
 * Translations update from Weblate
   [\#214](https://github.com/vector-im/element-desktop/pull/214)
 * Upgrade to Node 14
   [\#212](https://github.com/vector-im/element-desktop/pull/212)
 * Bump npm-registry-fetch from 4.0.2 to 4.0.7
   [\#210](https://github.com/vector-im/element-desktop/pull/210)
 * Update electron-builder for Node 16 compatibility
   [\#204](https://github.com/vector-im/element-desktop/pull/204)
 * Bump hosted-git-info from 2.8.5 to 2.8.9
   [\#209](https://github.com/vector-im/element-desktop/pull/209)
 * Bump glob-parent from 5.1.1 to 5.1.2
   [\#206](https://github.com/vector-im/element-desktop/pull/206)
 * Bump dot-prop from 4.2.0 to 4.2.1
   [\#208](https://github.com/vector-im/element-desktop/pull/208)
 * Bump y18n from 3.2.1 to 3.2.2
   [\#207](https://github.com/vector-im/element-desktop/pull/207)
 * Bump normalize-url from 4.5.0 to 4.5.1
   [\#205](https://github.com/vector-im/element-desktop/pull/205)
 * Put Preferences menu item in correct location on macOS
   [\#200](https://github.com/vector-im/element-desktop/pull/200)
 * Switch zoomIn accelerator to default
   [\#202](https://github.com/vector-im/element-desktop/pull/202)

Changes in [1.7.30](https://github.com/vector-im/element-desktop/releases/tag/v1.7.30) (2021-06-07)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.30-rc.1...v1.7.30)

 * No changes since rc.1

Changes in [1.7.30-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.30-rc.1) (2021-06-01)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.29...v1.7.30-rc.1)

 * Translations update from Weblate
   [\#199](https://github.com/vector-im/element-desktop/pull/199)
 * Migrate to `eslint-plugin-matrix-org`
   [\#197](https://github.com/vector-im/element-desktop/pull/197)
 * Upgrade to Electron 12.0.9
   [\#198](https://github.com/vector-im/element-desktop/pull/198)

Changes in [1.7.29](https://github.com/vector-im/element-desktop/releases/tag/v1.7.29) (2021-05-24)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.29-rc.1...v1.7.29)

 * No changes since rc.1

Changes in [1.7.29-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.29-rc.1) (2021-05-19)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.28...v1.7.29-rc.1)

 * Translations update from Weblate
   [\#196](https://github.com/vector-im/element-desktop/pull/196)
 * Translations update from Weblate
   [\#195](https://github.com/vector-im/element-desktop/pull/195)

Changes in [1.7.28](https://github.com/vector-im/element-desktop/releases/tag/v1.7.28) (2021-05-17)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.28-rc.1...v1.7.28)

 * No changes since rc.1

Changes in [1.7.28-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.28-rc.1) (2021-05-11)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.27...v1.7.28-rc.1)

 * Add Windows native module requirements
   [\#190](https://github.com/vector-im/element-desktop/pull/190)
 * Prevent black screen when closing window while in full screen mode on macOS
   [\#192](https://github.com/vector-im/element-desktop/pull/192)

Changes in [1.7.27](https://github.com/vector-im/element-desktop/releases/tag/v1.7.27) (2021-05-10)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.27-rc.1...v1.7.27)

 * No changes since rc.1

Changes in [1.7.27-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.27-rc.1) (2021-05-04)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.26...v1.7.27-rc.1)

 * Translations update from Weblate
   [\#191](https://github.com/vector-im/element-desktop/pull/191)
 * Bump ssri from 6.0.1 to 6.0.2
   [\#187](https://github.com/vector-im/element-desktop/pull/187)
 * Disables HardwareMediaKeyHandling
   [\#180](https://github.com/vector-im/element-desktop/pull/180)
 * Translations update from Weblate
   [\#189](https://github.com/vector-im/element-desktop/pull/189)
 * Add internationalisation support
   [\#188](https://github.com/vector-im/element-desktop/pull/188)
 * Fix event index passphrase change process
   [\#186](https://github.com/vector-im/element-desktop/pull/186)

Changes in [1.7.26](https://github.com/vector-im/element-desktop/releases/tag/v1.7.26) (2021-04-26)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.26-rc.1...v1.7.26)

 * No changes since rc.1

Changes in [1.7.26-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.26-rc.1) (2021-04-21)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.25...v1.7.26-rc.1)

 * Remove Debian dependency libappindicator3-1
   [\#170](https://github.com/vector-im/element-desktop/pull/170)
 * Fix exit shortcuts for non QWERTY keyboards
   [\#185](https://github.com/vector-im/element-desktop/pull/185)
 * Fix using yarn run fetch with a specific version
   [\#182](https://github.com/vector-im/element-desktop/pull/182)
 * Switch nightly to not-staging Scalar by default
   [\#181](https://github.com/vector-im/element-desktop/pull/181)

Changes in [1.7.25](https://github.com/vector-im/element-desktop/releases/tag/v1.7.25) (2021-04-12)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.25-rc.1...v1.7.25)

 * No changes since rc.1

Changes in [1.7.25-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.25-rc.1) (2021-04-07)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.24...v1.7.25-rc.1)

 * Fix disabling spellchecker
   [\#179](https://github.com/vector-im/element-desktop/pull/179)
 * Upgrade to Electron 12.0.2
   [\#178](https://github.com/vector-im/element-desktop/pull/178)
 * Avoid exit listener to hijack other application shortcuts
   [\#177](https://github.com/vector-im/element-desktop/pull/177)
 * Migrate native-node-modules docs to element-desktop
   [\#176](https://github.com/vector-im/element-desktop/pull/176)
 * Add prompt to warn before quitting the application
   [\#173](https://github.com/vector-im/element-desktop/pull/173)
 * Upgrade to Electron 11.4.1
   [\#172](https://github.com/vector-im/element-desktop/pull/172)
 * Fix docker:build:native documentation typo
   [\#174](https://github.com/vector-im/element-desktop/pull/174)

Changes in [1.7.24](https://github.com/vector-im/element-desktop/releases/tag/v1.7.24) (2021-03-29)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.24-rc.1...v1.7.24)

 * No changes since rc.1

Changes in [1.7.24-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.24-rc.1) (2021-03-25)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.23...v1.7.24-rc.1)

 * No changes since 1.7.23

Changes in [1.7.23](https://github.com/vector-im/element-desktop/releases/tag/v1.7.23) (2021-03-15)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.23-rc.1...v1.7.23)

 * No changes since rc.1

Changes in [1.7.23-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.23-rc.1) (2021-03-11)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.22...v1.7.23-rc.1)

 * Fix disabling spell-checker
   [\#171](https://github.com/vector-im/element-desktop/pull/171)
 * Add multi language spell check
   [\#154](https://github.com/vector-im/element-desktop/pull/154)

Changes in [1.7.22](https://github.com/vector-im/element-desktop/releases/tag/v1.7.22) (2021-03-01)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.22-rc.1...v1.7.22)

 * No changes since rc.1

Changes in [1.7.22-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.22-rc.1) (2021-02-24)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.21...v1.7.22-rc.1)

 * Disable Countly
   [\#169](https://github.com/vector-im/element-desktop/pull/169)
 * Upgrade to Electron 11.2.3
   [\#168](https://github.com/vector-im/element-desktop/pull/168)

Changes in [1.7.21](https://github.com/vector-im/element-desktop/releases/tag/v1.7.21) (2021-02-16)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.21-rc.1...v1.7.21)

 * No changes since rc.1

Changes in [1.7.21-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.21-rc.1) (2021-02-10)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.20...v1.7.21-rc.1)

 * Fix desktop Matrix screen sharing
   [\#161](https://github.com/vector-im/element-desktop/pull/161)

Changes in [1.7.20](https://github.com/vector-im/element-desktop/releases/tag/v1.7.20) (2021-02-04)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.19...v1.7.20)

 * No changes since 1.7.19

Changes in [1.7.19](https://github.com/vector-im/element-desktop/releases/tag/v1.7.19) (2021-02-03)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.19-rc.1...v1.7.19)

 * No changes since rc.1

Changes in [1.7.19-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.19-rc.1) (2021-01-29)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.18...v1.7.19-rc.1)

 * Remove Buildkite pipeline file
   [\#167](https://github.com/vector-im/element-desktop/pull/167)
 * Upgrade deps 2021-01-18
   [\#166](https://github.com/vector-im/element-desktop/pull/166)
 * package: Bump our seshat version
   [\#164](https://github.com/vector-im/element-desktop/pull/164)
 * Enable context isolation, bridge expected IPC
   [\#163](https://github.com/vector-im/element-desktop/pull/163)

Changes in [1.7.18](https://github.com/vector-im/element-desktop/releases/tag/v1.7.18) (2021-01-26)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.17...v1.7.18)

 * No changes since 1.7.17

Changes in [1.7.17](https://github.com/vector-im/element-desktop/releases/tag/v1.7.17) (2021-01-18)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.17-rc.1...v1.7.17)

 * [Release] package: Bump our seshat version
   [\#165](https://github.com/vector-im/element-desktop/pull/165)

Changes in [1.7.17-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.17-rc.1) (2021-01-13)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.16...v1.7.17-rc.1)

 * package: Bump our Seshat version
   [\#162](https://github.com/vector-im/element-desktop/pull/162)
 * Upgrade to Electron 10.2.0
   [\#159](https://github.com/vector-im/element-desktop/pull/159)

Changes in [1.7.16](https://github.com/vector-im/element-desktop/releases/tag/v1.7.16) (2020-12-21)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.16-rc.1...v1.7.16)

 * No changes since rc.1

Changes in [1.7.16-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.16-rc.1) (2020-12-16)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.15...v1.7.16-rc.1)

 * Bump ini from 1.3.5 to 1.3.8
   [\#158](https://github.com/vector-im/element-desktop/pull/158)
 * Add gitter.im to room directory
   [\#157](https://github.com/vector-im/element-desktop/pull/157)

Changes in [1.7.15](https://github.com/vector-im/element-desktop/releases/tag/v1.7.15) (2020-12-07)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.15-rc.1...v1.7.15)

 * No changes since rc.1

Changes in [1.7.15-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.15-rc.1) (2020-12-02)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.14...v1.7.15-rc.1)

 * No changes since 1.7.14

Changes in [1.7.14](https://github.com/vector-im/element-desktop/releases/tag/v1.7.14) (2020-11-23)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.14-rc.1...v1.7.14)

 * No changes since rc.1

Changes in [1.7.14-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.14-rc.1) (2020-11-18)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.13...v1.7.14-rc.1)

 * Correct spelling mistakes
   [\#151](https://github.com/vector-im/element-desktop/pull/151)

Changes in [1.7.13](https://github.com/vector-im/element-desktop/releases/tag/v1.7.13) (2020-11-09)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.13-rc.1...v1.7.13)

 * No changes since rc.1

Changes in [1.7.13-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.13-rc.1) (2020-11-04)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.12...v1.7.13-rc.1)

 * Add countly experiment to develop/nightly configs
   [\#150](https://github.com/vector-im/element-desktop/pull/150)

Changes in [1.7.12](https://github.com/vector-im/element-desktop/releases/tag/v1.7.12) (2020-10-28)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.11...v1.7.12)

 * No changes since 1.7.11

Changes in [1.7.11](https://github.com/vector-im/element-desktop/releases/tag/v1.7.11) (2020-10-26)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.11-rc.1...v1.7.11)

 * No changes since rc.1

Changes in [1.7.11-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.11-rc.1) (2020-10-21)
=============================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.10...v1.7.11-rc.1)

 * Bump npm-user-validate from 1.0.0 to 1.0.1
   [\#148](https://github.com/vector-im/element-desktop/pull/148)
 * Use keytar for the seshat passphrase.
   [\#147](https://github.com/vector-im/element-desktop/pull/147)
 * Upgrade to Electron 10.1.3
   [\#146](https://github.com/vector-im/element-desktop/pull/146)

Changes in [1.7.10](https://github.com/vector-im/element-desktop/releases/tag/v1.7.10) (2020-10-20)
===================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.9...v1.7.10)

 * No changes since 1.7.9

Changes in [1.7.9](https://github.com/vector-im/element-desktop/releases/tag/v1.7.9) (2020-10-12)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.9-rc.1...v1.7.9)

 * No changes since rc.1

Changes in [1.7.9-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.9-rc.1) (2020-10-07)
===========================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.8...v1.7.9-rc.1)

 * package.json: Bump the seshat version.
   [\#145](https://github.com/vector-im/element-desktop/pull/145)
 * Explicitly depend on `request` as webcontents-handler requires it
   [\#144](https://github.com/vector-im/element-desktop/pull/144)
 * Upgrade png-to-ico
   [\#143](https://github.com/vector-im/element-desktop/pull/143)
 * Point 'new issue' link at issue-type choice page
   [\#142](https://github.com/vector-im/element-desktop/pull/142)

Changes in [1.7.8](https://github.com/vector-im/element-desktop/releases/tag/v1.7.8) (2020-09-28)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.8-rc.1...v1.7.8)

 * No changes since rc.1

Changes in [1.7.8-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.8-rc.1) (2020-09-23)
===========================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.7...v1.7.8-rc.1)

 * Fix neon error by upgrading Seshat
   [\#141](https://github.com/vector-im/element-desktop/pull/141)
 * Upgrade to Electron 10.1.1
   [\#140](https://github.com/vector-im/element-desktop/pull/140)

Changes in [1.7.7](https://github.com/vector-im/element-desktop/releases/tag/v1.7.7) (2020-09-14)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.6...v1.7.7)

 * No changes since 1.7.6

Changes in [1.7.6](https://github.com/vector-im/element-desktop/releases/tag/v1.7.6) (2020-09-14)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.6-rc.1...v1.7.6)

 * No changes since rc.1

Changes in [1.7.6-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.6-rc.1) (2020-09-09)
===========================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.5...v1.7.6-rc.1)

 * Update to Element pipeline name
   [\#139](https://github.com/vector-im/element-desktop/pull/139)
 * Bump bl from 4.0.2 to 4.0.3
   [\#137](https://github.com/vector-im/element-desktop/pull/137)

Changes in [1.7.5](https://github.com/vector-im/element-desktop/releases/tag/v1.7.5) (2020-09-01)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.5-rc.1...v1.7.5)

 * No changes since 1.7.5-rc.1

Changes in [1.7.5-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.5-rc.1) (2020-08-26)
===========================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.4...v1.7.5-rc.1)

 * Settings v3: Update configs for new feature flag behaviour
   [\#135](https://github.com/vector-im/element-desktop/pull/135)
 * Add reaction preview labs flags to nightly
   [\#134](https://github.com/vector-im/element-desktop/pull/134)

Changes in [1.7.4](https://github.com/vector-im/element-desktop/releases/tag/v1.7.4) (2020-08-17)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.4-rc.1...v1.7.4)

 * No changes since 1.7.4-rc.1

Changes in [1.7.4-rc.1](https://github.com/vector-im/element-desktop/releases/tag/v1.7.4-rc.1) (2020-08-13)
===========================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.3...v1.7.4-rc.1)

 * Update policy links to element.io
   [\#132](https://github.com/vector-im/element-desktop/pull/132)
 * Update bug report submission URL
   [\#131](https://github.com/vector-im/element-desktop/pull/131)
 * Update code signing cert for Windows
   [\#130](https://github.com/vector-im/element-desktop/pull/130)
 * Replace Riot with Element in docs and comments
   [\#129](https://github.com/vector-im/element-desktop/pull/129)
 * Fix order of README steps
   [\#128](https://github.com/vector-im/element-desktop/pull/128)
 * Upgrade to Electron 9.1.2
   [\#127](https://github.com/vector-im/element-desktop/pull/127)

Changes in [1.7.3](https://github.com/vector-im/element-desktop/releases/tag/v1.7.3) (2020-08-05)
=================================================================================================
[Full Changelog](https://github.com/vector-im/element-desktop/compare/v1.7.3-rc.1...v1.7.3)

 * No changes since 1.7.3-rc.1

Changes in [1.7.3-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.7.3-rc.1) (2020-07-31)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.7.2...v1.7.3-rc.1)

 * Clean up linting
   [\#126](https://github.com/vector-im/riot-desktop/pull/126)
 * Update renaming workaround for 'Element' name
   [\#125](https://github.com/vector-im/riot-desktop/pull/125)

Changes in [1.7.2](https://github.com/vector-im/riot-desktop/releases/tag/v1.7.2) (2020-07-27)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.7.1...v1.7.2)

 * Catch exceptions from main method in fetch script
   [\#124](https://github.com/vector-im/riot-desktop/pull/124)
 * Use new eslint package
   [\#122](https://github.com/vector-im/riot-desktop/pull/122)
 * Remove ' (Riot)' from app name
   [\#123](https://github.com/vector-im/riot-desktop/pull/123)

Changes in [1.7.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.7.1) (2020-07-16)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.7.0...v1.7.1)

 * Bump lodash from 4.17.15 to 4.17.19
   [\#121](https://github.com/vector-im/riot-desktop/pull/121)
 * Don't forget nightly when computing userData path
   [\#120](https://github.com/vector-im/riot-desktop/pull/120)
 * Fix hosting link
   [\#119](https://github.com/vector-im/riot-desktop/pull/119)
 * New macOS icon
   [\#117](https://github.com/vector-im/riot-desktop/pull/117)
 * Update README.md
   [\#118](https://github.com/vector-im/riot-desktop/pull/118)
 * More icon updates
   [\#115](https://github.com/vector-im/riot-desktop/pull/115)
 * Don't forget to yarn install
   [\#114](https://github.com/vector-im/riot-desktop/pull/114)

Changes in [1.7.0](https://github.com/vector-im/riot-desktop/releases/tag/v1.7.0) (2020-07-15)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.8...v1.7.0)

 * Fix lint error
   [\#113](https://github.com/vector-im/riot-desktop/pull/113)
 * Delabs font-scaling
   [\#112](https://github.com/vector-im/riot-desktop/pull/112)
 * Remove room list labs flag from config
   [\#109](https://github.com/vector-im/riot-desktop/pull/109)
 * Remove the irc layout setting from labs
   [\#111](https://github.com/vector-im/riot-desktop/pull/111)
 * Update npm to ^6.14.6
   [\#108](https://github.com/vector-im/riot-desktop/pull/108)

Changes in [1.6.8](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.8) (2020-07-03)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.8-rc.1...v1.6.8)

 * No changes since rc.1

Changes in [1.6.8-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.8-rc.1) (2020-07-01)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.7...v1.6.8-rc.1)

 * Show expiring toast on completed downloads to prompt user to open
   [\#106](https://github.com/vector-im/riot-desktop/pull/106)
 * Upgrade to Electron 9.0.5
   [\#107](https://github.com/vector-im/riot-desktop/pull/107)
 * Add new spinner labs option to config.json
   [\#105](https://github.com/vector-im/riot-desktop/pull/105)
 * electron-main: Skip the reindex if we're going to delete the db anyways.
   [\#104](https://github.com/vector-im/riot-desktop/pull/104)
 * riot-desktop: Bump the required seshat version.
   [\#103](https://github.com/vector-im/riot-desktop/pull/103)
 * main: Add an event index IPC method to check if a room is being indexed.
   [\#100](https://github.com/vector-im/riot-desktop/pull/100)
 * electron-main: Add support to set and get the user version.
   [\#102](https://github.com/vector-im/riot-desktop/pull/102)
 * Upgrade to Electron 9
   [\#94](https://github.com/vector-im/riot-desktop/pull/94)

Changes in [1.6.7](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.7) (2020-06-29)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.6...v1.6.7)

 * No changes since 1.6.6

Changes in [1.6.6](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.6) (2020-06-23)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.6-rc.1...v1.6.6)

 * No changes since rc.1

Changes in [1.6.6-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.6-rc.1) (2020-06-17)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.5...v1.6.6-rc.1)

 * Upgrade needle to avoid bugs with modern Node
   [\#101](https://github.com/vector-im/riot-desktop/pull/101)
 * Fix riot-desktop manual update check getting stuck on Downloading...
   [\#99](https://github.com/vector-im/riot-desktop/pull/99)
 * Electron recall latest downloaded update for when the user manually asks
   [\#98](https://github.com/vector-im/riot-desktop/pull/98)
 * use keytar to store pickle keys
   [\#95](https://github.com/vector-im/riot-desktop/pull/95)

Changes in [1.6.5](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.5) (2020-06-16)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.4...v1.6.5)

 * No changes since 1.6.4

Changes in [1.6.4](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.4) (2020-06-05)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.3...v1.6.4)

 * No changes since 1.6.3

Changes in [1.6.3](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.3) (2020-06-04)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.3-rc.1...v1.6.3)

 * No changes since rc.1

Changes in [1.6.3-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.3-rc.1) (2020-06-02)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.2...v1.6.3-rc.1)

 * Fix electron context menu copy/save-as
   [\#96](https://github.com/vector-im/riot-desktop/pull/96)
 * Fixed error in README.md/User-specified config.json
   [\#97](https://github.com/vector-im/riot-desktop/pull/97)
 * Update Modular hosting link
   [\#92](https://github.com/vector-im/riot-desktop/pull/92)
 * Enforce sandbox on all spawned BrowserWindow objects
   [\#91](https://github.com/vector-im/riot-desktop/pull/91)
 * Run before-quit on updates too to flush rageshake
   [\#93](https://github.com/vector-im/riot-desktop/pull/93)
 * Enable new room list labs flag
   [\#87](https://github.com/vector-im/riot-desktop/pull/87)
 * Add asar-webapp script
   [\#59](https://github.com/vector-im/riot-desktop/pull/59)
 * Bump acorn from 6.4.0 to 6.4.1
   [\#50](https://github.com/vector-im/riot-desktop/pull/50)
 * Enable font scaling flag for nightly
   [\#89](https://github.com/vector-im/riot-desktop/pull/89)
 * Enable IRC UI labs flag in nightly
   [\#88](https://github.com/vector-im/riot-desktop/pull/88)
 * Update help message to fix broken url to electron docs
   [\#86](https://github.com/vector-im/riot-desktop/pull/86)

Changes in [1.6.2](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.2) (2020-05-22)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.1...v1.6.2)

 * No changes since 1.6.2

Changes in [1.6.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.1) (2020-05-19)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.1-rc.1...v1.6.1)

 * No changes since rc.1

Changes in [1.6.1-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.1-rc.1) (2020-05-14)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0...v1.6.1-rc.1)

 * Add CI scripts to install and link JS SDK
   [\#85](https://github.com/vector-im/riot-desktop/pull/85)
 * Use Xenial as the build image's base distribution
   [\#84](https://github.com/vector-im/riot-desktop/pull/84)
 * Persist GPG keys for Linux builds via Docker
   [\#83](https://github.com/vector-im/riot-desktop/pull/83)
 * Update README to mention profile support
   [\#81](https://github.com/vector-im/riot-desktop/pull/81)
 * Remove Conflicts from riot-desktop
   [\#82](https://github.com/vector-im/riot-desktop/pull/82)
 * Add a default Linux distribution
   [\#79](https://github.com/vector-im/riot-desktop/pull/79)
 * Remove invite only padlocks feature flag config
   [\#77](https://github.com/vector-im/riot-desktop/pull/77)
 * package.json: Bump the Seshat dep.
   [\#75](https://github.com/vector-im/riot-desktop/pull/75)
 * Remove encrypted message search feature flag
   [\#74](https://github.com/vector-im/riot-desktop/pull/74)
 * Update readme now it's the real source
   [\#73](https://github.com/vector-im/riot-desktop/pull/73)

Changes in [1.6.0](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0) (2020-05-05)
==============================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.6...v1.6.0)

 * No changes since rc.6

Changes in [1.6.0-rc.6](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.6) (2020-05-01)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.5...v1.6.0-rc.6)

 * No changes since rc.5

Changes in [1.6.0-rc.5](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.5) (2020-04-30)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.4...v1.6.0-rc.5)

 * Remove feature flag docs from docs on release
   [\#78](https://github.com/vector-im/riot-desktop/pull/78)
 * package.json: Bump the Seshat dep.
   [\#76](https://github.com/vector-im/riot-desktop/pull/76)

Changes in [1.6.0-rc.4](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.4) (2020-04-23)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.3...v1.6.0-rc.4)

 * No changes since rc.3

Changes in [1.6.0-rc.3](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.3) (2020-04-17)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.2...v1.6.0-rc.3)

 * widen search paths / fix vector-im/riot-web#13190 [to release]
   [\#72](https://github.com/vector-im/riot-desktop/pull/72)

Changes in [1.6.0-rc.2](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.2) (2020-04-16)
========================================================================================================
[Full Changelog](https://github.com/vector-im/riot-desktop/compare/v1.6.0-rc.1...v1.6.0-rc.2)

 * No changes since rc.1

Changes in [1.6.0-rc.1](https://github.com/vector-im/riot-desktop/releases/tag/v1.6.0-rc.1) (2020-04-15)
========================================================================================================

 * Enable cross-signing / E2EE by default for DM on release
   [\#70](https://github.com/vector-im/riot-desktop/pull/70)
 * Add a release script
   [\#69](https://github.com/vector-im/riot-desktop/pull/69)
 * Fix Electron SSO handling to support multiple profiles
   [\#67](https://github.com/vector-im/riot-desktop/pull/67)
 * Add riot-desktop shortcuts for forward/back matching browsers&slack
   [\#68](https://github.com/vector-im/riot-desktop/pull/68)
 * package.json: Bump the Seshat version.
   [\#66](https://github.com/vector-im/riot-desktop/pull/66)
 * Bump minimist from 1.2.2 to 1.2.3
   [\#64](https://github.com/vector-im/riot-desktop/pull/64)
 * Add cfg to access the hak.json
   [\#65](https://github.com/vector-im/riot-desktop/pull/65)
 * Extract dep versions out to hak.json
   [\#63](https://github.com/vector-im/riot-desktop/pull/63)
 * Make the openssl version a variable
   [\#62](https://github.com/vector-im/riot-desktop/pull/62)
 * Update openssl
   [\#61](https://github.com/vector-im/riot-desktop/pull/61)
 * Fix spellcheck language fallback algorithm
   [\#60](https://github.com/vector-im/riot-desktop/pull/60)
 * package.json: Bump the required Seshat version.
   [\#57](https://github.com/vector-im/riot-desktop/pull/57)
 * Remove welcome user from config
   [\#56](https://github.com/vector-im/riot-desktop/pull/56)
 * electron-main: Immediately set the eventIndex variable to null when
   closing.
   [\#55](https://github.com/vector-im/riot-desktop/pull/55)
 * Enable Seshat on Nightly
   [\#54](https://github.com/vector-im/riot-desktop/pull/54)
 * Register Mac electron specific Cmd+, shortcut to User Settings
   [\#53](https://github.com/vector-im/riot-desktop/pull/53)
 * Bump minimist from 1.2.0 to 1.2.2
   [\#52](https://github.com/vector-im/riot-desktop/pull/52)
 * package.json: Bump the required Seshat version.
   [\#51](https://github.com/vector-im/riot-desktop/pull/51)
 * Updates for Seshat 1.2.0 (not yet released) and support to delete events
   from the index.
   [\#47](https://github.com/vector-im/riot-desktop/pull/47)
 * Add custom themes labs flag
   [\#49](https://github.com/vector-im/riot-desktop/pull/49)
 * Get the app ID from the cintext
   [\#46](https://github.com/vector-im/riot-desktop/pull/46)
 * Electron 8 changes. Deprecations. Updates.
   [\#38](https://github.com/vector-im/riot-desktop/pull/38)
 * Bump seshat dependency
   [\#45](https://github.com/vector-im/riot-desktop/pull/45)
 * Move deb control logic to builder
   [\#44](https://github.com/vector-im/riot-desktop/pull/44)
 * Add 'nightly' to brand too
   [\#43](https://github.com/vector-im/riot-desktop/pull/43)
 * Enable seshat in labs on nightly
   [\#42](https://github.com/vector-im/riot-desktop/pull/42)
 * Add config for Riot Nightly
   [\#41](https://github.com/vector-im/riot-desktop/pull/41)
 * Add a windows signing script
   [\#40](https://github.com/vector-im/riot-desktop/pull/40)
 * riot-desktop open SSO in browser so user doesn't have to auth twice
   [\#37](https://github.com/vector-im/riot-desktop/pull/37)
 * Remove the certificate config for windows
   [\#39](https://github.com/vector-im/riot-desktop/pull/39)
 * Missed an await
   [\#36](https://github.com/vector-im/riot-desktop/pull/36)
 * Exit with exit code on exception
   [\#35](https://github.com/vector-im/riot-desktop/pull/35)
 * Fix the set-version script
   [\#34](https://github.com/vector-im/riot-desktop/pull/34)
 * Pass through the env var we actually use to docker
   [\#33](https://github.com/vector-im/riot-desktop/pull/33)
 * Upgrade to electron 8.0.1 and implement spellchecking
   [\#30](https://github.com/vector-im/riot-desktop/pull/30)
 * Fix check script
   [\#31](https://github.com/vector-im/riot-desktop/pull/31)
 * Support fetching the latest develop build
   [\#29](https://github.com/vector-im/riot-desktop/pull/29)
 * Hopefully enable subpixel font rendering
   [\#28](https://github.com/vector-im/riot-desktop/pull/28)
 * Add our native modules separately into the files
   [\#27](https://github.com/vector-im/riot-desktop/pull/27)
 * Fix setversion script's yarn call on windows
   [\#26](https://github.com/vector-im/riot-desktop/pull/26)
 * Split 32/64 bit building
   [\#25](https://github.com/vector-im/riot-desktop/pull/25)
 * Build on 32 bit Windows
   [\#23](https://github.com/vector-im/riot-desktop/pull/23)
 * Build seshat on Linux
   [\#22](https://github.com/vector-im/riot-desktop/pull/22)
 * Native module builds: matrix-seshat for mac & win
   [\#21](https://github.com/vector-im/riot-desktop/pull/21)
 * Port desktop fixes
   [\#20](https://github.com/vector-im/riot-desktop/pull/20)
 * Add accelerators to context menu options like cut&paste in electron
   [\#19](https://github.com/vector-im/riot-desktop/pull/19)
 * Build the deb into a repo
   [\#18](https://github.com/vector-im/riot-desktop/pull/18)
 * Better Docker Support
   [\#17](https://github.com/vector-im/riot-desktop/pull/17)
 * Use a custom control file for the Debian package
   [\#14](https://github.com/vector-im/riot-desktop/pull/14)
 * Support config directories
   [\#15](https://github.com/vector-im/riot-desktop/pull/15)
 * Don't bail if we can't notarise
   [\#16](https://github.com/vector-im/riot-desktop/pull/16)
 * Set version automatically
   [\#13](https://github.com/vector-im/riot-desktop/pull/13)
 * Sign natively on Windows
   [\#12](https://github.com/vector-im/riot-desktop/pull/12)
 * Fix the linting errors
   [\#11](https://github.com/vector-im/riot-desktop/pull/11)
 * Electron API Updates
   [\#10](https://github.com/vector-im/riot-desktop/pull/10)
 * Package webapp into an asar archive
   [\#9](https://github.com/vector-im/riot-desktop/pull/9)
 * Sanitise scripts
   [\#8](https://github.com/vector-im/riot-desktop/pull/8)
 * Exit after importing key
   [\#6](https://github.com/vector-im/riot-desktop/pull/6)
 * Use portable mkdirp
   [\#5](https://github.com/vector-im/riot-desktop/pull/5)
 * Add explicit 'node' to scripts
   [\#4](https://github.com/vector-im/riot-desktop/pull/4)
 * Check properly
   [\#3](https://github.com/vector-im/riot-desktop/pull/3)
 * Add rimraf
   [\#2](https://github.com/vector-im/riot-desktop/pull/2)
 * Build electron app from pre-built tarball
   [\#1](https://github.com/vector-im/riot-desktop/pull/1)


