:root {
  --TB-top: calc(var(--server-container) + var(--window-padding));
  --TB-tr-roundness: var(--window-roundness);
  --TB-position-top: var(--TB-top, var(--window-padding));
  --TB-position-right: var(--window-padding);
  --tint: rgba(var(--tint-colour), var(--tint-brightness));
  --white-half: rgba(255,255,255,0.025);
  --white: rgba(255,255,255,0.05);
  --white-double: rgba(255,255,255,0.1);
  --white-triple: rgba(255,255,255,0.15);
  --gradient: linear-gradient(var(--gradient-direction), rgb(var(--gradient-primary)), rgb(var(--gradient-secondary)));
  --gradient-20: linear-gradient(var(--gradient-direction), rgba(var(--gradient-primary), 0.2), rgba(var(--gradient-secondary), 0.2));
  --gradient-50: linear-gradient(var(--gradient-direction), rgba(var(--gradient-primary), 0.5), rgba(var(--gradient-secondary), 0.5));
  --gradient-90: linear-gradient(var(--gradient-direction), rgba(var(--gradient-primary), 0.9), rgba(var(--gradient-secondary), 0.9));
  --text-shadow: 1;
  --chat-embed: var(--background-secondary);
  --discord-green: 67,181,129;
  --discord-yellow: 219,171,9;
  --discord-red: 215,58,73;
  --discord-purple: 89,54,149;
  --discord-invisible: 117,128,142;
  --discord-nitro: 255,115,250;
  --discord-blurple: 114,137,218;
  --discord-spotify: 29,185,84;
  --discord-twitch: 89,54,149;
  --discord-xbox: 16,124,16;
  --version: "Frosted Glass 2.0.10";
}

.theme-dark {
  --header-primary: #fff;
  --header-secondary: #bbb;
  --text-normal: #fff;
  --text-default: #ddd;
  --text-muted: #aaa;
  --text-link: #00b0f4;
  --channels-default: #ddd;
  --interactive-normal: #bbb;
  --interactive-hover: #eee;
  --interactive-active: #fff;
  --interactive-muted: #777;
  --background-primary: transparent;
  --background-secondary: rgba(0,0,0,0.3);
  --background-secondary-alt: transparent;
  --background-tertiary: transparent;
  --background-accent: #4f545c;
  --background-floating: transparent;
  --background-mobile-primary: #36393f;
  --background-mobile-secondary: #2f3136;
  --background-modifier-hover: rgba(255,255,255,0.05);
  --background-modifier-active: rgba(255,255,255,0.07);
  --background-modifier-selected: rgba(255,255,255,0.1);
  --background-modifier-accent: rgba(255,255,255,0.1);
  --background-mentioned: rgba(250,166,26,0.05);
  --background-mentioned-hover: rgba(250,166,26,0.08);
  --background-message-hover: rgba(4,4,5,0.07);
  --elevation-stroke: 0 0 0 1px rgba(4,4,5,0.15);
  --elevation-low: 0 1px 0 rgba(4,4,5,0.2),0 1.5px 0 rgba(6,6,7,0.05),0 2px 0 rgba(4,4,5,0.05);
  --elevation-medium: 0 4px 4px rgba(0,0,0,0.16);
  --elevation-high: 0 8px 16px rgba(0,0,0,0.24);
  --logo-primary: #fff;
  --guild-header-text-shadow: 0 1px 1px rgba(0,0,0,0.4);
  --channeltextarea-background: rgba(255,255,255,0.05);
  --activity-card-background: #202225;
  --textbox-markdown-syntax: #8e9297;
  --deprecated-card-bg: rgba(0,0,0,0.3);
  --deprecated-card-editable-bg: rgba(0,0,0,0.3);
  --deprecated-store-bg: #36393f;
  --deprecated-quickswitcher-input-background: var(--channeltextarea-background);
  --deprecated-quickswitcher-input-placeholder: rgba(255,255,255,0.5);
  --deprecated-text-input-bg: rgba(0,0,0,0.1);
  --deprecated-text-input-border: rgba(0,0,0,0.3);
  --deprecated-text-input-border-hover: #040405;
  --deprecated-text-input-border-disabled: #202225;
  --deprecated-text-input-prefix: #dcddde;
  --text-link: var(--link-colour);
}

#app-mount:before {
  content: "";
  background: var(--background-image);
  background-position: var(--background-image-position, center);
  background-size: var(--background-image-size, cover);
  position: absolute;
  height: calc(100vh + var(--background-image-blur) * 2);
  width: calc(100vw + var(--background-image-blur) * 2);
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

#app-mount .layers-OrUESM {
  margin: var(--window-padding);
  overflow: hidden;
  border-radius: var(--window-roundness);
}
#app-mount .layer-86YKbF {
  background: var(--tint);
}
#app-mount .base-2jDfDU:before {
  content: "";
  position: absolute;
  height: 5px;
  width: 100%;
  background: linear-gradient(rgba(0, 0, 0, 0.2), transparent);
  z-index: 1;
  top: 48px;
  pointer-events: none;
  -webkit-user-select: none;
     -moz-user-select: none;
      -ms-user-select: none;
          user-select: none;
}
#app-mount .botTagRegular-2HEhHi {
  background: var(--gradient);
  color: var(--text-normal);
  margin-top: 0;
}
#app-mount .botText-1fD6Qk {
  font-weight: 600;
}
#app-mount .botTagInvert-18-95s {
  color: rgb(var(--gradient-primary));
}
#app-mount .botTagInvert-18-95s .botText-1fD6Qk {
  font-weight: bold;
}

::-moz-selection {
  background: rgb(var(--gradient-primary));
  color: var(--text-normal);
}

::selection {
  background: rgb(var(--gradient-primary));
  color: var(--text-normal);
}

#app-mount .app-2CXKsg::before {
  content: "Your version of Frosted Glass is outdated. Please redownload";
  white-space: pre-wrap;
  display: var(--update-notice-1, block);
  color: #fff;
  text-align: center;
  padding: 10px 0;
  box-sizing: border-box;
  background: rgb(var(--discord-blurple), 0.7);
  text-shadow: 0 2px 3px rgba(0, 0, 0, var(--text-shadow));
}

::-webkit-scrollbar {
  width: 8px !important;
  height: 8px !important;
}

::-webkit-scrollbar,
::-webkit-scrollbar-track,
::-webkit-scrollbar-track-piece {
  border-color: transparent !important;
  background: transparent !important;
}

::-webkit-scrollbar-thumb {
  border-radius: 10px !important;
  border: none !important;
  background-clip: content-box !important;
  background: var(--scrollbar-colour) !important;
}

::-webkit-scrollbar-corner {
  visibility: hidden !important;
}

.scrollerThemed-2oenus.themeHidden-2yP93k .scroller-2FKFPG::-webkit-scrollbar,
.scrollerThemed-2oenus.themeHidden-2yP93k .scroller-2FKFPG::-webkit-scrollbar-corner,
.scrollerThemed-2oenus.themeHidden-2yP93k .scroller-2FKFPG::-webkit-scrollbar-thumb,
.scrollerThemed-2oenus.themeHidden-2yP93k .scroller-2FKFPG::-webkit-scrollbar-track {
  display: none !important;
}

::-webkit-input-placeholder, body, button, input, select, textarea {
  font-family: var(--font, "Whitney");
}

#app-mount .tooltip-14MtrL {
  color: var(--text-normal);
  text-align: center;
  font-weight: 600;
}
#app-mount .tooltipPrimary-3qLMbS {
  background: var(--gradient);
}
#app-mount .tooltipPrimary-3qLMbS .tooltipPointer-3L49xb {
  display: none;
}

#app-mount .layers-OrUESM:before {
  content: "";
  background: var(--background-image);
  background-position: var(--background-image-position, center);
  background-size: var(--background-image-size, cover);
  background-repeat: var(--background-image-repeat, no-repeat);
  height: calc(100vh + var(--background-image-blur) * 2);
  width: calc(100vw + var(--background-image-blur) * 2);
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  position: absolute;
  filter: blur(var(--background-image-blur));
  pointer-events: none;
  -webkit-user-select: none;
     -moz-user-select: none;
      -ms-user-select: none;
          user-select: none;
}
#app-mount [role=menu],
#app-mount .autocompleteInner-y1mjDl,
#app-mount .container-2McqkF,
#app-mount .container-enaOkj,
#app-mount .container-8Futzw,
#app-mount .contextMenu-HLZMGh:not(.scroller-2FKFPG),
#app-mount .emojiPicker-6YCk8a,
#app-mount .messagesPopoutWrap-1MQ1bW,
#app-mount .modal-2RrUKJ:not(.slide-2pHaq5),
#app-mount .root-1gCeng:not(.fullscreenOnMobile-1bD22y),
#app-mount .root-8LYsGj,
#app-mount .subMenuContext-2n_9YM .scrollerWrap-2lJEkd,
#app-mount [class*=userPopout][aria-modal=true],
#app-mount section.positionContainer-3unAXC .drawerSizingWrapper-27qFHb,
#app-mount .quickswitcher-pKcM9U,
#app-mount .root-1gCeng.wrapper-2ZbzR9,
#app-mount .modalRoot-1Kx4Hb,
#app-mount .container-3JTnYm.thin-1ybCId.scrollerBase-_bVAAt,
#app-mount .popoutContainer-2wbmiM,
#app-mount .root-1gCeng:not(.modal-3Crloo),
#app-mount .container-2O1UgZ,
#app-mount .container-18GwIk,
#app-mount .popout-TdhJ6Z {
  overflow: hidden !important;
  position: relative;
  border-radius: 3px;
}
#app-mount [role=menu]:before,
#app-mount .autocompleteInner-y1mjDl:before,
#app-mount .container-2McqkF:before,
#app-mount .container-enaOkj:before,
#app-mount .container-8Futzw:before,
#app-mount .contextMenu-HLZMGh:not(.scroller-2FKFPG):before,
#app-mount .emojiPicker-6YCk8a:before,
#app-mount .messagesPopoutWrap-1MQ1bW:before,
#app-mount .modal-2RrUKJ:not(.slide-2pHaq5):before,
#app-mount .root-1gCeng:not(.fullscreenOnMobile-1bD22y):before,
#app-mount .root-8LYsGj:before,
#app-mount .subMenuContext-2n_9YM .scrollerWrap-2lJEkd:before,
#app-mount [class*=userPopout][aria-modal=true]:before,
#app-mount section.positionContainer-3unAXC .drawerSizingWrapper-27qFHb:before,
#app-mount .quickswitcher-pKcM9U:before,
#app-mount .root-1gCeng.wrapper-2ZbzR9:before,
#app-mount .modalRoot-1Kx4Hb:before,
#app-mount .container-3JTnYm.thin-1ybCId.scrollerBase-_bVAAt:before,
#app-mount .popoutContainer-2wbmiM:before,
#app-mount .root-1gCeng:not(.modal-3Crloo):before,
#app-mount .container-2O1UgZ:before,
#app-mount .container-18GwIk:before,
#app-mount .popout-TdhJ6Z:before {
  content: "";
  background: linear-gradient(var(--tint), var(--tint)), var(--popout-modal-image);
  background-position: var(--popout-modal-position, center);
  background-size: var(--popout-modal-size, cover);
  background-attachment: var(--popout-modal-attachment, fixed);
  background-repeat: var(--popout-modal-repeat, no-repeat);
  box-shadow: inset 0 0 0 100vmax rgba(0, 0, 0, var(--popout-modal-brightness));
  height: calc(100% + var(--popout-modal-blur) * 5);
  width: calc(100% + var(--popout-modal-blur) * 5);
  top: calc(var(--popout-modal-blur) / -1 * 2.5);
  left: calc(var(--popout-modal-blur) / -1 * 2.5);
  position: absolute;
  filter: blur(var(--popout-modal-blur));
  pointer-events: none;
  -webkit-user-select: none;
     -moz-user-select: none;
      -ms-user-select: none;
          user-select: none;
  z-index: -1;
}

#app-mount .lookFilled-1Gx00P.colorPrimary-3b3xI6,
#app-mount .lookGhost-2Fn_0-.colorGrey-2DXtkV,
#app-mount .lookInverted-2D7oAl.colorBrand-3pXr91,
#app-mount .lookOutlined-3sRXeN.colorPrimary-3b3xI6,
#app-mount .lookOutlined-3sRXeN.colorWhite-rEQuAQ {
  background-color: var(--white);
  color: var(--text-normal);
  border-color: transparent;
  transition: 0.2s ease;
}
#app-mount .lookFilled-1Gx00P.colorPrimary-3b3xI6:hover,
#app-mount .lookGhost-2Fn_0-.colorGrey-2DXtkV:hover,
#app-mount .lookInverted-2D7oAl.colorBrand-3pXr91:hover,
#app-mount .lookOutlined-3sRXeN.colorPrimary-3b3xI6:hover,
#app-mount .lookOutlined-3sRXeN.colorWhite-rEQuAQ:hover {
  background: var(--white-double);
}
#app-mount .lookFilled-1Gx00P.colorPrimary-3b3xI6:active,
#app-mount .lookGhost-2Fn_0-.colorGrey-2DXtkV:active,
#app-mount .lookInverted-2D7oAl.colorBrand-3pXr91:active,
#app-mount .lookOutlined-3sRXeN.colorPrimary-3b3xI6:active,
#app-mount .lookOutlined-3sRXeN.colorWhite-rEQuAQ:active {
  background: var(--white-triple);
}
#app-mount .actionRed-gYn8D3,
#app-mount .colorRed-1TFJan {
  background: rgba(var(--discord-red), 0.5);
  border: none;
  color: #fff;
  transition: 0.2s ease;
}
#app-mount .actionRed-gYn8D3:active, #app-mount .actionRed-gYn8D3:hover,
#app-mount .colorRed-1TFJan:active,
#app-mount .colorRed-1TFJan:hover {
  background: rgb(var(--discord-red));
}
#app-mount .lookFilled-1Gx00P.colorGreen-29iAKY {
  background: rgba(var(--discord-green), 0.4);
  transition: 0.2s ease;
}
#app-mount .lookFilled-1Gx00P.colorGreen-29iAKY:active, #app-mount .lookFilled-1Gx00P.colorGreen-29iAKY:hover {
  background: rgb(var(--discord-green));
}
#app-mount .lookInverted-2D7oAl.colorGreen-29iAKY {
  background: var(--white);
}
#app-mount .lookInverted-2D7oAl.colorGreen-29iAKY:hover {
  background: var(--white-double);
}
#app-mount .lookInverted-2D7oAl.colorGreen-29iAKY:active {
  background: var(--white-triple);
}
#app-mount .bd-pfbtn,
#app-mount .lookFilled-1Gx00P.colorBrand-3pXr91 {
  background: var(--gradient);
}
#app-mount .lookLink-9FtZy-.colorBrand-3pXr91 {
  color: rgb(var(--gradient-primary));
  opacity: 1;
}
#app-mount .lookOutlined-3sRXeN.colorBrand-3pXr91 {
  background: rgba(var(--discord-blurple), 0.3);
  border: transparent;
  transition: 0.2s ease;
  color: #fff;
}
#app-mount .lookOutlined-3sRXeN.colorBrand-3pXr91:active, #app-mount .lookOutlined-3sRXeN.colorBrand-3pXr91:hover {
  background: rgb(var(--discord-blurple));
}
#app-mount .bd-search-wrapper,
#app-mount .input-2g-os5:not(.searchBoxInput-3h4etz) {
  background: var(--background-secondary);
  border-color: transparent;
  color: var(--text-normal);
}
#app-mount .bd-search-wrapper::-moz-placeholder, #app-mount .input-2g-os5:not(.searchBoxInput-3h4etz)::-moz-placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .bd-search-wrapper:-ms-input-placeholder, #app-mount .input-2g-os5:not(.searchBoxInput-3h4etz):-ms-input-placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .bd-search-wrapper::placeholder,
#app-mount .input-2g-os5:not(.searchBoxInput-3h4etz)::placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .bd-search::-moz-placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .bd-search:-ms-input-placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .bd-search::placeholder {
  color: rgba(255, 255, 255, 0.5);
}
#app-mount .item-26Dhrx {
  border: none;
  background: var(--background-secondary);
}
#app-mount .item-26Dhrx .checkbox-1ix_J3 {
  border: none;
  background: var(--white-double);
}
#app-mount .item-26Dhrx .checkbox-1ix_J3.checked-1pZh2h {
  background: var(--text-normal) !important;
}
#app-mount .item-26Dhrx[style*="rgb(114, 137, 218)"] {
  background: var(--gradient) !important;
}
#app-mount .item-26Dhrx[style*="rgb(114, 137, 218)"] .checkbox-1ix_J3 {
  background: var(--text-normal);
}
#app-mount .item-26Dhrx[style*="rgb(114, 137, 218)"] polyline {
  stroke: rgb(var(--gradient-primary));
}
#app-mount .item-26Dhrx[style*="rgb(240, 71, 71)"] .checkbox-1ix_J3, #app-mount .item-26Dhrx[style*="rgb(250, 166, 26)"] .checkbox-1ix_J3, #app-mount .item-26Dhrx[style*="rgb(67, 181, 129)"] .checkbox-1ix_J3 {
  background: var(--text-normal);
}
#app-mount .valueUnchecked-2lU_20 {
  background: var(--white-double);
}
#app-mount .themeDefault-24hCdX.valueChecked-m-4IJZ {
  background: var(--gradient);
}
#app-mount .checkboxElement-uwAa9F:checked + span {
  border-color: rgb(var(--gradient-primary));
  background: rgb(var(--gradient-primary));
}
#app-mount .checkbox-3s5GYZ {
  color: rgb(var(--gradient-primary));
}
#app-mount .checkbox-1ix_J3 {
  background: var(--white);
  border: none;
}
#app-mount .checkbox-1ix_J3.checked-1pZh2h {
  background: var(--gradient) !important;
  border: none !important;
}
#app-mount [class*=css][class*=control], #app-mount .select-1Pkeg4 {
  background: var(--background-secondary);
  border-color: transparent;
}
#app-mount [class*=css][class*=placeholder] {
  color: rgba(255, 255, 255, 0.5);
  opacity: 1;
}
#app-mount .bar-1Bhnl9 {
  background: var(--white-double);
}
#app-mount .barFill-2Bh7CX {
  background: var(--gradient);
}
#app-mount .container-1nZlH6 {
  background: var(--background-secondary);
  border-color: transparent;
}

#app-mount .title-3qD0b- .searchBar-zdmu7v {
  background: var(--background-secondary);
}

#app-mount .notice-2HEN-u {
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 0;
  box-shadow: none;
  padding-right: var(--TB-header-padding, 12px);
}
#app-mount .notice-2HEN-u .button-1iHNQ2 {
  top: 0;
  background: var(--white);
  border-color: transparent;
  color: #fff;
}
#app-mount .notice-2HEN-u .button-1iHNQ2:hover {
  background: var(--white-double);
}
#app-mount .notice-2HEN-u .button-1iHNQ2:active {
  background: var(--white-triple);
}
#app-mount .closeButton-30b1gR {
  right: unset;
  left: 0;
  height: 48px;
}
#app-mount .noticeStreamerMode-2TSQpg {
  background: rgba(var(--discord-twitch), 0.6);
}

#app-mount .guilds-2JjMmN {
  background-color: transparent;
}
#app-mount .guilds-2JjMmN .scrollerBase-_bVAAt {
  background-color: rgba(0, 0, 0, var(--serverlist-brightness));
}
#app-mount .guilds-2JjMmN .scrollerBase-_bVAAt::-webkit-scrollbar {
  display: none;
}

#app-mount .guilds-2JjMmN [class*=expandedFolderBackground] {
  background: var(--white);
}
#app-mount .guilds-2JjMmN [class*=folder] {
  background: transparent;
}

#app-mount .guilds-2JjMmN .tutorialContainer-1pL9QS .childWrapper-1j_1ub {
  background: var(--gradient);
  background-color: transparent;
}
#app-mount .guilds-2JjMmN .tutorialContainer-1pL9QS .listItem-3SmSlK:first-child .wrapper-3kah-n:before {
  content: "";
  border-radius: 50%;
  position: absolute;
  background: var(--home-button-image, url("https://gibbu.github.io/BetterDiscord-Themes/FrostedGlass/assets/discord.svg"));
  background-size: var(--home-button-size, cover);
  background-position: var(--home-button-position, center);
  height: 100%;
  width: 100%;
  transition: 0.2s ease;
}
#app-mount .guilds-2JjMmN .tutorialContainer-1pL9QS .listItem-3SmSlK:first-child .wrapper-3kah-n.selected-1Drb7Z:before {
  border-radius: 30%;
}
#app-mount .guilds-2JjMmN .tutorialContainer-1pL9QS .homeIcon-r0w4ny {
  display: none;
}
#app-mount .guilds-2JjMmN .selected-1Drb7Z .acronym-2zrAHN {
  background: var(--white-double);
}
#app-mount .guilds-2JjMmN .acronym-2zrAHN {
  background: var(--white);
}
#app-mount .guilds-2JjMmN .acronym-2zrAHN:hover {
  background: var(--white-double);
}
#app-mount .guilds-2JjMmN [class*=circleIconButton] {
  background: var(--white);
  color: rgb(var(--gradient-primary));
}
#app-mount .guilds-2JjMmN [class*=circleIconButton].selected-ugP_am, #app-mount .guilds-2JjMmN [class*=circleIconButton]:hover {
  background: var(--white-double);
  color: var(--text-normal);
}

#app-mount .sidebar-1tnWFu {
  border-radius: 0;
  background: rgba(0, 0, 0, var(--left-brightness));
}
#app-mount .sidebar-1tnWFu .container-1NXEtd,
#app-mount .sidebar-1tnWFu .privateChannels-oVe7HL,
#app-mount .sidebar-1tnWFu .scroller-WSmht3 {
  background-color: transparent;
}
#app-mount .sidebar-1tnWFu [role=list] > div[style="width: 100%; height: 84px; visibility: hidden;"] {
  height: 120px !important;
}

#app-mount .header-2o-2hj {
  background: transparent;
  box-shadow: none;
}
#app-mount .animatedContainer-1pJv5C {
  -webkit-mask: linear-gradient(rgba(0, 0, 0, 0.9) 60%, rgba(0, 0, 0, 0) 100%) !important;
  top: 48px;
  background: transparent;
}

#app-mount .containerDefault-YUSmu3 .modeUnread-3Cxepe .content-1gYQeQ {
  background: var(--white);
}
#app-mount .containerDefault-YUSmu3 .wrapper-1ucjTd:hover .content-1gYQeQ {
  background: var(--background-modifier-hover);
}
#app-mount .containerDefault-YUSmu3 .wrapper-1ucjTd:hover .content-1gYQeQ .icon-2W8DHg {
  color: var(--interactive-hover);
}
#app-mount .containerDefault-YUSmu3.selected-2TbFuo .content-1gYQeQ {
  background: var(--gradient) !important;
}
#app-mount .containerDefault-YUSmu3.selected-2TbFuo .content-1gYQeQ .icon-2W8DHg {
  color: var(--text-normal);
}
#app-mount .users-i_3-kL {
  background: var(--white);
  padding: 0 5px;
  width: auto;
}
#app-mount .total-3tKGEB {
  background: var(--white-double);
  padding: 0 5px;
  width: auto;
}
#app-mount .containerUserOver-SDa1HW:after {
  background: var(--gradient-20);
  border: 2px solid rgb(var(--gradient-primary));
}

#app-mount .channel-1Shao0.selected-1-Z6gm .layout-1qmrhw {
  background: var(--gradient);
}

#app-mount .panels-3wFtMD {
  background: transparent;
}
#app-mount .panels-3wFtMD .lookFilled-1Gx00P.colorBrand-3pXr91 {
  background: var(--white);
}
#app-mount .panels-3wFtMD .lookFilled-1Gx00P.colorBrand-3pXr91:hover {
  background: var(--white-double);
}
#app-mount .panels-3wFtMD .lookFilled-1Gx00P.colorBrand-3pXr91:active {
  background: var(--white-triple);
}
#app-mount .container-1zzFcN {
  border-bottom: none;
}

#app-mount .unread-1xRYoj {
  background: var(--gradient);
}

#app-mount .content-1jQy2l:before {
  content: none;
}
#app-mount .chat-2ZfjoI {
  background: rgba(0, 0, 0, var(--middle-brightness));
}
#app-mount .messages-3amgkR {
  background-color: transparent;
  text-shadow: 0 2px 5px rgba(0, 0, 0, var(--text-shadow));
}
#app-mount .newMessagesBar-1hF-9G {
  background: var(--gradient);
  opacity: 1;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.5);
}
#app-mount .jumpToPresentBar-1cEnH0 {
  border-radius: 8px;
  background-color: var(--white-double);
  padding-bottom: 0;
  bottom: 10px;
}
#app-mount .jumpToPresentBar-1cEnH0:hover {
  background-color: var(--white-triple);
}

#app-mount .cozy-3raOZG .header-23xsNx {
  margin-left: 0;
  padding-left: 0;
}
#app-mount .message-G6O-Wv {
  background: transparent;
  box-shadow: none;
}
#app-mount .message-2CShn3 {
  background: transparent !important;
}
#app-mount .message-2CShn3 .reaction-1hd86g {
  background: var(--white);
}
#app-mount .message-2CShn3 .reaction-1hd86g.reactionMe-wv5HKu {
  background: var(--gradient);
}
#app-mount .message-2CShn3 .reaction-1hd86g.reactionMe-wv5HKu .reactionCount-2mvXRV {
  color: var(--text-normal);
}
#app-mount .message-2CShn3 .wrapper-2vIMkT {
  background: var(--background-secondary);
}
#app-mount .message-2CShn3 .attachment-33OFj0,
#app-mount .message-2CShn3 .wrapperAudio-1jDe0Q,
#app-mount .message-2CShn3 code {
  background-color: var(--chat-embed);
  border: none;
}
#app-mount .message-2CShn3 .embedFull-2tM8-- {
  background-color: var(--chat-embed);
}
#app-mount .hljs {
  color: var(--text-default);
}
#app-mount .mentioned-Tre-dv {
  background: var(--gradient-20) !important;
}
#app-mount .mentioned-Tre-dv:before {
  background: var(--gradient);
}
#app-mount .wrapper-1ZcZW- {
  background: var(--gradient);
  color: var(--text-normal);
}

#app-mount .form-3gdLxP {
  margin-top: 0;
}
#app-mount .form-3gdLxP .attachButton-_ACFSu {
  padding: 10px;
}
#app-mount .form-3gdLxP .placeholder-1_mJY1,
#app-mount .form-3gdLxP .slateTextArea-27tjG0 {
  padding-left: 5px;
}

#app-mount .divider-2rZFJK {
  border: none;
}
#app-mount .divider-2rZFJK .content-3spvdd {
  display: flex;
  width: 100%;
  justify-content: center;
  align-items: center;
  color: var(--text-muted);
}
#app-mount .divider-2rZFJK .content-3spvdd:before, #app-mount .divider-2rZFJK .content-3spvdd:after {
  content: "";
  flex: 1;
  height: 1px;
  display: block;
  background: var(--background-modifier-accent);
}
#app-mount .divider-2rZFJK .content-3spvdd:before {
  margin-right: 10px;
}
#app-mount .divider-2rZFJK .content-3spvdd:after {
  margin-left: 10px;
}
#app-mount .divider-2rZFJK.isUnread-3Lojb- {
  border-top: 1px solid rgb(var(--discord-red));
}

#app-mount .wrapper-1gVUIN.minimum-fXpVNc {
  background: var(--background-secondary);
}
#app-mount .centerButton-3CaNcJ {
  background: var(--white);
}
#app-mount .centerButton-3CaNcJ:hover {
  background: var(--white-double);
}
#app-mount .controlButton-2PMNom.leaveButton-2YnTyt {
  background: rgba(var(--discord-red), 0.5);
}
#app-mount .controlButton-2PMNom.leaveButton-2YnTyt:hover {
  background: rgb(var(--discord-red));
}
#app-mount .quickSelect-384d3G {
  margin-top: 10px;
}

#app-mount .threadSidebar-1o3BTy {
  background: rgb(0, 0, 0, var(--middle-brightness));
}

#app-mount .container-2o3qEW {
  background-color: rgba(0, 0, 0, var(--right-brightness));
}
#app-mount .members-3WRCEx {
  background: transparent;
}
#app-mount .members-3WRCEx > div {
  background: transparent;
}

#app-mount .member-2gU6Ar.selected-1-Z6gm .layout-1qmrhw {
  background: var(--gradient);
}
#app-mount .member-2gU6Ar.selected-1-Z6gm .roleColor-rz2vM0 {
  color: var(--text-normal) !important;
}
#app-mount .member-2gU6Ar.selected-1-Z6gm .botTagRegular-2HEhHi {
  background: var(--text-normal);
  color: rgb(var(--gradient-primary));
  margin-top: 0;
}
#app-mount .member-2gU6Ar.selected-1-Z6gm .botText-1fD6Qk {
  font-weight: 900;
}
#app-mount .member-2gU6Ar.selected-1-Z6gm .premiumIcon-1rDbWQ {
  color: var(--text-normal);
}

.colorDefault-2K3EoJ.focused-3afm-j,
.colorDefault-2K3EoJ:hover:not(.hideInteraction-1iHO1O) {
  background: var(--white);
}

#app-mount [class*=userPopout][aria-modal=true] {
  box-shadow: none;
  overflow: hidden;
  opacity: 0;
  -webkit-animation: fadeIn 0.3s ease forwards;
          animation: fadeIn 0.3s ease forwards;
}
#app-mount [class*=userPopout][aria-modal=true] .headerNormal-T_seeN {
  background: transparent;
}
#app-mount [class*=userPopout][aria-modal=true] .headerPlaying-j0WQBV {
  background: var(--gradient-50);
}
#app-mount [class*=userPopout][aria-modal=true] .headerXbox-3G-4PF {
  background: rgba(var(--discord-xbox), 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .headerSpotify-zpWxgT {
  background: rgba(var(--discord-spotify), 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .headerStreaming-2FjmGz {
  background: rgba(var(--discord-twitch), 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .wrapper-1VLyxH::after {
  border-radius: 3px;
}
#app-mount [class*=userPopout][aria-modal=true] .activityName-3YXl6e,
#app-mount [class*=userPopout][aria-modal=true] .headerTag-2pZJzA,
#app-mount [class*=userPopout][aria-modal=true] .nameNormal-2lqVQK,
#app-mount [class*=userPopout][aria-modal=true] .nameWrap-3Z4G_9,
#app-mount [class*=userPopout][aria-modal=true] .textRow-1sENuL {
  color: var(--text-normal);
}
#app-mount [class*=userPopout][aria-modal=true] .body-3iLsc4 {
  background: transparent;
}
#app-mount [class*=userPopout][aria-modal=true] .role-2irmRk {
  height: auto;
  position: relative;
  overflow: hidden;
  color: var(--text-normal);
}
#app-mount [class*=userPopout][aria-modal=true] .roleCircle-3xAZ1j::after {
  content: "";
  position: absolute;
  height: 24px;
  width: 100%;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  background: inherit;
  opacity: 0.2;
  z-index: -1;
}
#app-mount [class*=userPopout][aria-modal=true] .footer-1fjuF6 {
  background: transparent;
  border: none;
}
#app-mount [class*=userPopout][aria-modal=true] .quickMessage-1yeL4E {
  background: var(--background-secondary);
  border: none;
  color: var(--text-normal);
}
#app-mount [class*=userPopout][aria-modal=true] .quickMessage-1yeL4E::-moz-placeholder {
  color: rgba(255, 255, 255, 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .quickMessage-1yeL4E:-ms-input-placeholder {
  color: rgba(255, 255, 255, 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .quickMessage-1yeL4E::placeholder {
  color: rgba(255, 255, 255, 0.3);
}
#app-mount [class*=userPopout][aria-modal=true] .protip-YaFfgO {
  display: none;
}

#app-mount [role=menu] {
  box-shadow: none;
  -webkit-animation: fadeIn 0.3s ease forwards;
          animation: fadeIn 0.3s ease forwards;
}
#app-mount .focused-3afm-j .check-1JyqgN {
  color: #fff;
}
#app-mount .button-F9qN4n {
  background: var(--white);
}
#app-mount .button-F9qN4n.focused-3ZzkKr {
  background: var(--white-double);
  box-shadow: 0 0 0 2px rgb(var(--gradient-primary));
}

#app-mount .drawerSizingWrapper-27qFHb {
  right: 0;
  position: absolute !important;
}
#app-mount .drawerSizingWrapper-27qFHb .nav-2KnmHb {
  position: absolute;
  padding: 0 0 0 13px;
  top: 16px;
  z-index: 999;
}
#app-mount .drawerSizingWrapper-27qFHb [class*=searchBar] {
  background: var(--background-secondary);
  margin-left: 105px;
}
#app-mount .drawerSizingWrapper-27qFHb .contentWrapper-2txmjs {
  display: grid;
  grid-template-rows: auto;
  background: transparent;
}
#app-mount .drawerSizingWrapper-27qFHb [aria-selected=true] .navButton-3Mnpqt {
  background: var(--gradient);
}
#app-mount .drawerSizingWrapper-27qFHb .navButton-3Mnpqt {
  background: var(--white);
  padding: 6px 5px 7px;
}
#app-mount .drawerSizingWrapper-27qFHb .categoryFadeBlurple-1HuV1x {
  background: var(--gradient-90);
}
#app-mount .drawerSizingWrapper-27qFHb .focused-q9B2e4:after,
#app-mount .drawerSizingWrapper-27qFHb .result-3OpoO7:hover:after {
  box-shadow: inset 0 0 0 2px rgb(var(--gradient-primary));
}
#app-mount .drawerSizingWrapper-27qFHb .result-3OpoO7 {
  background-color: var(--white) !important;
}
#app-mount .drawerSizingWrapper-27qFHb .emojiItemSelected-2Lg50V {
  background: var(--white-double);
}
#app-mount .drawerSizingWrapper-27qFHb .categoryWrapper-UZ5YNj {
  background: var(--background-secondary);
}
#app-mount .drawerSizingWrapper-27qFHb .category-3Xkx2x {
  color: var(--text-normal);
}

.emojiPicker-6YCk8a {
  box-shadow: none;
  background: transparent;
  -webkit-animation: fadeIn 0.3s ease forwards;
          animation: fadeIn 0.3s ease forwards;
}
.emojiPicker-6YCk8a [class*=header] {
  box-shadow: none;
}
.emojiPicker-6YCk8a .searchBar-2M9mRP {
  background: var(--background-secondary);
}

#app-mount #guild-header-popout .item-1tOPte.colorPremium-p4p7qO {
  color: rgb(var(--discord-nitro));
}
#app-mount #guild-header-popout .item-1tOPte.colorPremium-p4p7qO .icon-LYJorE {
  color: rgb(var(--discord-nitro));
}
#app-mount #guild-header-popout .item-1tOPte.colorBrand-ROmMP1 {
  color: rgb(var(--discord-blurple));
}
#app-mount #guild-header-popout .item-1tOPte.colorBrand-ROmMP1 .icon-LYJorE {
  color: rgb(var(--discord-blurple));
}
#app-mount #guild-header-popout .item-1tOPte.colorDanger-2qLCe1 {
  color: rgb(var(--discord-red));
}
#app-mount #guild-header-popout .item-1tOPte.colorDanger-2qLCe1 .icon-LYJorE {
  color: rgb(var(--discord-red));
}

#app-mount .container-2McqkF {
  background: transparent;
  box-shadow: none;
}
#app-mount .container-2McqkF .displayedNick-2dDbfG,
#app-mount .container-2McqkF .filter-5YbOzJ,
#app-mount .container-2McqkF .header-3A13BX {
  color: var(--text-normal);
}
#app-mount .container-2McqkF .answer-2fBfuP,
#app-mount .container-2McqkF .displayUsername-14aOpK {
  color: var(--text-muted);
}
#app-mount .container-2McqkF .option-2KkUJO .plusIcon-2V7coV {
  color: var(--text-normal);
}
#app-mount .container-2McqkF .option-2KkUJO.selected-rZcOL- {
  background: var(--white);
}
#app-mount .container-2McqkF .option-2KkUJO.selected-rZcOL-:after {
  background: linear-gradient(90deg, transparent, var(--white-double));
}
#app-mount .container-2McqkF .option-2KkUJO:after {
  background: transparent;
}
#app-mount .container-2McqkF .react-datepicker,
#app-mount .container-2McqkF .react-datepicker__header {
  background: transparent;
}
#app-mount .container-2McqkF .react-datepicker__month {
  background: var(--background-secondary);
  border-radius: 3px;
}
#app-mount .container-2McqkF .react-datepicker__day {
  border-color: var(--white);
  background: var(--white);
}
#app-mount .container-2McqkF .react-datepicker__day--selected:after {
  background: var(--gradient);
}
#app-mount .container-2McqkF .react-datepicker__day--disabled,
#app-mount .container-2McqkF .react-datepicker__day--outside-month {
  background: transparent;
}
#app-mount .searchAnswer-23w-CH {
  background: var(--white);
  margin-left: 0;
}
#app-mount .searchFilter-2UfsDk {
  background: var(--white);
}

#app-mount .autocomplete-3NRXG8 {
  box-shadow: none;
}
#app-mount .autocomplete-3NRXG8 .selectorSelected-1_M1WV {
  background: var(--white);
}
#app-mount .autocomplete-3NRXG8 .divider-1bJsnZ {
  background-color: var(--white);
}
#app-mount .autocomplete-3NRXG8 .description-11DmNu,
#app-mount .autocomplete-3NRXG8 .descriptionUsername-J_75O8 {
  color: var(--text-normal);
}
#app-mount .autocomplete-3NRXG8 .descriptionDiscriminator-tCKMLV {
  color: var(--text-muted);
}

#app-mount .messagesPopoutWrap-1MQ1bW {
  box-shadow: none;
}

#app-mount .container-enaOkj {
  background: var(--background-secondary);
  margin: 0 10px 10px;
  border-radius: 3px;
  padding: 0;
  overflow: hidden;
}
#app-mount .channelHeader-DFRX8q {
  background: transparent;
  padding: 15px 15px 0;
  height: auto;
  position: static;
}
#app-mount .channelHeader-DFRX8q .tertiary-1e-lAP,
#app-mount .channelHeader-DFRX8q .item-3XjbnG.selected-g-kMVV {
  background: var(--white);
}
#app-mount .channelHeader-DFRX8q .tertiary-1e-lAP:hover,
#app-mount .channelHeader-DFRX8q .item-3XjbnG.selected-g-kMVV:hover {
  background: var(--white-double);
}
#app-mount .container-iA3Qrz {
  margin: 0 16px 16px;
  padding: 0;
  border-radius: 3px;
  box-sizing: border-box;
  background: var(--white);
}
#app-mount .messageContainer-3VTXBC {
  padding: 15px 15px 15px 0;
  box-sizing: border-box;
}

#app-mount .container-2O1UgZ .container-2oNtJn {
  background: var(--white);
}

#app-mount .container-2rzKKA {
  border: none;
  background: var(--white);
}
#app-mount .container-2rzKKA:hover {
  background: var(--white-double);
}

#app-mount .modal-3c3bKg {
  transform: scale(1) translateZ(0px) !important;
  -webkit-animation: fadeInTop 0.3s ease forwards !important;
          animation: fadeInTop 0.3s ease forwards !important;
}
#app-mount .modal-2RrUKJ {
  background-color: transparent;
  box-shadow: none;
}
#app-mount .modal-2RrUKJ .cardWarning-2yPNAa {
  background-color: rgba(var(--discord-yellow), 0.2);
  border: 2px solid rgb(var(--discord-yellow));
}
#app-mount .modal-2RrUKJ .footer-1Ip3Sd {
  box-shadow: none;
  background: var(--background-secondary);
}
#app-mount .footer-2gL1pp {
  background: var(--background-secondary);
  box-shadow: none;
}

#app-mount .root-8LYsGj {
  background: transparent;
}
#app-mount .root-8LYsGj .topSectionNormal-2-vo2m {
  background: var(--background-secondary);
}
#app-mount .root-8LYsGj .topSectionSpotify-1lI0-P {
  background: rgba(var(--discord-spotify), 0.3);
}
#app-mount .root-8LYsGj .topSectionPlaying-1J5E4n {
  background: var(--gradient-50);
}
#app-mount .root-8LYsGj .topSectionStreaming-1Tpf5X {
  background: rgba(var(--discord-twitch), 0.3);
}
#app-mount .root-8LYsGj .topSectionXbox-3fWLjS {
  background: rgba(var(--discord-xbox), 0.3);
}
#app-mount .root-8LYsGj .svg-2azL_l {
  z-index: 1;
}
#app-mount .root-8LYsGj .body-3ND3kc {
  background: transparent;
}
#app-mount .root-8LYsGj .tabBarContainer-1s1u-z {
  border: none;
}
#app-mount .root-8LYsGj .userInfoSection-2acyCx {
  border: none;
}
#app-mount .root-8LYsGj .connectedAccount-36nQx7 {
  background: var(--background-secondary);
  border: none;
}

#app-mount .uploadModal-2ifh8j {
  position: relative;
  box-shadow: none;
}
#app-mount .uploadModal-2ifh8j .inner-3nWsbo {
  margin: 0;
  position: relative;
  z-index: 2;
}
#app-mount .uploadModal-2ifh8j .footer-3mqk7D {
  background: transparent;
  box-shadow: none;
  position: relative;
  z-index: 2;
}
#app-mount .uploadModal-2ifh8j:before {
  content: "";
  position: absolute;
  background: var(--popout-modal-image) center/cover fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
  pointer-events: none;
  border-radius: 5px;
}
#app-mount .uploadModal-2ifh8j:after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 3px;
  background: rgba(0, 0, 0, var(--popout-modal-brightness));
  box-shadow: var(--tint);
  z-index: 1;
  -webkit-backdrop-filter: blur(var(--popout-modal-blur));
          backdrop-filter: blur(var(--popout-modal-blur));
}

#app-mount .root-1gCeng {
  box-shadow: none;
  background: transparent;
}
#app-mount .root-1gCeng .colorHeaderPrimary-jN_yGr {
  color: #fff;
}
#app-mount .root-1gCeng .colorHeaderSecondary-g5teka {
  color: #ddd;
}
#app-mount .root-1gCeng .container-UC8Ug1,
#app-mount .root-1gCeng .lookFilled-1Gx00P.colorGrey-2DXtkV {
  background: rgba(255, 255, 255, 0.1);
}
#app-mount .root-1gCeng .container-UC8Ug1:hover,
#app-mount .root-1gCeng .lookFilled-1Gx00P.colorGrey-2DXtkV:hover {
  background: rgba(255, 255, 255, 0.15);
}
#app-mount .root-1gCeng .colorStandard-21JIj7 {
  color: #fff;
}
#app-mount .root-1gCeng .footer-2gL1pp {
  background: rgba(0, 0, 0, 0.2);
}
#app-mount .root-1gCeng .backButton-iA7KIs {
  color: #ddd;
}
#app-mount .root-1gCeng .backButton-iA7KIs:hover {
  color: #fff;
}
#app-mount .root-1gCeng .input--jS-j2 {
  background: transparent;
}
#app-mount .root-1gCeng .input-2g-os5 {
  background: rgba(255, 255, 255, 0.1);
  color: #fff;
}
#app-mount .root-1gCeng .sampleLink-2NLvZg {
  color: #ddd;
}

#app-mount .quickswitcher-pKcM9U {
  box-shadow: none;
  padding: 20px;
}
#app-mount .quickswitcher-pKcM9U .scrollerOuter-3FLELE {
  margin-top: 10px;
  margin-right: 0;
  border-radius: 3px;
}
#app-mount .quickswitcher-pKcM9U .scroller-2qwVWY {
  padding: 10px 5px 10px 10px;
  box-sizing: border-box;
}
#app-mount .quickswitcher-pKcM9U .scroller-2qwVWY > div[style*="width: 100%;"] {
  display: none;
}
#app-mount .quickswitcher-pKcM9U .protip-1jXzAl {
  display: none;
}

#app-mount .modalRoot-1Kx4Hb .header-1TKi98 {
  padding-top: 150px;
}
#app-mount .modalRoot-1Kx4Hb .art-347BZj {
  position: absolute;
  transform: translate(-50%, 20px);
  width: 150px;
}
#app-mount .modalRoot-1Kx4Hb .header-3C6qT5 {
  padding-top: 0;
}

#app-mount .scroller-2GkvCq,
#app-mount .reactors-1VXca7 {
  background: transparent;
}

#app-mount .image-3HC6rC {
  filter: grayscale(1);
  opacity: 0.5;
}
#app-mount .container-36u7Lw {
  background: rgba(0, 0, 0, var(--middle-brightness));
}

#app-mount .content-1SgpWY .discoverHeader-1TWTqG {
  margin: 0 0 10px;
  height: 48px;
  display: flex;
  align-items: center;
  padding-left: 10px;
}
#app-mount .content-1SgpWY .categoryItem-3zFJns.selected-1-Z6gm .itemInner-3gVXMG {
  background: var(--gradient);
}
#app-mount .content-1SgpWY .pageWrapper-2PwDoS {
  background: rgba(0, 0, 0, var(--middle-brightness));
}
#app-mount .content-1SgpWY .pageWrapper-2PwDoS .scrollerWrap-2lJEkd {
  margin-top: 48px;
  margin-bottom: 48px;
}
#app-mount .content-1SgpWY .card-2TuZPZ {
  background: var(--background-secondary);
}
#app-mount .content-1SgpWY .card-2TuZPZ:hover {
  box-shadow: none;
}
#app-mount .content-1SgpWY .footer-26kPv_ {
  opacity: 0;
  pointer-events: none;
}

#app-mount .container-2cd8Mz {
  background: rgba(0, 0, 0, var(--middle-brightness));
}
#app-mount .container-2cd8Mz .inset-SbsSFp {
  background-color: var(--background-secondary);
}
#app-mount .container-2cd8Mz .itemCard-3Etziu:hover {
  background: var(--white);
}
#app-mount .container-2cd8Mz .nowPlayingColumn-1eCBCN {
  background: rgba(0, 0, 0, var(--right-brightness));
}

#app-mount .perksModal-fSYqOq {
  background-color: rgba(0, 0, 0, var(--middle-brightness));
  background-image: none;
  margin: var(--window-padding);
  border-radius: var(--window-roundness);
}
#app-mount .tierWrapper-W9ajqp {
  box-shadow: none !important;
}
#app-mount .ctaBar-2UsjF2,
#app-mount .tier-12tKuZ {
  background: var(--background-secondary);
}
#app-mount .tierHeader---JJFb {
  background-color: var(--background-secondary);
  color: var(--text-normal);
}
#app-mount .tierLock-3CSxSX {
  color: var(--text-normal);
}
#app-mount .tierBody-16Chc9 {
  background: transparent;
}
#app-mount .perk-2WeBWW {
  background-color: var(--background-secondary);
}

#app-mount .applicationStore-2nk7Lo {
  background: rgba(0, 0, 0, var(--middle-brightness));
}

#app-mount [aria-label*=SETTINGS] .sidebarRegionScroller-FXiQOh {
  background-color: rgba(0, 0, 0, var(--left-brightness));
}
#app-mount [aria-label*=SETTINGS] .multiInput-1e2xJ7 .input-2g-os5 {
  background: transparent;
}
#app-mount [aria-label*=SETTINGS] .description-3_Ncsb,
#app-mount [aria-label*=SETTINGS] .h5-18_1nd:not(.isEnabled-2qCZy8),
#app-mount [aria-label*=SETTINGS] .labelDescriptor-1PqHgD,
#app-mount [aria-label*=SETTINGS] .viewBody-2Qz-jg {
  color: var(--text-normal);
}

#app-mount #user-settings .authedApp-1tw-eT {
  background: var(--background-secondary);
}
#app-mount #user-settings .connection-1fbD7X {
  position: relative;
  overflow: hidden;
  background-color: transparent !important;
  box-shadow: none;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(0, 154, 229)"] {
  background: rgba(0, 154, 229, 0.2) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(2, 31, 37)"] {
  background: rgba(2, 31, 37, 0.3) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(255, 69, 0)"] {
  background: rgba(255, 69, 0, 0.2) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(29, 185, 84)"] {
  background: rgba(29, 185, 84, 0.2) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(24, 35, 50)"] {
  background: rgba(24, 35, 50, 0.4) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(89, 54, 149)"] {
  background: rgba(89, 54, 149, 0.3) !important;
}
#app-mount #user-settings .connection-1fbD7X .integration-3kMeY4 {
  background: var(--white);
  border: none;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(29, 161, 242)"] {
  background: rgba(29, 161, 242, 0.2) !important;
}
#app-mount #user-settings .connection-1fbD7X[style*="rgb(203, 33, 32)"] {
  background: rgba(203, 33, 32, 0.2) !important;
}
#app-mount #user-settings .connectionHeader-2rV1ze {
  background: transparent;
  border: none;
  margin-bottom: 0;
}
#app-mount #user-settings .connectionDelete-XXTMqE {
  border: none;
  background: var(--white);
  transition: 0.2s ease;
}
#app-mount #user-settings .connectionDelete-XXTMqE:after, #app-mount #user-settings .connectionDelete-XXTMqE:before {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 2px;
  height: 16px;
}
#app-mount #user-settings .connectionDelete-XXTMqE:before {
  transform: translate(-50%, -50%) rotate(45deg);
}
#app-mount #user-settings .connectionDelete-XXTMqE:after {
  transform: translate(-50%, -50%) rotate(-45deg);
}
#app-mount #user-settings .connectionDelete-XXTMqE span {
  display: none;
}
#app-mount #user-settings .connectionDelete-XXTMqE:hover {
  background: var(--white-double);
}
#app-mount #user-settings .connectionDelete-XXTMqE:active {
  background: var(--white-triple);
}
#app-mount #user-settings .card-2ART2V:before {
  border-color: transparent;
  background: var(--white);
}
#app-mount #user-settings .game-3x3aDt {
  box-shadow: 0 1px 0 0 var(--background-modifier-accent);
}
#app-mount #user-settings .item-3eFBNF {
  box-shadow: inset 0 -1px 0 0 var(--background-modifier-accent);
}

#app-mount .info-1sUqUG .colorMuted-20987_:first-child:before {
  content: var(--version);
  display: block;
}
#app-mount .contentRegion-3HkfJJ {
  background: rgba(0, 0, 0, var(--middle-brightness));
}
#app-mount .auditLog-3jNbM6 {
  border: none;
  border-radius: 3px;
  overflow: hidden;
}
#app-mount .header-GwIGlr {
  background: var(--background-secondary);
}
#app-mount .timestamp-1mruiI {
  color: var(--text-muted);
}
#app-mount .divider-1pnAR2 {
  display: none;
}
#app-mount .changeDetails-bk98pu {
  background: var(--background-secondary);
}

#app-mount #bd-settingspane-container h3 {
  color: var(--text-normal);
}
#app-mount #bd-settingspane-container .style-description {
  color: var(--text-default);
  border-color: var(--background-modifier-accent);
}

#app-mount #bd-settings-sidebar .ui-tab-bar-item {
  color: var(--text-muted);
}
#app-mount #bd-settings-sidebar .ui-tab-bar-item:hover {
  color: var(--text-normal);
  background-color: var(--background-modifier-hover);
}
#app-mount #bd-settings-sidebar .ui-tab-bar-item.selected {
  background: var(--background-modifier-selected);
  color: var(--text-normal);
}

#app-mount .editor-wrapper {
  background: var(--background-secondary);
}
#app-mount #bd-customcss-detach-container {
  background: var(--background-secondary);
  overflow: hidden;
}
#app-mount #bd-customcss-detach-container .editor-wrapper {
  height: calc(100% + 41px);
}
#app-mount.bd-detached-editor .winButton-iRh8-Z {
  right: calc(30% + 20px) !important;
}
#app-mount #bd-customcss-attach-controls {
  height: auto;
}
#app-mount .ace_active-line,
#app-mount .ace_gutter-active-line,
#app-mount .ace_selection {
  background: var(--white-double);
}
#app-mount .ace_editor {
  background-color: transparent;
}
#app-mount .ace_gutter {
  background: var(--background-secondary);
}
#app-mount .help-text,
#app-mount span[style="font-size: 10px; margin-left: 5px;"] {
  display: none;
}
#app-mount #bd-customcss-attach-controls {
  background: var(--background-secondary);
  box-shadow: inset 0 0 0 100vmax var(--background-secondary);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px;
  box-sizing: border-box;
}
#app-mount #bd-customcss-attach-controls .checkbox-group li {
  margin-top: 0;
}
#app-mount #bd-customcss-attach-controls button {
  margin: 0 0 0 10px;
  border-radius: 3px !important;
  border: none !important;
  background: var(--white);
  color: var(--text-normal);
  transition: 0.2s ease;
}
#app-mount #bd-customcss-attach-controls button:active, #app-mount #bd-customcss-attach-controls button:hover {
  background: var(--white-double);
}

html.platform-win .scroller-2TZvBN {
  padding-top: 10px;
}

html.platform-osx .macButtons-2MuSAC {
  position: absolute;
  top: var(--window-padding);
  left: var(--window-padding);
  background: rgba(0, 0, 0, var(--serverlist-brightness));
  width: 72px;
  border-top-left-radius: var(--window-roundness);
}
html.platform-osx .wrapper-1Rf91z {
  margin-top: 30px;
}
html.platform-osx .scroller-2TZvBN {
  padding-top: 15px;
}

#app-mount .xenoLib-notifications {
  padding: calc(var(--window-padding) * 2 + 48px) calc(var(--window-padding) * 2) calc(var(--window-padding) * 2) calc(var(--window-padding) * 2);
  box-sizing: border-box;
}
#app-mount .xenoLib-notification:not(:only-child) {
  margin-bottom: 15px;
}
#app-mount .xenoLib-notification-content-wrapper {
  padding: 0;
  box-sizing: border-box;
  z-index: 10;
}

@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeInTop {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
@keyframes fadeInTop {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
