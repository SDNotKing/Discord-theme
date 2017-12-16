/**********************************************************************************************************************************/
/****************************************************************/
/*Alls*/
.badge {
    background-color: #11d4ad;
    border: 1px solid rgba(0, 0, 0, 0.5);
    color: #000000;
}
/*THIS IS AN EXAMPLE OF BAD DESIGN:
* {
    transition: all 400ms ease;
}*/
/****************************************************************/
/****************************************************************/
/*Acount*/
.account .avatar-small .status {
    bottom: -1px;
}
/****************************************************************/
/****************************************************************/
/*Animations*/
.message:not(.message-sending),
.message-content:not(.message-sending),
.image:not(.message-sending),
.avatar-large:not(.message-sending),
.tooltip,
.guild,
.section,
.context-menu,
.friends-row,
.channel,.user-settings-modal,
.channel-voice-states,
.selected:before,
.markdown-modal,
.icon-muted,
.icon-deafened,
.empty-message,
.popout-menu,
.channel-members,
.user-popout,
.emoji-picker,
.popout,
.option-popout {
    animation: fadeScreen 0.5s;
}
/*Hearts*/
img[alt*=":heart:"], 
img[alt*=":hearts:"], 
img[alt*=":green_heart:"], 
img[alt*=":blue_heart:"], 
img[alt*=":purple_heart:"],
img[alt*=":yellow_heart:"], 
img[alt*=":heartbeat:"], 
img[alt*=":heartpulse:"], 
img[alt*=":black_heart:"], 
img[alt*=":sparkling_heart:"] { animation: heartbeat 1s infinite;}
/*Emojis     */
/*Money Wings*/ img[alt*=":money_with_wings:"] {animation: wobble 2s infinite;}
/*Kiss       */ img[alt*=":kiss:"] {animation: heartbeat 1s infinite;}
/*Hammer     */ img[alt*=":hammer:"] {animation: wobble 0.5s infinite;}
/*Pickaxe    */ img[alt*=":pick:"] {animation: wobble 0.5s infinite;}
/*Bomb       */ img[alt*=":bomb:"] {animation: bomb 2s infinite;}
/*Boom       */ img[alt*=":boom:"] {animation: boom 2s infinite;}
/*Eyes       */ img[alt*=":eyes:"] {animation: eyes 4s infinite;animation-timing-function:steps(1);}
/*Laughing   */ img[alt*=":laughing:"] {transform: rotate(-90deg);}
/*Heart Eyes */ img[alt*=":heart_eyes:"] {animation: heartbeat 1s infinite;}
/*Joyful     */ img[alt*=":joy:"] {animation: joy 2s infinite;}
/*Upside Down*/ img[alt*=":upside_down:"] {animation: wobble 2s infinite;}
/*Scream     */ img[alt*=":scream:"], img[alt*=":scream_cat:"] {animation: scare 2s infinite;}
/*ROFL       */ img[alt*=":rofl:"] {animation: rofl 2s infinite;}
/*Sneezing   */ img[alt*=":sneezing_face:"] {animation: wobble 1s infinite;}
/*Joyful Cat */ img[alt*=":joy_cat:"] {animation: joy 2s infinite;}
/*Heart Eyes */ img[alt*=":heart_eyes_cat:"] {animation: heartbeat 1s infinite;}
/*Waving     */ img[alt*=":wave:"] {animation: wobble 2s infinite;}
/*Angry      */ img[alt*=":angry:"], .emoji[alt*="Angery"], .emoji[alt*="Thonkery"] {animation: vibrate 0.2s infinite;}
/*Soccer     */ img[alt*=":soccer:"] {animation: rotate 2s infinite;} 
/*Basketball */ img[alt*=":basketball:"] {animation: rotate 2s infinite;}
/*Baseball   */ img[alt*=":baseball:"] {animation: rotate 2s infinite;} 
/*Tennis     */ img[alt*=":tennis:"] {animation: rotate 2s infinite;}
/*Gear       */ img[alt*=":gear:"] {animation: rotate 2s infinite;}
/*Disc & CD  */ img[alt*=":cd:"], img[alt*=":dvd:"] {animation: rotate 2s infinite;} 
/*Snowflake  */ img[alt*=":snowflake:"] {animation: rotate 2s infinite;}
/*Sun        */ img[alt*=":sunny:"] {animation: rotate 2s infinite;}
/*Hourglass  */ img[alt*=":hourglass:"] {animation: hourglass 2s infinite;}
/*mmLol      */ .emoji[alt*="mmLol"] {animation: mmlol 5s infinite;}
.emoji.jumboable { transition: all .6s ease; }
.emoji.jumboable:hover {
resize: both;
width: 42pt;
height: 42pt;
-webkit-filter: drop-shadow(0 0 5px black);
}
.emoji { transition: all .6s ease; }
.emoji:hover {
resize: both;
width: 32pt;
height: 32pt;
-webkit-filter: drop-shadow(0 0 5px black);
}
/*Reveal Up*/
.markup, .accessory, .comment {
animation: revealUp 0.7s;
}
/****************************************************************/
/****************************************/
/*  Flash, Open Animation, Emojis       */
/*======================================*/
/*              Animations              */
/*======================================*/
/*                                      */
/****************************************/
@-webkit-keyframes flash2 {
0%{
opacity: 0;
-webkit-filter: blur(0px);
transform: translateX(-100%);
}
50%{
opacity: 0;
}
75%{
-webkit-filter: blur(1px);
}
100%{
opacity: 1;
-webkit-filter: blur(0px);
transform: translateX(initial);
}
}
@keyframes flash2 {
0%{
opacity: 0;
transform: translateX(-100%);
}
50%{
opacity: 0;
}
100%{
opacity: 1;
transform: translateX(initial);
}
}
@keyframes guildtip {
0% {
opacity: 0;
filter:brightness();
box-shadow: inset 4px 0 30px 10px rgba(180,180,220,0)
transform: translateX(-100%);
}
50% {
opacity: 0;
}
60% {opacity: 1;}
100% {
opacity: 1;
filter:brightness(110%);
box-shadow: inset 4px 0 30px 10px rgba(180,180,220,.5)
transform: translateX(initial);
}
}
@keyframes guildtip2 {
0% {
box-shadow: inset 4px 0 30px 10px rgba(180,180,220,0)
}
100% {
box-shadow: inset 4px 0 30px 10px rgba(180,180,220,.5)
}
}
@-webkit-keyframes glowpulse {
0%{
-webkit-filter: drop-shadow(0 0 0 rgba(0,114,114,0));
}
100%{
-webkit-filter: drop-shadow(0 0 5px rgba(0,114,114,1)) drop-shadow(0 0 5px rgba(0,114,144,1)) drop-shadow(0 0 5px rgba(0,114,114,1)) saturate(200%);
}
}
@keyframes glowpulse {
0%{
filter: drop-shadow(0 0 0 rgba(0,111,114,0));
}
100%{
filter: drop-shadow(0 0 5px rgba(0,114,114,1)) drop-shadow(0 0 5px rgba(0,0,114,1)) drop-shadow(0 0 5px rgba(0,114,114,1)) saturate(200%);
}
}
/*Hue*/
@-webkit-keyframes hue {
0%{ -webkit-filter: hue-rotate(0deg); }
100%{ -webkit-filter: hue-rotate(360deg); }
}
/*Working*/
@-webkit-keyframes working {
25%{ content: "Working";   }
50%{ content: "Working.";  }
75%{ content: "Working.."; }
100%{content: "Working...";}
}
@keyframes working {
25%{ content: "Working";   }
50%{ content: "Working.";  }
75%{ content: "Working.."; }
100%{content: "Working...";}
}
@keyframes fadeScreen {
from { opacity: 0;   }
to {   opacity: 100; }
}
@keyframes wobble   {0%,100%{transform:rotate(20deg)}50%{transform:rotate(-20deg)}}
@keyframes scare    {0%,100%{transform:rotate(9deg)}50%{transform:rotate(-9deg)}}
@keyframes hourglass{0%,100%,41%{transform:rotate(0)}20%,40%{transform:rotate(-180deg)}}
@keyframes rotate   {0%{transform:rotate(0)}100%{transform:rotate(360deg)}}
@keyframes rofl     {0%{transform:rotate(45deg)}100%{transform:rotate(404deg)}}
@keyframes heartbeat{0%,100%,40%,80%{transform:scale(.75)}20%,60%{transform:scale(1)}}
@keyframes joy      {0%,100%,50%{transform:scale(.9)}25%,75%{transform:scale(1)}}
@keyframes boom     {0% {transform:scale(.1)}20% {transform:scale(1)}80% {transform:scale(1);opacity: 1;}100%{opacity: 0;}}
@keyframes bomb     {0%,100%,20%{transform:scale(1)}90%{transform:scale(.6)}95%{transform:scale(1.5)}}
@keyframes eyes     {0%,25%,75%{transform:scaleX(1)}50%,100%{transform:scaleX(-1)}}
@keyframes mmlol    {0% { transform: rotate(0deg); }69% { transform: rotate(0deg); }70% { transform: rotate(-90deg); }99% { transform: rotate(-90deg); }100% { transform: rotate(0deg); }}
@keyframes vibrate  {25%{transform: translateX(3px) translateY(-2px)}50%{transform: translateX(-1px) translateY(3px)}75%{transform: translateX(-4px) translateY(-2px)}100%{transform: translateX(2px) translateY(-1px)}}
/*Message reveal*/
@keyframes revealUp {
0%, 60%, 75%, 100% {
-webkit-transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
}
0% {
opacity: 0;
-webkit-transform: translate3d(0, 100px, 0);
transform: translate3d(0, 100px, 0);
}
60% {
opacity: 0.5;
-webkit-transform: translate3d(0, 7px, 0);
transform: translate3d(0, 7px, 0);
}
75% {
opacity: 1;
-webkit-transform: translate3d(0, 5px, 0);
transform: translate3d(0, 5px, 0);
}
100% {
-webkit-transform: translate3d(0, 0, 0);
transform: translate3d(0, 0, 0);
}
}
/*modalanim*/
@-webkit-keyframes modalanim {
from {
-webkit-transform: scale(1));
transform: scale(1));
opacity: 0;
}
to {
-webkit-transform: scale(1);
transform: scale(1);
opacity: 1;
}
}
@keyframes modalanim {
from {
-webkit-transform: scale(1));
transform: scale(1));
opacity: 0;
}
to {
-webkit-transform: scale(1);
transform: scale(1);
opacity: 1;
}
}
/*bg-in*/
@-webkit-keyframes bg-in {
0% { opacity: 0; }
100% {}
}
/*bg-in*/
@keyframes bg-in {
0% { opacity: 0; }
100% {}
}
/* Code assisted by http://www.cssnewbie.com/pure-css-bouncing-ball/#.WG1LYi_QdhE */
@keyframes moveX {
from { left: -1%; } to { left: 62%; }
}
@keyframes moveY {
from { top: -4%; } to { top: 84%; }
}
@-webkit-keyframes spinner {
from { -webkit-transform: rotateY(0deg);    }
to   { -webkit-transform: rotateY(-360deg); }
}
@keyframes spinner {
from { -moz-transform: rotateY(0deg);
-ms-transform: rotateY(0deg);
transform: rotateY(0deg);
}
to {
-moz-transform: rotateY(-360deg);
-ms-transform: rotateY(-360deg);
transform: rotateY(-360deg);
}
}
/****************************************************************/
/****************************************************************/
/*Animated Gifs*/
/*Thanks for using this theme!*/
/*HansAnonymous#8784*/
/*.avatar-profile[style*="168216897450541056"],
.avatar-large[style*="168216897450541056"],
.avatar-small[style*="168216897450541056"] {
background: url('https://i.imgur.com/3bbqVxD.gif') !important;
background-size: cover !important;
}*/

/*Howdy! It's ya girl Pierçalina#5403*/
.avatar-profile[style*="215925240646205440"],
.avatar-large[style*="215925240646205440"],
.avatar-small[style*="215925240646205440"] {
background: url('https://i.imgur.com/Kcx9An6.gif') !important;
background-size: cover !important;
}
/****************************************************************/
/****************************************************************/
/*Backface visibility*/
.markup,
body {
backface-visibility: hidden;
-webkit-backface-visibility: hidden;
}
/****************************************************************/
/****************************************************************/
/*Background*/
#friends,
.friends-table,
.guild-channels,
.channels-wrap,
.links,
.chat,
.messages-wrapper,
.title-wrap,
.content,
.chat-empty,
.private-channels,
.guild-header header,
.guild-header header:after,
.typing,
.divider-red span {
    background: transparent !important;
    border: 0 !important;
}
.markup pre code,
.theme-dark .layers, .layer {
background: transparent !important;
}
.channel-members-wrap,
.guilds-wrapper,
.channels-wrap .scrollerWrap-2uBjct,
.channels-wrap .flexChild-1KGW5q,
.container-iksrDt,
.container-3lnMWU,
#friends .friends-header, .chat .title-wrap,
.popout.popout-bottom-right.no-arrow.no-shadow,
.private-channels .search-bar,
.chat form .channel-text-area-default,
.headerBar-cxbhPD {
box-shadow: none;
}
.typing, .typing-animate {
background: transparent !important;
background-color: rgba(0,0,0,0.0) !important;
}
.header-1tSljs,
.container-iksrDt,
.popout-open .header-1tSljs{
background: linear-gradient(to right, rgba(0, 0, 0, 0.05), rgba(0, 0, 0, 0.04)) !important;
}
.headerBar-cxbhPD{
background: linear-gradient(to right, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.04)) !important;
}
.header-1tSljs:hover {
background: linear-gradient(to right, rgba(0, 0, 0, 0.08), rgba(0, 0, 0, 0.07)) !important;
}
.channels-3g2vYe{
background: linear-gradient(to right, rgba(0, 0, 0, 0.05), rgba(0, 0, 0, 0.04));
}
.chat .content,
.theme-dark .title-qAcLxz{
background: linear-gradient(to right, rgba(0, 0, 0, 0.02), rgba(0, 0, 0, 0));
}
.guilds-wrapper, .guilds, .guilds.scroller {
background: linear-gradient(to right, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.03));
}
.guild-channels .channel-text:hover {
background: linear-gradient(to right, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.0));
}
.theme-dark .links, .theme-dark .links {
border-top: 1px solid #1c1e22;
}
.theme-light .account, .theme-light .links {
border-top: 1px solid #1c1e22;
}
.markup pre, .markup code {
/*font-family: 'MS ????', 'Ubuntu Mono', Consolas, Monaco, monospace !important;*/
font-size: 13px;
background: rgba(10, 10, 10, 0.7) !important;
border: 0 !important;
border-radius: 0 !important;
}
.CodeMirror-scroll,
#bd-customcss-attach-controls,
.autocomplete-1TnWNR.autocomplete-1LLKUa {
background-color: rgba(0,14,14,0.4) !important;
}
.CodeMirror-gutter.CodeMirror-linenumbers {
transform: translateY(-5px);
background-color: rgba(0,7,7,0.4) !important;
}
#bd-customcss-detach-controls-button .btn.btn-primary,
.selectorSelected-2M0IGv.selector-nbyEfM.selectable-3iSmAf,
.innerEnabled-gLHeOL.inner-3if5cm.flex-3B1Tl4.innerAutocomplete-2qsvzH,
.buttonBrandFilledDefault-2Rs6u5.buttonFilledDefault-AELjWf.buttonDefault-2OLW-v.button-2t3of8.buttonFilled-29g7b5.buttonBrandFilled-3Mv0Ra.mediumGrow-uovsMu {
background-color: rgba(0,28,28,0.4) !important;
}
#bd-customcss-detach-controls-button .btn.btn-primary:hover,
.autocompleteRowVertical-3_UxVA.autocompleteRow-31UJBI,
.buttonBrandFilledDefault-2Rs6u5.buttonFilledDefault-AELjWf.buttonDefault-2OLW-v.button-2t3of8.buttonFilled-29g7b5.buttonBrandFilled-3Mv0Ra.mediumGrow-uovsMu:hover {
background-color: rgba(0,56,56,0.8) !important;
}
.content-region#bd-settingspane-container .content-column.default {
background: transparent !important;
}
.bda-slist li{
background-color: rgba(0,28,28,0.4) !important;
}
.private-channel-call {
background-color: rgba(0,0,0,0.7);
box-shadow: inset 0 -4px 10px 0 rgba(0,0,0,0.0);
background-image: url();
}
.private-channels .channel:hover,
.private-channels .channel.selected {
background: -webkit-linear-gradient(left,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
}
#rmenu {
background: #007272;
border: 1px solid #007272;
}
.mention {
background: rgba(255,255,255,0.05);
}
.layer, .layers { background: rgba(0,0,0,.05)!important; }
.create-guild-container {
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
}
.create-guild-container .actions {
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
}
.create-guild-container .actions .action.create, .create-guild-container .actions .action.join {
background: rgba(0,57,57,0.7);
}
.inner-1_1f7b,
.modal-3HOjGZ.modal-2CasLk.sizeSmall-1sh0-r,
.headerNormal-1cioxU.header-3mZJcV,
.body-3rkFrF,
.footer-2J5zqP {
background: rgba(0,90,135,0.9);
}
.body-3rkFrF{
    padding-bottom: 8px;
    border-bottom: none;
}
.scroller-wrap .scroller::-webkit-scrollbar-thumb, .scroller-wrap .scroller::-webkit-scrollbar-track-piece{
background-color: rgba(0, 0, 0, 0.42) !important;
border: none !important;
}
.settings .settings-inner .settings-panel{
color: rgba(255, 255, 255, 0.9);
}
#rtc-connection{
background-color: rgba(0, 0, 0, 0.42);
border: none;
}
#rtc-connection .btn-group{
border-radius: 0;
border: none;
}
#rtc-connection .btn{
background-color: rgba(0, 0, 0, 0.5);
}
#rtc-connection .btn-info{
border-radius: 0;
border: none;
}
#rtc-connection .btn-disconnect{
box-shadow: none;
}
#rtc-connection-popout hr{
border-color: rgba(255, 255, 255, 0.3);
}
#rtc-debug-modal #users-section .user-list{
border-right: 1px solid rgba(255, 255, 255, 0.2);
}
#rtc-debug-modal .diagnostics-checkbox{
border-radius: 0;
}
h3{
color: rgba(255, 255, 255, 0.9);
}
.popout.popout-top section:after, .popout.popout-top-right section:after{
border-top-color: #7289da;
}
.popout section{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0 !important;
}
.popout header,
.user-popout {
border-radius: 0 !important;
}
.popout header{
background-color: rgba(42, 42, 42, 0.8);
}
.popout-menu{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.popout-menu .popout-menu-item.invite:hover,
.popout-menu .popout-menu-item.leave:hover{
background-color: rgba(255, 255, 255, 0.2);
}
.popout-menu .popout-menu-item{
color: rgba(255, 255, 255, 0.8);
}
.popout-menu .popout-menu-item:hover{
color: rgba(255, 255, 255, 0.9);
background-color: rgba(255, 255, 255, 0.2);
}
.popout-menu .popout-menu-separator{
border-color: rgba(255, 255, 255, 0.2);
}
.notification-settings-modal .notification-settings-modal-channel-settings-list{
box-shadow: none;
}
.channel-notification-settings .content label{
color: rgba(255, 255, 255, 0.8);
}
.channel-mute-button{
opacity: 0.5;
}
.channel-notification-settings{
border-color: rgba(255, 255, 255, 0.2);
}
.small-popout-box{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
border: 0;
}
.option-popout .btn-item{
color: rgba(255, 255, 255, 0.8);
}
.option-popout .btn-item:hover{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.9);
}
.modal-content{
background-color: rgba(0, 0, 0, 0);
}
.modal-content .form-inner p{
color: rgba(255, 255, 255, 0.3);
}
.private-channels .channel:hover,
.private-channels .channel.selected{
background: none;
}
.private-channels .channel:hover{
background-color: rgba(0, 0, 0, 0.2);
}
.private-channels .channel.selected{
background-color: rgba(0, 0, 0, 0.42);
}
.theme-dark .private-channel-recipients-invite .friend.selected{
background: none;
}
.theme-dark .private-channel-recipients-invite .friend:hover{
background: rgba(255, 255, 255, 0.2);
}
.theme-dark .private-channel-recipients-invite .friend{
background: none;
}
.private-channel-recipients-invite .footer button{
border-radius: 0;
}
.private-channel-call .btn-icon{
border-radius: 0;
}
.private-channel-call .btn-text{
border-radius: 0;
}
.theme-dark .chat .private-channel-call{
background-color: rgba(0, 0, 0, 0.05);
}
.theme-dark .ui-quick-select-popout{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.ui-quick-select-popout-option:hover{
background-color: rgba(255, 255, 255, 0.2) !important;
}
.incoming-call .title{
color: rgba(255, 255, 255, 0.9);
}
.incoming-call .incoming-call-inner{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.incoming-call .options .option{
border-radius: 0;
}
.ui-quick-select-popout-option.selected{
background-color: rgba(0, 0, 0, 0);
}
.theme-dark .themed-popout .footer{
background: none;
}
#friends .btn{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
#friends .friends-empty .btn{
border-radius: 0;
}
#friends .btn:hover{
background-color: rgba(255, 255, 255, 0.42);
}
#friends .friends-header .tab-bar .tab-bar-item {
border-radius: 0;
}
.theme-dark #friends .friends-table .friend-table-add-wrapper .friend-table-add-header{
background: 0 0;
border: 0;
}
.add-friend-input-wrapper{
border-radius: 0;
border: 0;
}
.theme-dark .add-friend-input-wrapper {
background-color: rgba(0, 0, 0, 0.42);
}
.theme-dark #friends .friends-header .tab-bar .tab-bar-item:hover:not(.selected){
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark #friends .friends-table .friends-row .friends-column-actions .friends-action{
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2);
}
#friends .friends-table .friends-row:hover:not(.selected){
background-color: rgba(0, 0, 0, 0.2);
border: 0;
border-radius: 0;
}
.chat form{
box-shadow: none;
}
.theme-dark .chat .has-more button {
background: rgba(0, 0, 0, 0.42);
border: 0;
border-radius: 0 !important;
}
.theme-dark .chat .jump-to-present-bar {
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
.theme-dark .chat .jump-to-present-bar:hover{
background-color: rgba(60, 60, 60, 0.8) !important;
}
.chat .jump-to-present-bar button{
color: rgba(255, 255, 255, 0.8);
}
div.guild-header{
background-color: rgba(0, 0, 0, 0.5);
height: 57px;
}
.theme-dark .friends-table .messages .divider:not(.red) div,
.theme-dark .messages-wrapper .messages .divider:not(.red) div{
background-color: rgba(255, 255, 255, 0.1);
}
.new-messages-indicator{
display: none;
}
.new-messages-indicator.bottom{
border-radius: 0;
}
.form .control-groups.control-separator{
border-color: rgba(255, 255, 255, 0.2);
}
.region-select .region-select-inner,
.region-select button{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
border: 0;
}
.region-select-name,
.region-select button{
color: rgba(255, 255, 255, 0.8);
}
.region-select button:hover{
background-color: rgba(255, 255, 255, 0.42);
color: rgba(255, 255, 255, 0.95);
}
.region-select-modal{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.region-select-modal .region-select-modal-header{
color: rgba(255, 255, 255, 0.9);
}
.region-select-modal .region-select-modal-option{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
border: 0;
}
.instant-invites .instant-invites-header{
border-color: rgba(255, 255, 255, 0.2);
}
.search-bar-tag{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
.search-bar.search-bar-light .search-bar-inner{
background-color: rgba(0, 0, 0, 0.5) !important;
border-radius: 0 !important;
border: 0;
}
.search-bar.search-bar-light input{
color: rgba(255, 255, 255, 0.8);
}
.guild-settings-modal-integrations .guild-settings-modal-integrations-header{
border-color: rgba(255, 255, 255, 0.2);
box-shadow: none;
}
.guild-settings-modal-integrations .guild-settings-modal-integrations-body.no-integrations p{
color: rgba(255, 255, 255, 0.5);
}
.guild-settings-modal-members{
background-color: rgba(0, 0, 0, 0);
}
.guild-settings-modal-members .guild-settings-modal-members-header .form .Select .Select-value{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
}
.guild-settings-modal-members .guild-settings-modal-members-header,
.guild-settings-modal-members .guild-settings-modal-list .member+.member{
border-color: rgba(255, 255, 255, 0.2);
}
.guild-settings-modal-members .guild-settings-modal-members-footer{
border-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .guild-settings-members-member .tag{
color: rgba(255, 255, 255, 0.7);
}
.guild-settings-modal .emoji-row .btn+.btn,
.guild-settings-modal .member-buttons .btn{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border-radius: 0;
border: 0;
}
.guild-settings-modal .member-buttons .btn:hover {
background-color: rgba(255, 255, 255, 0.42);
}
.guild-settings-modal .member-buttons .btn.btn-danger:hover{
background-color: rgba(255, 200, 200, 0.42);
}
.guild-settings-modal .emoji-row .btn.btn-danger,
.guild-settings-modal .member-buttons .btn.btn-danger{
border: 0;
}
#settings-roles .roles{
border-color: rgba(255, 255, 255, 0.2);
}
#settings-roles .roles header{
border-color: rgba(255, 255, 255, 0.2);
}
#settings-roles .roles li:hover{
background: rgba(255, 255, 255, 0.1) none;
}
#settings-roles .roles li.selected{
background: rgba(255, 255, 255, 0.2) none;
}
.color-picker .swatches .swatch.large{
border-radius: 0;
}
.color-picker-popout{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
border: 0;
box-shadow: none;
}
.guild-settings-modal-members .guild-settings-modal-list .member .member-username{
color: rgba(255, 255, 255, 0.8);
}
.color-picker-popout input{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border-radius: 0;
border: 0;
}
.color-picker .swatches .swatch.custom:after,
.color-picker .swatches .swatch.selected:after{
border-radius: 0;
}
.guild-settings-modal-emoji .guild-settings-modal-emoji-header p{
color: rgba(255, 255, 255, 0.5);
}
.guild-settings-modal-emoji .guild-settings-modal-emoji-header,
.guild-settings-modal-emoji .emoji-row{
border-color: rgba(255, 255, 255, 0.2);
}
.guild-settings-modal-emoji .emoji-row .emoji-name{
border-radius: 0;
border: 0;
}
.guild-settings-modal .emoji-row .btn{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
.guild-settings-modal .emoji-row .btn.btn-danger:hover{
background-color: rgba(255, 200, 200, 0.4);
}
.clipboard-input-inner{
background-color: rgba(255, 255, 255, 0.2);
border: 0;
border-radius: 0;
}
.clipboard-input-inner input{
background-color: rgba(255, 255, 255, 0);
color: rgba(255, 255, 255, 0.8);
}
.clipboard-input-inner button{
background-color: rgba(255, 255, 255, 0.6);
border: 0;
}
.clipboard-input-inner button:first-of-type:before{
background: none;
}
.webhooks .webhooks-header{
border-color: rgba(255, 255, 255, 0.2);
}
.webhooks .webhook{
background-color:rgba(255, 255, 255, 0.2);
border-radius: 0;
border: 0;
}
.webhooks .webhook .webhook-header .webhook-details .webhook-name{
color: rgba(255, 255, 255, 0.8);
}
.webhooks .webhook .webhook-header .webhook-details .webhook-created-on{
color: rgba(255, 255, 255, 0.5);
}
.ui-webhook-row .remove-webhook{
right: -24px !important;
}
.form .btn-clear{
background: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border-radius: 0;
border: 0;
}
.form .btn-clear:hover{
background: rgba(255, 255, 255, 0.4);
}
.tooltip{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.friends-header{
background-color: rgba(0, 0, 0, 0.5) !important;
height: 57px !important;
border: 0 !important;
}
.search-bar{
background-color: rgba(0, 0, 0, 0.5);
box-shadow: none;
}
.search-bar.search-bar-light{
background-color: rgba(0, 0, 0, 0);
}
.search-bar .search-bar-inner{
border: 0;
border-radius: 0;
}
.guild-channels .channel-text.selected,
.guild-channels .channel-text:hover{
background-size: 0 0 !important;
}
.guild-channels .channel-text.selected{
background-color: rgba(0, 0, 0, 0.42);
}
.guild-channels .channel-text:hover{
background-color: rgba(0, 0, 0, 0.2);
}
.create-guild-container{
background-color: rgba(0, 0, 0, 0);
}
.create-guild-container .create-or-join .form-inner{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.create-guild-container .action{
background-color: rgba(255, 255, 255, 0.2);
}
.create-guild-container .action.create .action-header,
.create-guild-container .action.join .action-header{
color: rgba(255, 255, 255, 0.8);
}
.theme-dark .channel-members{
background-color: rgba(0, 0, 0, 0);
}
.channel-members-wrap .scroller-wrap .scroller{
background: rgba(0, 0, 0, 0.2);
}
.theme-dark .channel-members .member.popout-open{
background: 0 0;
}
.channel-members .member:hover{
background: rgba(0, 0, 0, 0.42) !important;
}
.theme-dark .channel-members .member.popout-open{
background-color: rgba(0, 0, 0, 0.42) !important;
}
.theme-dark .channel-members .member:not(.disabled).popout-open,
.theme-dark .channel-members .member:not(.disabled):hover{
background: 0 0;
}
.theme-dark .channel-members .member:hover{
background-color: rgba(0, 0, 0, 0.2);
}
.member-roles .member-role{
color: rgba(255, 255, 255, 0.8);
border-radius: 0 !important;
background-color: rgba(255, 255, 255, 0.2);
border-color: rgba(255, 255, 255, 0.3);
}
.member-roles .member-role.member-role-add{
border-color: rgba(255, 255, 255, 0.3);
background-color: rgba(255, 255, 255, 0.15);
}
.user-popout .username-wrapper .discord-tag .username{
color: rgba(255, 255, 255, 0.9);
}
.user-popout .username-wrapper .discord-tag .discriminator{
color: rgba(255, 255, 255, 0.75);
}
#autocomplete-popout section{
background-color: rgba(42, 42, 42, 0.8);
}
#autocomplete-popout .row.selected{
background: none;
background-color: rgba(255, 255, 255, 0.1) !important;
}
#autocomplete-popout header{
background-color: rgba(33, 33, 33, 0.9);
}
#autocomplete-popout .row a,
#autocomplete-popout .row.selected a,
#autocomplete-popout .row:hover a{
color: rgba(255, 255, 255, 0.8);
}
#autocomplete-popout .empty h4{
color: rgba(255, 255, 255, 0.8);
}
.embed .image,
.embed video,
.embed .embed-video-actions .embed-video-actions-inner{
border-radius: 0;
}
.embed.embed-rich .embed-rich-thumb{
border-radius: 0;
}
.quick-message{
border: 0 !important;
border-radius: 0;
background-color: rgba(0, 0, 0, 0.3);
}
.quick-message.isBlocked{
background-color: rgba(0, 0, 0, 0.6);
}
.channel-textarea-guard button{
border-radius: 0;
}
input:disabled{
opacity: 0.3;
}
.markdown-modal{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.markdown-modal .markdown-modal-header{
border: 0;
}
.markdown-modal .markdown-modal-footer{
border: 0;
background-color: rgba(0, 0, 0, 0);
}
.markdown-modal.selectable .scroller{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .message-group .comment .markup .mention{
background-color: rgba(179, 224, 255, 0.1);
}
.theme-dark .message-group.is-local-bot-message{
background: rgba(42, 42, 42, 0.42) none;
border-bottom: 1px solid rgba(255, 255, 255, 0.04);
box-shadow: none;
}
.theme-dark .channel-textarea-inner{
border: 0;
border-radius: 0;
background-color: rgba(0, 0, 0, 0.42);
}
.theme-dark .channel-textarea-inner .channel-textarea-upload{
border: 0;
}
.guild-header header{
box-shadow: none;
}
.avatar-wrapper {
background: rgba(0, 0, 0, 0) !important
}
.popout .user-popout .body,
.popout .user-popout .footer {
background-color: rgba(42, 42, 42, 0.8) !important;
border: 0 !important;
}
.header::after{
background-size: 0 0;
}
.theme-dark .themed-popout .header,
.theme-dark .themed-popout{
border-radius: 0;
border: 0 !important;
box-shadow: 0 0;
}
.theme-dark .themed-popout .header{
background-color: rgba(0, 0, 0, 0.5);
}
.theme-dark .themed-popout{
background-color: rgba(42, 42, 42, 0.8);
}
.theme-dark .messages-popout-wrap .messages-popout .message-group{
background-color: rgba(0, 0, 0, 0.5);
border-radius: 0;
border: 0 !important;
box-shadow: 0 0;
}
.theme-dark .messages-popout-wrap .messages-popout .channel-separator .channel-name{
color: rgba(255, 255, 255, 0.8);
}
.messages-popout .message-group .action-buttons{
background-color: rgba(42, 42, 42, 0) !important;
background-size: 0 0;
box-shadow: none !important;
}
.messages-popout .message-group .action-buttons:hover{
background-color: rgba(255, 255, 255, 0.2) !important;
}
.theme-dark .themed-popout .text{
color: rgba(255, 255, 255, 0.8);
}
.search-popout{
margin-top: 0 !important;
background-color: rgba(0, 0, 0, 0);
}
.results-group{
margin-top: 0 !important;
}
div.search{
background-color: rgba(0, 0, 0, 0.3);
}
div.search-bar{
border-radius: 0 !important;
}
.option strong,
span.displayed-nick,
span.answer{
color: rgba(197, 207, 237, 1) !important;
}
span.username{
color: rgba(197, 207, 237, 1);
}
.search-popout{
border-radius: 0;
}
span.filter{
color: rgba(179, 224, 255, 1) !important;
}
span.discriminator{
color: rgba(135, 144, 156, 1);
}
.messages-wrapper .new-messages-bar {
background: rgba(114, 137, 218, 0.5) !important;
border-radius: 0;
}
.theme-dark .messages-wrapper .messages .divider:not(.red) span{
background-color: rgba(0, 0, 0, 0);
color: rgba(255, 255, 255, 0.5);
border-radius: 0 !important;
}
.chat .divider.divider-red{
background-color: rgba(0, 0, 0, 0) !important;
z-index: 1 !important;
}
.theme-dark .friends-table .messages .divider.divider-red>div{
background-color: rgba(0, 0, 0, 0) !important;
}
.theme-dark .messages-wrapper .messages .divider.divider-red>div{
background-color: rgba(240, 71, 71, 0) !important;
}
.theme-dark .messages-wrapper .messages .divider:before{
background-color: #eceeef !important;
opacity: 0.05;
}
.theme-dark .messages-wrapper .messages .divider.divider-red>span{
background-color: rgba(240, 71, 71, 0.35) !important;
color: rgb(240, 71, 71);
z-index: 1 !important;
}
.emoji-picker .header{
background-color: rgba(0, 0, 0, 0.3);
border: 0 !important;
}
div.emoji-picker{
background-color: rgba(42, 42, 42, 0.8);
border: 0 !important;
border-radius: 0 !important;
}
.emoji-picker .scroller .emoji-item.selected{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
input.emoji-name.input{
background-color: rgba(255, 255, 255, 0.2) !important;
color: rgba(255, 255, 255, 0.8);
}
.guild-settings-modal-emoji .emoji-uploader .emoji-uploader-username{
color: rgba(255, 255, 255, 0.8);
}
.deprecated-settings-modal .settings-inner{
background-color: rgba(42, 42, 42, 0.8);
}
.deprecated-settings-modal .settings-actions{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
border: none;
}
.notification-settings-modal.deprecated-settings-modal .settings-actions{
border-radius: 0;
}
.notification-settings-modal.deprecated-settings-modal .settings-inner:first-child{
border-radius: 0;
}
div.search-header,
div.search-results-wrap{
background-color: rgba(0, 0, 0, 0.2) !important;
}
span.channel-name{
background-color: rgba(0, 0, 0, 0.0) !important;
}
.theme-dark .search .search-bar{
background-color: rgba(0, 0, 0, 0.5);
}
.theme-dark .search-popout{
box-shadow: none !important;
}
.search-popout .option .non-text{
color: rgba(255, 255, 255, 0.9);
}
.search-popout .search-query{
background-color: rgba(0, 0, 0, 0.5);
border: 0;
}
.search-popout .results-group:before{
border: 0;
}
.theme-dark .theme-light .ui-calendar-picker .react-datepicker,
.theme-light .ui-calendar-picker .react-datepicker{
background-color: rgba(0, 0, 0, 0.25);
}
.theme-dark .theme-light .ui-calendar-picker .react-datepicker__header,
.theme-light .ui-calendar-picker .react-datepicker__header{
background-color: rgba(0, 0, 0, 0);
}
.search-popout .date-picker{
background-color: rgba(0, 0, 0, 0.25);
border: 0;
}
.theme-dark .theme-light .ui-calendar-picker .react-datepicker__current-month,
.theme-light .ui-calendar-picker .react-datepicker__current-month{
background-color: rgba(0, 0, 0, 0) !important;
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .theme-light .ui-calendar-picker .react-datepicker__week .react-datepicker__day:last-of-type,
.theme-light .ui-calendar-picker .react-datepicker__week .react-datepicker__day:last-of-type,
.theme-dark .theme-light .ui-calendar-picker .react-datepicker__day,
.theme-light .ui-calendar-picker .react-datepicker__day,
.theme-dark .theme-light .ui-calendar-picker .react-datepicker__day-name,
.theme-light .ui-calendar-picker .react-datepicker__day-name{
color: rgba(255, 255, 255, 0.9);
}
.react-datepicker{
border-radius: 0;
background-color: rgba(42, 42, 42, 0);
color: rgba(255, 255, 255, 0.8);
}
.react-datepicker .react-datepicker__header{
background-color:rgba(0, 0, 0, 0);
}
.react-datepicker .react-datepicker__day--disabled,
.react-datepicker .react-datepicker__day--outside-month
{
background-color: rgba(255, 255, 255, 0.1) !important;
color: rgba(255, 255, 255, 0.42) !important;
}
.react-datepicker__day{
border-color: rgba(255, 255, 255, 0.2);
}
.react-datepicker .react-datepicker__current-month{
color: rgba(255, 255, 255, 0.8);
}
.react-datepicker .react-datepicker__day-name{
color: rgba(255, 255, 255, 0.5);
}
.react-datepicker .react-datepicker__day{
border: 0;
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
}
.search-popout .date-picker .date-picker-hint{
background-color: rgba(42, 42, 42, 0);
border: 0;
border-radius: 0;
}
.react-datepicker .react-datepicker__navigation.react-datepicker__navigation--next,
.react-datepicker .react-datepicker__navigation.react-datepicker__navigation--previous{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
border: 0;
}
.react-datepicker .react-datepicker__month>.react-datepicker__week:first-of-type>.react-datepicker__day:first-of-type,
.react-datepicker .react-datepicker__month>.react-datepicker__week:last-of-type>.react-datepicker__day:first-of-type,
.react-datepicker .react-datepicker__month>.react-datepicker__week:last-of-type>.react-datepicker__day:last-of-type,
.react-datepicker .react-datepicker__month>.react-datepicker__week:first-of-type>.react-datepicker__day:last-of-type{
border-radius: 0;
}
.react-datepicker .react-datepicker__month .react-datepicker__week>.react-datepicker__day:last-of-type,
.react-datepicker .react-datepicker__month>.react-datepicker__week:last-of-type .react-datepicker__day{
border: 0;
}
.react-datepicker .react-datepicker__day.react-datepicker__day--disabled,
.react-datepicker .react-datepicker__day.react-datepicker__day--disabled:hover{
color: rgba(255, 255, 255, 0.42);
}
.search-popout .date-picker .date-picker-hint .hint-value{
color: rgba(255, 255, 255, 0.9);
border-radius: 0;
}
.react-datepicker .react-datepicker__day.react-datepicker__day--selected:hover,
.react-datepicker .react-datepicker__day:hover{
background-color: rgba(255, 255, 255, 0.3);
}
.react-datepicker .react-datepicker__day.react-datepicker__day--today:after{
background-color: rgba(255, 255, 255, 0.5);
}
span.search-filter,
span.search-answer,
div.jump-button{
background-color: rgba(255, 255, 255, 0.2) !important;
color: rgba(255, 255, 255, 0.9);
border-radius: 0;
}
.messages-popout .message-group .action-buttons .jump-button{
background-color: rgba(0, 0, 0, 0) !important;
}
div.option.selected{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.42) !important;
}
div.results-group{
background-color: rgba(0, 0, 0, 0.5) !important;
border-radius: 0 !important;
border: 0;
box-shadow: none !important;
}
.theme-dark .search-results-wrap .scroller-wrap .scroller::-webkit-scrollbar-thumb{
background-color: rgba(0, 0, 0, 0.42) !important;
border: none !important;
}
.theme-dark .search-results-wrap .scroller-wrap .scroller::-webkit-scrollbar-track-piece,
.scroller-wrap .scroller::-webkit-scrollbar-track-piece{
background: rgba(0, 0, 0, 0) !important;
}
.theme-dark .search-results-wrap .search-header .total-results{
color: rgba(255, 255, 255, 0.8);
opacity: 1 !important;
}
.theme-dark .search-results-wrap .search-header .tab.selected{
color: rgba(255, 255, 255, 0.8);
border-color: rgba(255, 255, 255, 0.8);
}
span.search-answer{
margin-left: 0;
}
.hide-overflow{
overflow: hidden !important;
}
.theme-dark .search-results-wrap .search-result .search-result-message.hit,
.message-group .sink-interactions.clickable{
border-radius: 0 !important;
}
div.option::after,
div.option.selected::after,
div.option.user::after,
div.option.user.selected::after,
div.option.search-option.selected::after,
div.option.search-option::after,
div.option.history::after,
div.option.history.selected::after
{
background-size: 0 0 !important;
}
div.popout.popout-bottom.no-shadow.search-popout{
background-color: rgba(42, 42, 42, 0.5) !important;
}
div.search-result-message.hit{
background-color: rgba(0, 0, 0, 0.42) !important;
box-shadow: 0 0 !important;
border: 0 !important;
}
div.search-result.expanded{
border: 0 !important;
}
div.search-result::before,
div.search-result::after
{
background-size: 0 0;
}
button.btn-stroked{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border: 0;
border-radius: 0;
}
.btn-filled.white{
border-radius: 0;
}
.premium-settings .subscription,
.premium-settings .payment-method .payment-info .card-tools button,
.premium-settings .premium-header .premium-options button,
.premium-settings .subscription,
.premium-settings .subscription .premium-tools button,
.premium-payment-modal,
.premium-payment-modal .premium-animation>svg,
.premium-payment-modal .premium-payment-form,
.premium-payment-modal .premium-payment-button,
.premium-settings .payment-method .payment-info .card-tools .ui-button,
.fancy-credit-input{
border-radius: 0;
}
.ui-form-title.h2,
.premium-settings .billing-history-list li .date,
.premium-settings .billing-history-list li .description,
.premium-settings .billing-history-list li .payment-details{
color: rgba(255, 255, 255, 0.9);
}
.premium-settings .premium-header{
border-color: rgba(255, 255, 255, 0.2);
}
.premium-settings .premium-header .premium-options button.btn-clear{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
}
.premium-settings .premium-header .premium-options button.btn-clear:hover{
background-color: rgba(255, 255, 255, 0.42);
}
.premium-settings .premium-header .premium-options button.btn-clear strong{
color: rgba(255, 255, 255, 0.9);
}
div.card-description,
div.card-details,
.premium-settings .payment-method .payment-info .card-info .card-description strong,
li.completed,
span.amount {
color: rgba(255, 255, 255, 0.8) !important;
}
.premium-settings .payment-subhead,
.premium-settings .billing-history .payment-subhead{
color: rgba(255, 255, 255, 0.3);
}
.alert.form.premium-unsubscribe strong,
.alert.form.premium-upgrade strong{
color: rgba(197, 207, 237, 1);
}
.quickswitcher.dark{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
box-shadow: none;
}
.qs-tutorial-messages .qs-search-message{
opacity: 0.9;
}
.quickswitcher.dark .big-input{
color: rgba(255, 255, 255, 0.9);
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
box-shadow: none;
}
.quickswitcher.dark .scroller-wrap:before{
background: 0 #7289da;
height: 5px;
}
.quickswitcher .result .result-display-name,
.quickswitcher .result .result-username{
opacity: 1;
}
.quickswitcher.dark .result>div .result-match,
.quickswitcher.dark .result>div .result-type-icon{
opacity: 0.9;
}
.quickswitcher .result .result-display-name{
opacity: 1;
color: rgba(197, 207, 237, 1);
}
.quickswitcher .result .result-username{
opacity: 1;
color: rgba(197, 207, 237, 0.4);
}
.quickswitcher .result{
border-radius: 0;
}
.quickswitcher.dark .result.selected{
background-color: rgba(255, 255, 255, 0.2);
}
.quickswitcher.dark .result.selected:after{
box-shadow: none;
background-color: rgba(255, 255, 255, 0);
}
.quickswitcher.dark .result>div.unread .result-match,
.quickswitcher.dark .result>div.unread .result-type-icon{
opacity: 0.9;
}
.ui-card{
border: none;
}
.ui-selectable-item{
border-radius: 0;
}
.ui-search-bar{
background-color: rgba(0, 0, 0, 0.5) !important;
border-radius: 0;
}
.ui-search-bar .input{
border-radius: 0;
}
.ui-popout-list{
border-radius: 0;
}
.dark-elevation-border-high, .theme-dark .elevation-border-high{
background-color: rgba(42, 42, 42, 0.8);
box-shadow: none;
}
.theme-dark .ui-standard-sidebar-view .btn-close{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .ui-standard-sidebar-view .btn-close:hover{
background-color: rgba(255, 255, 255, 0.2);
}
.ui-tab-bar.SIDE .ui-tab-bar-item,
.ui-card,
.ui-button,
.ui-radiogroup .ui-card,
.ui-checkbox-wrapper .ui-checkbox,
.ui-standard-sidebar-view .btn-close,
.user-settings-keybinds .ghost-pill,
.user-settings-games .not-detected,
.user-settings-games .now-playing,
.ui-hover-card:before{
border-radius: 0;
border: none;
}
.ui-radiogroup .radio-item{
border-radius: 0;
}
.theme-dark .ui-standard-sidebar-view{
background: 0 0;
}
.theme-dark .ui-card-primary{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .ui-card-primary:not(.editable):not(.outline) .ui-form-text{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .ui-card-primary.editable{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .ui-card-primary.editable:hover{
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .ui-card-primary .ui-form-title.h5{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .ui-radiogroup .desc{
color: rgba(255, 255, 255, 0.7);
}
.theme-dark .ui-standard-sidebar-view .sidebar-region,
.theme-dark .ui-standard-sidebar-view .sidebar-region .scrollbar{
background-color: rgba(0, 0, 0, 0.42);
}
.theme-dark .ui-standard-sidebar-view .content-region,
.theme-dark .ui-standard-sidebar-view .content-region .scrollbar{
background-color: rgba(0, 0, 0, 0.55);
}
.theme-dark .ui-hover-card:before{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .ui-modal,
.theme-dark .ui-modal-content{
background-color: rgba(42, 42, 42, 0.42);
border-radius: 0;
}
.theme-dark .ui-modal-footer{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
box-shadow: none;
}
.ui-select .Select-menu{
border-radius: 0;
}
.theme-dark .ui-select .Select-option:hover{
background-color: rgba(84, 84, 84, 0.8) !important;
}
.theme-dark .ui-select .Select-option{
background-color: rgba(42, 42, 42, 0.8) !important;
}
.theme-dark .ui-select .Select-control{
border-radius: 0;
background-color: rgba(0, 0, 0, 0.3);
}
.Select-option:last-child{
border-radius: 0;
}
.theme-dark .ui-select .Select-menu-outer{
background-color: rgba(42, 42, 42, 0);
box-shadow: none;
}
.theme-dark .ui-select .Select-option.is-selected{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.theme-dark .ui-select .Select-option.is-selected:hover{
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .ui-selectable-item:hover{
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .ui-audit-log{
background-color: rgba(255, 255, 255, 0.1);
border: none;
}
.ui-audit-log{
border-radius: 0;
}
.theme-dark .ui-audit-log{
color: rgba(255, 255, 255, 0.7)
}
.theme-dark .ui-audit-log .user-hook .discrim{
opacity: 0.9;
}
.theme-dark .ui-audit-log strong{
color: rgba(197, 207, 237, 1);
}
.theme-dark .ui-audit-log .timestamp{
color: rgba(255, 255, 255, 0.6);
}
.dark-elevation-border-low, .theme-dark .elevation-border-low{
background-color: rgba(42, 42, 42, 0.8);
border: none;
}
.ui-color-picker-swatch.custom,
.ui-color-picker-swatch.default,
.ui-color-picker-swatch{
border-radius: 0;
}
.theme-dark .ui-form-title.h5{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .ui-form-text.style-description, .theme-dark .ui-form-text.style-label-descriptor{
color: rgba(255, 255, 255, 0.6);
}
.ui-role-list-add{
border-radius: 0;
}
.ui-role-list-role{
border-radius: 0;
}
.roles-list-popout{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.ui-flex.flex-horizontal>.ui-flex{
margin-right: 0;
}
.ui-text-input .input{
border-radius: 0;
border: none;
}
.theme-dark .ui-text-input .input,
.theme-dark .ui-text-input .input.editable:focus,
.theme-dark .ui-text-input .input.editable:hover {
background-color: rgba(0, 0, 0, 0.5);
}
.ui-button.white.outlined{
background-color: rgba(255, 255, 255, 0.1);
border: none;
}
.ui-input-button{
border-radius: 0;
border: none;
}
.ui-input-button .ui-input-button-ui-button{
border-radius: 0;
}
.theme-dark .ui-input-button{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .ui-button.grey.ghost{
background-color: rgba(255, 255, 255, 0.1);
border-radius: 0;
}
.theme-dark .ui-text-input.emoji-alias-input .input{
background-color: rgba(0, 0, 0, 0.5);
}
.theme-dark .ui-card.outline{
background-color: rgba(255, 255, 255, 0.1);
}
.ui-settings-notice{
border-radius: 0;
}
.ui-role-list .ui-role-list-role{
border-radius: 0;
}
.user-settings-connections .connection{
border-radius: 0;
}
.user-settings-connections .connection-header{
border: none;
border-radius: 0;
}
.theme-dark .user-settings-notifications .notifications-sound{
box-shadow: inset 0 -1px 0 0 rgba(255, 255, 255, 0.2);
}
.connection-delete{
border-radius: 0;
}
.round-remove-button{
top: 0 !important;
right: -44px !important;
background-color: rgba(255, 255, 255, 0.2) !important;
box-shadow: none !important;
border-radius: 0;
}
.mfa-modal .mfa-step{
border:none;
}
.theme-dark .user-settings-games .game {
box-shadow: 0 1px 0 0 rgba(255, 255, 255, 0.2) !important;
}
.theme-dark .user-settings-games .game-name-input:focus,
.theme-dark .user-settings-games .game-name-input:hover{
background-color: rgba(255, 255, 255, 0.2);
border: none;
border-radius: 0;
}
.theme-dark .user-settings-games .last-played,
.theme-dark .user-settings-games .overlay-status-text{
color: rgba(255, 255, 255, 0.42);
}
.content-2mSKOj{
border-radius: 0;
}
.contentSelectedText-3j5CXt{
background-color: rgba(0, 0, 0, 0.5);
}
.content-2mSKOj:hover{
background-color: rgba(0, 0, 0, 0.25);
}
.container-RYiLUQ,
.private-channels .channel.selected a{
background-color: rgba(0, 0, 0, 0) !important;
}
.private-channels .channel:hover a {
background-color: rgba(0, 0, 0, 0);
}
.contentHoveredText-2HYGIY,
.contentHoveredVoice-3qGNKh:active,
.contentSelectedVoice-gTtYM9:active{
background-color: rgba(0, 0, 0, 0);
}
.container-3lnMWU{
background-color: rgba(0, 0, 0, 0.5);
border-bottom: none;
}
.wrapper-2xO9RX{
border-radius: 0;
box-shadow: none;
text-shadow: none;
}
.wrapper-2ldvyE{
background-color: rgba(0, 0, 0, 0.5);
border-radius: 0;
}
.card-3DrRmC{
border: none;
border-radius: 0;
}
.theme-dark .cardPrimary-ZVL9Jr{
background-color: rgba(255, 255, 255, 0.1);
}
.buttonOutlined-38aLSW{
border-radius: 0;
}
.button-2t3of8{
border-radius: 0;
}
.light-elevation-border-high,
.theme-light .elevation-border-high{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
box-shadow: none;
}
.ui-new-terms-modal .button-container{
background-color: rgba(42, 42, 42, 0.8);
border: none;
}
.theme-light .primary-2giqSn{
color: rgba(255, 255, 255, 0.9);
}
.ui-new-terms-modal .ack{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .modal-3HOjGZ{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
box-shadow: none;
}
.input-2YozMi{
border-radius: 0;
border: none;
}
.theme-dark .input-2YozMi{
background-color: rgba(0, 0, 0, 0.3);
}
.theme-dark .message-25xg43{
border-radius: 0;
box-shadow: none;
}
.checkboxBox-2i2Ris{
border-radius: 0;
}
.auditLog-1XsYCj{
border-radius: 0;
border: none;
}
.theme-dark .headerClickable-1jGUp8, .theme-dark .headerDefault-1ajMkj{
background-color: rgba(0, 0, 0, 0.3);
}
.theme-dark .headerExpanded-wW1rBx{
background-color: rgba(0, 0, 0, 0.6);
}
.theme-dark .divider-ShvCWe{
background-color: rgba(0, 0, 0, 0.3);
}
.theme-dark .changeDetails-zbf-61{
background-color: rgba(0, 0, 0, 0.3);
}
.theme-dark .copyInputDefault-36NOFa{
background-color: rgba(0, 0, 0, 0.3);
border-radius: 0;
border: none;
}
.buttonGreyGhost-SfY7zU{
background-color: rgba(255, 255, 255, 0.1);
}
.buttonGreyGhost-SfY7zU:hover{
background-color: rgba(255, 255, 255, 0.2);
}
.item-3879bf{
border-radius: 0;
}
.theme-dark .elevationHigh-3lNfp9{
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.theme-dark .bubble-17BwqU:before{
border-top-color: #7289da;
}
.grabber-1TZCZi{
border-radius: 0;
}
.theme-dark .bar-2cFRGz{
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .inner-3if5cm{
background-color: rgba(0, 0, 0, 0.42);
border-radius: 0;
}
.theme-dark .autocomplete-1TnWNR{
background-color: rgba(10, 10, 10, 0.9);
border-radius: 0;
}
.selector-nbyEfM{
border-radius: 0;
}
.theme-dark .selectorSelected-2M0IGv{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .description-YnaVYa{
color: rgba(255, 255, 255, 0.8)
}
.theme-dark .descriptionUsername-1quCGz{
color: rgba(197, 207, 237, 1);
}
.popout{
box-shadow: none;
}
.botTagInvert-gorWR_{
border-radius: 0;
background: rgba(0, 108, 200, 0.5) !important;
color: rgba(255, 255, 255, 0.9) !important;
}
.header-3mZJcV{
padding-top: 15px;
padding-bottom: 15px;
}
.body-3rkFrF{
padding-top: 15px;
padding-bottom: 15px;
}
.footer-2J5zqP{
padding-top: 0;
padding-bottom: 15px;
}
.endBodySection-1WYzxu{
margin-bottom: 15px;
}
.protip.inline{
padding-top: 10px;
}
.item-3H-QZD:first-child,
.item-3H-QZD:last-child,
.item-3H-QZD{
border-radius: 0;
border: none;
}
.theme-dark .item-3H-QZD {
background-color: rgba(255, 255, 255, 0.1);
}
.denySelected-h37B9e{
background: #f04747 !important;
}
.theme-dark .passthroughSelected-3_g4oB{
background: #747f8d !important;
}
.allowSelected-1FAg8y{
background: #43b581 !important;
}
.prefix-dCECsB,
.wrapper-2ldvyE{
font-family: "MS UI Gothic", Whitney, Helvetica Neue, Helvetica, Arial, sans-serif;
}
.theme-dark .headerExpanded-wW1rBx{
color: rgba(255, 255, 255, 0.7) !important;
}
.theme-dark .userHook-DFT5u7{
color: rgba(197, 207, 237, 1);
}
.theme-dark .footer-1PYmcw{
background: rgba(0, 0, 0, 0.42) !important;
border-radius: 0;
box-shadow: none;
border: none;
}
.form.deprecated .has-value .Select-placeholder{
color: rgba(255, 255, 255, 0.8);
}
.form.deprecated .btn-default,
.form.deprecated .btn-default:hover{
border: none;
}
.round-30vw42{
border-radius: 0;
}
.theme-dark .checkbox-1QwaS4{
border: none;
}
.roundRemoveButton-1NEXB9{
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2);
box-shadow: none;
}
.form.deprecated .Select-option{
color: rgba(255, 255, 255, 0.8);
}
.form.deprecated .Select-option.is-focused{
background-color: rgba(255, 255, 255, 0.1);
color: rgba(255, 255, 255, 0.8);
}
.form.deprecated .Select-option.is-focused:hover{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
}
.form.deprecated .Select-option:hover{
background-color: rgba(255, 255, 255, 0.1);
}
.checkboxWrapper-2Yvr_Y{
background-color: rgba(255, 255, 255, 0.2);
}
.checkboxWrapper-2Yvr_Y:hover{
background-color: rgba(255, 255, 255, 0.3);
}
.box-XhjOl4{
border-radius: 0;
}
.theme-dark .ui-video{
background: none;
}
.theme-dark .private-channel-call{
background: none;
}
.ui-call-avatar.video{
border-radius: none;
}
.headerLive-2dDMvp{
border: none;
margin-bottom: -15px;
}
.bodyDivider-3OPnU2{
background: none;
}
.nameSmall-2HcWNX{
color: rgba(255, 255, 255, 0.7);
}
.contentSmall-3Or8WV{
color: rgba(255, 255, 255, 0.6);
}
.assetsLargeImage-3apSRO{
border-radius: 0;
}
.form.deprecated .form-inner{
background: none;
}
.theme-dark .quickswitcher-2NdiGJ{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.theme-dark .tipsWithoutResults-202oQR,
.theme-dark .tipsWithResults-3TVZGE{
background-color: rgba(0, 0, 0, 0.42);
margin: 0 -21px -1px -21px;
padding-left: 21px;
padding-right: 21px;
border: none;
color: rgba(255, 255, 255, 0.5);
}
.theme-dark .input-MwQhcX{
background-color: rgba(0, 0, 0, 0.5);
border-radius: 0;
box-shadow: none;
color: rgba(255, 255, 255, 0.9);
}
.match-2k4Voy{
color: rgba(197, 207, 237, 1);
}
.theme-dark .cardPrimaryEditable-2IQ7-V{
background-color: rgba(255, 255, 255, 0.1);
}
.theme-dark .descChecked-KbaI-r,
.theme-dark .titleChecked-3Ngoss {
color: rgba(255, 255, 255, 1) !important;
}
.theme-dark .h5-3KssQU,
.text-align-right{
color: rgba(255, 255, 255, 0.85);
}
.overflow-ellipsis,
.invite-settings-invite-row .channel-name{
opacity: 1 !important;
}
.theme-dark .title-3i-5G_{
color: rgba(255, 255, 255, 0.7);
}
.theme-dark .text-1rLRsh,
.theme-dark .title-38OOBL,
.theme-dark .description-3MVziF,
.theme-dark .labelDescriptor-1BebCl,
.theme-dark .desc-2dKaro,
.invite-settings-invite-row .channel-name{
color: rgba(255, 255, 255, 0.5);
}
.theme-dark .discrim-xHdOK3,
.invite-settings-invite-row .countdown-never{
color: rgba(255, 255, 255, 0.5);
opacity: 1 !important;
}
.theme-dark .timestamp-5LpvaA{
color: rgba(255, 255, 255, 0.3);
}
.theme-dark .emoji-alias-input .emoji-input{
background-color: rgba(255, 255, 255, 0.2);
}
.bar-Y-RLyN{
opacity: 0.8;
}
.bodyTitle-yehI7c{
margin-bottom: 3px;
}
.endBodySection-1WYzxu{
margin-bottom: 8px;
}
.protip.inline{
padding-top: 0;
}
.headerTagNormal-KyD3_J,
.headerActivityText-3qBQRo{
margin-bottom: 0;
}
.theme_dark-2FtE3l{
background: none;
background-color: rgba(0, 0, 0, 0.77);
}
.theme-dark .container-a2vS7i,
.theme-dark .reactors-2PjMP0,
.theme-dark .sidebar-32BRdp{
background-color: rgba(22, 22, 22, 0.8);
}
.scroller-2IVcoQ{
background-color: rgba(42, 42, 42, 0.8);
}
.reactionDefault-2V6kdV,
.reactionSelected-rLBoT_{
border-radius: 0;
}
.container-2OU7Cz{
background-color: rgba(0, 0, 0, 0);
}
.appMount-14L89u{
background: none;
}
.typeWindows-15E0Ys{
background-color: rgba(0, 0, 0, 0.9);
margin-top: 0;
padding-top: 4px;
}
.private-channels .search-bar{
box-shadow: none;
padding-bottom: 1px;
}
.theme-dark .chat form{
background-color: rgba(0, 0, 0, 0);
box-shadow: none;
}
/****************************************************************/
/****************************************************************/
/*BD Stuff*/
#bd-pane .scroller-wrap div[style*="background:#2E3136; color:#ADADAD; height:30px; position:absolute; bottom:0; left:0; right:0;"] {
background: rgba(0,57,57,0.4) !important;
}
#bd-pane > div > div > div.bd-settings > div:nth-child(6) > span:nth-child(1) {
color: #006969;
}
/****************************************************************/
/****************************************************************/
/*Buttons*/
.invite-button{
background-color: rgba(0, 0, 0, 0.5);
border: 0;
border-radius: 0;
}
.invite-button.can-click{
border-radius: 0;
background-color: rgba(0, 0, 0, 0.5);
border: none;
}
.invite-button .invite-button-body,
.invite-button .invite-button-header{
color: rgba(255, 255, 255, 0.8);
}
.invite-button-body{
color: #99aab5 !important;
}
.invite-btn {
background-color: rgba(0, 204, 204, 0.5);
}
.btn-group {
border: 0px solid rgba(0,0,0,0) !important;
}
.btn-mute,
.btn-account,
.account .btn-deafen,
.account .btn-mute {
border-right: 0px;
}
.account .btn-deafen, .account .btn-settings {
box-shadow: inset 0px 0 0 #373b42;
}
#voice-connection .btn-info {
border-right: 0px;
}
#voice-connection .btn-disconnect {
box-shadow: inset 0px 0 0 #373b42;
}
.account {
border-top: 1px solid rgba(0,0,0,0);
}
.account .btn-settings:after {
opacity: 0.3;
}
div.new-messages-bar button {
margin-top: 10px;
background-color: rgba(0,57,57,0.2);
color: rgba(244,244,244,1);
}
.jump-to-present-bar button {
background-color: rgba(0,57,57,0.8) !important;
color: rgba(244,244,244,1) !important;
}
.action-buttons .jump-button {
background: transparent;
background-color: rgba(0, 114, 114, 0.6);
border: 1px solid rgba(0, 0, 0, 0.4);
}
.btn.btn-default {
background-color: rgba(0,57,57,1);
border-radius: 5px;
padding-left: 5px;
padding-right: 5px;
border-bottom: 0px;
}
.form .btn-default:hover {
border-bottom: none;
}
/****************************************************************/
/****************************************************************/
/*Channels: Hover and background*/
.guild-channels .channel-text:hover {
background: linear-gradient(to right, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.0));
}
.channel-members .member.popout-open, .channel-members .member:hover { 
background: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.3) 85%, transparent);
}
.guild-channels ul .channel-text.unread:not(.selected):not(.channel-muted):before {
left: -11px;
}
.guilds-wrapper .guilds .guild.unread, 
.channel.channel-text.unread:not(.channel-muted):not(.selected) {
-webkit-animation: glowpulse 1s infinite alternate;
animation: glowpulse 1s infinite alternate;
} 
.channel:not(.selected) {
transition: background 1s ease-out;
}
.channel:not(.selected):hover {
background: rgba(0, 0, 0, 0.0);
transition: background 1s ease-in;
}
.guild-channels .channel-text.selected,
.guild-channels .channel-text:hover {
background: -webkit-linear-gradient(left,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: rgba(0,0,0,0.2);
}
.channel-members {
z-index:2;
transition:all 400ms ease;
background-color: rgba(0, 0, 0, 0) !important;
}
.channel-members:hover {
transition:all 400ms ease;
background-color: rgba(0, 0, 0, 0.4) !important;
}
.channel-members .member:hover {
background: linear-gradient(90deg,rgba(0,0,0,4) ,rgba(0,0,0,0)) !important;
background-color: rgba(0, 0, 0, 0.2);
}
.channel-members:hover .member .member-activity, .channel-members:hover .member .member-username-inner{
opacity:1;
}
.channel-members .member.popout-open {
background: -webkit-linear-gradient(left,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: rgba(0,0,0,0.2) !important;
transition:all 400ms ease;
}
.channel-members .member .member-activity,
.channel-members .member .member-username-inner {
opacity:0;
transition:opacity 400ms ease, margin 100ms ease;   
}
.channel.selected.private,
.channel.channel-text.selected {
background: linear-gradient(to right,rgba(0, 0, 0, 0.4),rgba(0, 0, 0, 0));
}
.channels .channel-text.selected:before,
.guild-channels .channel-text.selected:hover:before,
.guild-channels .channel-text:hover.channel-muted:before,
.guild-channels .channel-text:hover:not(.unread):before,
.private-channels .channel.selected:before,
.private-channels .channel:hover:before {
border-left: 3px solid #00D1D1;
opacity: .25;
}
.chat .flex-vertical .flex-spacer .private >.content.flex-spacer.flex-horizontal>.flex-spacer.flex-vertical,
.chat.flex-vertical.flex-spacer.private>.content.flex-spacer.flex-horizontal>.flex-spacer.flex-vertical,
.chat.flex-vertical.flex-spacer>.content.flex-spacer.flex-horizontal>.flex-spacer.flex-vertical {
margin-right: -15px;
z-index:1
}
/****************************************************************/
/****************************************************************/
/*Chat*/
.chat .has-more button {
color:#00bbbb;
background:rgba(0,117,117,0.8);
border:none;
box-shadow:none;
}
.option-popout.small-popout-box {
background: linear-gradient(to right, rgba(0, 114, 114, 0.5), rgba(0, 57, 57, 1));
}
.option-popout.small-popout-box .btn-item{
background: linear-gradient(to right, rgba(0, 114, 114, 0.5), rgba(0, 114, 114, 1));
}
.inline {
background-color: rgba(0, 0, 0, 0.4);
border-radius: 5px;
font-size: 12px;
line-height: 22px;
}
.message-group h2 strong{
color: rgba(255, 255, 255, 0.95);
}
.message-group .comment .markup{
color: rgba(255, 255, 255, 0.7);
}

.theme-dark .message-group .embed{
background-color: rgba(10, 10, 10, 0.5);
border-radius: 0;
border: 0;
}
.message-group .mentioned .message-text:after{
border-radius: 0;
}
.theme-dark .reaction{
background-color: rgba(10, 10, 10, 0.3);
border-radius: 0;
}
.message-reactions-modal{
background: rgba(255, 255, 0, 0);
box-shadow: none;
}
.message-reactions-modal .message-reactions-list .scroller-wrap{
background-color: rgba(0, 0, 0, 0.3);
border-radius: 0;
}
.message-reactions-modal .message-reactions-list-inner{
background-color: rgba(0, 0, 0 ,0);
}
.message-reactions-modal .message-reactions-reactors{
background-color: rgba(42, 42, 42, 0.8);
}
.message-reactions-modal .message-reactions-reactors .reactor{
box-shadow: none;
}
.message-reactions-modal .message-reactions-list-inner .reaction.selected{
background-color: rgba(255, 255, 255, 0.2);
}
.message-reactions-modal .message-reactions-list-inner .reaction.selected:hover{
background-color: rgba(255, 255, 255, 0.25) !important;
}
.message-reactions-modal .message-reactions-list-inner .reaction{
background-color: rgba(255, 255, 255, 0.1);
border-radius: 0;
}
.message-reactions-modal .message-reactions-list-inner .reaction:hover{
background-color: rgba(255, 255, 255, 0.15) !important;
}
.message-reactions-modal .message-reactions-list-inner .reaction .count{
color: rgba(255, 255, 255, 0.9);
}
.message-reactions-modal .message-reactions-reactors .reactor .name{
color: rgba(197, 207, 237, 1);
}
.theme-dark .channel-textarea-autocomplete-inner header{
border: 0;
background-color: rgba(0, 0, 0, 0.5);
}
.channel-textarea-autocomplete-inner header strong{
color: rgba(255, 255, 255, 0.8);
}
.theme-dark .channel-textarea-autocomplete-inner{
border: 0;
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.theme-dark .channel-textarea-autocomplete-inner ul li.active{
background-color: rgba(255, 255, 255, 0.2);
}
.theme-dark .channel-textarea-autocomplete-inner:after{
border: 0;
}
.channel-textarea-autocomplete-inner:after{
border: 0;
}
.channel-textarea-guard .countdown .countdown-number{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
border: none;
}
.theme-dark .messages-wrapper .messages .message-group-blocked .message-group-blocked-btn{
display:none;
}
.theme-dark .messages-wrapper .messages .message-group-blocked{
border: none;
background: none;
}
div.message-group-blocked{
border-bottom: 1px solid hsla(0,0%,100%,.04) !important;
margin-top: 0;
margin-bottom: 0;
}
.divider+.message-group-blocked,
.empty-message+.message-group-blocked{
margin: 0;
display: none;
}

.message-group .avatar-large {
    border-color: rgba(0,0,0,0.5) !important;
    border-width: 9px !important;
    border: solid;
    width: 50px;
    height: 50px;
    background-repeat: no-repeat !important;
    background-size: 100%;
    background-color: transparent !important;
    position: relative;
    top: -10px;
    left: -5px;
    box-shadow: none;
    background-clip: content-box;
}
.message-group .avatar-large:hover {
    opacity: 1;
}
.message-group .comment {
    padding: 20px;
    padding-left: 50px;
    padding-right: 0px;
    border: none;
    border-radius: 16px;
    border-top-left-radius: 0px;
    border-color: rgba(255,255,255,0);
    margin: 0px 5px 0px -60px;
    background-color: rgba(255,255,255,0.1);
    /*background: radial-gradient(circle at -3px 15px, rgba(0,0,0,0) 47px, rgba(255,255,255,0.1) 15px);*/
}

.edit-container-outer .avatar-large{
    opacity: 0;
    transition: opacity 0s;
    display: none;
}
.innerNoAutocomplete-kaUXJZ {
    margin-left: 60px;
    margin-right: 40px;
}
.edit-container-inner .old-h2 .timestamp{
    padding-left: 60px;
}
.edit-container-inner .old-h2 .user-name {
    display: none;
}

.chat .divider:not(.divider-red) {
    margin-bottom: 10px;
}
.message-group {
    margin-bottom: -15px;
    border: none;
}
.chat .divider {
    margin-top: 20px;
}
.chat .divider > div{
    flex: 0;
}
.chat .divider.divider-red > div{
    flex: 0;
}
.divider.divider-red span {
    background-color: rgba(255,255,255,0.1) !important;
}
.divider.divider-red::before {
    display: none;
}
.divider span {
    background-color: rgba(255,255,255,0.1) !important;
}
.divider::before {
    display: none;
}
/****************************************************************/
/****************************************************************/
/*Chat Input Inner*/
.channel-textarea-autocomplete .images img {width: 100%;height: auto;} .channel-textarea-autocomplete-inner ul li {max-width: 100%;}
.channel-textarea-autocomplete-inner {
background:rgba(0,0,0,0.5) !important;
}
.channel-textarea-autocomplete-inner header {
background:rgba(0,0,0,0.5) !important;
}
.channel-textarea-inner {
background-color: rgba(0, 0, 0, 0.3) !important;
border-radius: 5px !important;
border: 0px solid rgba(0, 0, 0, 0.0);
-webkit-mask-image: -webkit-linear-gradient(top, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 1) 2%, rgba(0, 0, 0, 1) 68%, rgba(0, 0, 0, 0) 100%);
}
.channel-textarea-autocomplete {
background-color: #00CCCC;
}
.channel-textarea-inner textarea {
padding-left: 10px !important;
color: rgba(0, 204, 204, 0.7);
}
.channel-textarea {
margin-bottom: 2.3vh !important;
margin-top: 10px !important;
}
::-webkit-input-placeholder {
color: rgba(255, 255, 255, 0.6) !important;
}
.channel-textarea-autocomplete-inner .active {
background:rgba(0,0,0,0.84) !important;
}
/****************************************************************/
/****************************************************************/
/*Divider*/
.divider.divider-red span {
background-color: rgba(0, 0, 0, 0.7);
color: #00cccc;
}
.divider.divider-red>div {
background: rgba(0, 204, 204, 0.7);
}
/****************************************************************/
/****************************************************************/
/*Embeds*/
.embed-color-pill { 
background-color: rgba(0, 255, 255, .75) !important;
}
.embed.embed-rich {
border-radius: 5px !important;
border-bottom-left-radius: 0px;
border-top-left-radius: 0px;
}
.embed-video-actions {
width: 175%;
height: 152%;
}
.embed {
border-top-right-radius: 15px;
border-bottom-right-radius: 15px;
}
/****************************************************************/
/****************************************************************/
/*Emoji Menu*/
.bda-dark #bda-qem {
background: transparent;
border: 0px solid rgba(0, 0, 0, .5) !important;
}
.bda-dark #bda-qem button { 
background: rgba(0, 0, 0, .15);
border: 0px solid rgba(0, 0, 0, .5);
box-shadow: transparent;
}
.bda-dark #bda-qem button.active {
background: rgba(0, 0, 0, .5);
}
.bda-dark #bda-qem-favourite-container,
.bda-dark #bda-qem-twitch-container, 
.bda-dark .emoji-picker, 
.bda-dark .emoji-picker .category,
.bda-dark .emoji-picker .header .search-bar {
background: rgba(0, 0, 0, .5);
}
.emoji-picker .sticky-header {
background: rgba(0, 0, 0, .75);
}
/****************************************************************/
/****************************************************************/
/*Friends*/
.friends-table-body {
margin-right: 20px;
}
.friends-table, .messages-wrapper  {
background: rgba(0,0,0,0) !important;
}
#friends .friends-header, .search-bar {
background-color: rgba(0,0,0,0) !important;
}
#friends {
background: linear-gradient(to right, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.0)) !important;
}
#friends .friends-table .friends-row:hover {
background: -webkit-linear-gradient(left,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: linear-gradient(90deg,rgba(0, 0, 0, 0) 85%,rgba(0, 0, 0, 0));
background: rgba(0,0,0,0.2) !important;
}
.friends-table .scroller-wrap ::-webkit-scrollbar-track-piece, .messages-wrapper .scroller-wrap ::-webkit-scrollbar-track-piece {
background-color: rgba(0,0,0,0) !important;
border: none; 
}
.theme-dark .friends-table .scroller-wrap ::-webkit-scrollbar-thumb, .theme-dark .messages-wrapper .scroller-wrap ::-webkit-scrollbar-thumb {
background-color: rgba(0,0,0,0.2);
}
.theme-light .friends-table .scroller-wrap ::-webkit-scrollbar-thumb, .theme-light .messages-wrapper .scroller-wrap ::-webkit-scrollbar-thumb {
background-color: rgba(0,0,0,0.2);
}
.friends-table .scroller-wrap ::-webkit-scrollbar-thumb, .messages-wrapper .scroller-wrap ::-webkit-scrollbar-thumb {
border-color: rgba(0,0,0,0) !important;
}
.friends-header .header-toolbar {
margin-right: -11%;
}
.private-channels .avatar-small .status {
right: -2px;
bottom: -2px
}
/****************************************************************/
/****************************************************************/
/*Guild*/
.guild-inner, .guild { background-color: rgba(0,0,0,0) !important; }
.guild-header ul {
opacity: 0;
transition: transform .5s cubic-bezier(0.18, 0.89, 0.32, 1.28);
}
.guild-header-open ul {
opacity: 1;
transition: transform .5s cubic-bezier(0.18, 0.89, 0.32, 1.28);
}
.guild-header.guild-header-open ul {
-webkit-transform: translateZ(0);
transform: translateZ(0);
border-radius: 5px;
}
.guild-header header {
background-color: rgba(0,0,0,0) !important;
box-shadow: 0 1px 0 rgba(0,0,0,0),inset 0 -1px 0 rgba(0,0,0,0) !important;
}
.guild-separator {
border-top: 2px solid rgba(0, 204, 204, 0.5);
border-right: 1pt solid rgba(0, 204, 204, 0.5);
border-left: 1pt solid rgba(0, 204, 204, 0.5);
border-bottom: 2px solid rgba(0, 204, 204, 0.5);
border-radius: 5px;
}
.guild-separator:after {
background-color: transparent !important;
}
/****************************************************************/
/****************************************************************/
/*Toolbar*/
.header-toolbar button:nth-child(7) {
display: none;
}
.header-toolbar .separator {
visibility: hidden;
}
/****************************************************************/
/****************************************************************/
/*Hide Nitro*/
.tab-bar.SIDE .tab-bar-item:nth-child(3),
.channel-textarea-autocomplete-inner .premium-promo-autocomplete {
display: none;
}
/****************************************************************/
/****************************************************************/
/*Code: HLJS & BD Custom CSS*/
.hljs {
display: block;
font-family: 'Consolas', monospace;
font-size: 10pt;
overflow-x: auto;
background: #1D1F21 !important;
color: #448888 !important;
padding: 0.5em;
border-radius: 5px;
font-size: 14px;
}
.hljs-emphasis { font-style: italic; }
.hljs-strong { font-weight: bold; }
/* HLJS Colors */
/* Keyword */
.hljs-keyword { color: #E061C7; font-weight: bold; }
/* Builtins */
.hljs-built_in { color: #999999; }
/* Literal, Number */
.hljs-literal, .hljs-number { color: #F79768; }
.hljs-selector-id::first-letter, .hljs-number::first-letter { color: #DE8787; }
/* Regex */
.hljs-regexp { color: #B34D4D; }
/* String */
.hljs-string { color: #2497E3; }
/* Subst */
.hljs-subst { color: #F5C747; font-weight: bold; }
/* Symbol */
.hljs-symbol { color: #04AFBF; }
/* Class */
.hljs-class, .hljs-class .hljs-title { color: #E36222; }
/* Class keyword, Function keyword */
.hljs-class .hljs-keyword, .hljs-function .hljs-keyword { color: #50FA7B; }
/* Function */
.hljs-function, .hljs-function .hljs-title { color: #D65656; }
/* Params */
.hljs-params { color: #07CC95; }
/* Comment, Doctag, Meta Keyword, Meta String, Template Tag, Template Variable */
.hljs-comment, .hljs-doctag, .hljs-meta-keyword, .hljs-meta-string,
.hljs-template-tag, .hljs-template-variable { color: #9E9E9E; font-style: italic; }
/* Meta */
.hljs-meta { color: #E36222; font-style: italic; }
/* Tag */
.hljs-tag { color: #49C7F5; }
/* Name Of Tag */
.hljs-name, .hljs-builtin-name { color: #D75A64; }
/* Attr, Variable */
.hljs-attr, .hljs-variable { color: #78D69E; }
/* HLJS Markup, Bullets, Type */
.hljs-bullet, .hljs-type { color: #04AFBF; font-weight: bold; }
/* Code */
.hljs-code { color: #BEBEBE;  }
/* Emphasis */
.hljs-emphasis { font-style: italic; color: #AEAEAE; }
/* Strong */
.hljs-strong { font-weight: bold; }
/* Formula, Link */ 
.hljs-link { color: #DE935F; }
/* Section */
.hljs-section { color: #CC9C0C; font-weight: bold; }
/* Quote */
.hljs-quote { color: #789922; }
/* HLJS CSS, Tag Selector */
.hljs-selector-tag { color: #D75A64; }
/* ID Selector */
.hljs-selector-id { color: #CC3535; font-weight: bold; }
/* Attribute, Psuedo Selector */
.hljs-attribute, .hljs-selector-pseudo { color: #40C762; }
/* Class Selector */
.hljs-selector-class { color: #49C7F5; }
/* Attr Selector */
.hljs-selector-attr { color: #A25AFA; }
/* Diff Addition */
.hljs-addition { color: #80C771; }
/* Diff Deletion */
.hljs-deletion { color: #C24848; }
/* Symbol */
.hljs-symbol { color: #24A9DD; }
/*Sublime*/
.css .hljs-tag { color: #00f; }
.css .hljs-class,
.css .hljs-important { color: #f00; }
.css .hljs-value,
.css .hljs-hexcolor,
.css .hljs-number,
.css .hljs-function { color: rgba(255, 255, 255, 0.8); }
.css .hljs-attribute { color: #8080c0; }
.css .hljs-comment { color: #008000; }
.css .hljs-id,
.css .hljs-at_rule,
.css .hljs-keyword { color: #0080ff; }
.css .hljs-pseudo { color: #ff8000; }
#bd-customcss-detach-container { background-color: rgba(0,114,114,0.3); }
#bd-customcss-detach-editor #bd-customcss-innerpane, #bd-customcss-detach-editor .CodeMirror, .CodeMirror-code { background-color: rgba(7,77,114,0.8) !important; }
.CodeMirror-gutter.CodeMirror-linenumbers { background-color: rgba(7,57,57,0.8); }
#bd-customcss-attach-controls { background-color: rgba(0,114,114,0.3); }
.cm-property { color: white; }
.cm-qualifier { color: orange; }
.cm-keyword { color: red; }
.cm-builtin { color: purple; }
/****************************************************************/
/****************************************************************/
/*IceCold*/
.emotewrapper+.emotewrapper img[alt="IceCold"] { transform: translate3d(-100%,0,0); }
/****************************************************************/
/****************************************************************/
/*Icons*/
.icon-muted { background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-muted.svg'); }
.icon-deafened { background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-deafen.svg'); }
.channel.channel-voice .icon.icon-instant-settings,
.channel.channel-text.selected .icon.icon-settings {
background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-setting.svg');
opacity: 0.8 !important;
}
.channel.channel-voice:hover .icon.icon-instant-settings,
.channel.channel-text:hover .icon.icon-settings {
background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-setting.svg');
opacity: 0.8 !important;
}
.channel.channel-voice .icon.icon-instant-invite,
.channel.channel-text.selected .icon.icon-instant-invite {
background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-instant-invite.svg');
opacity: 0.8 !important;
}
.channel.channel-voice:hover .icon.icon-instant-invite,
.channel.channel-text:hover .icon.icon-instant-invite {
background-image: url('https://ditmcouk.ipage.com/noottech/discord-icons/cyan-firewatch/cyan-instant-invite.svg');
opacity: 0.8 !important;
}
/****************************************************************/
/****************************************************************/
/*Images: Profile & Guilds; */
.guilds-wrapper .guilds .guild .guild-inner,
.avatar-large,
.avatar-small,
.avatar-small.animate,
.avatar-large.animate,
.guilds-error,
.guilds .guilds-add,
.icon-friends,
.avatar-popout {
border-radius: 5px !important;
transition: all 400ms ease !important;
}
.guild:hover {
border-radius: 50px !important;
}
.friends-icon:hover {
background-color: rgba(0,114,114, 1); !important;
}
.guilds-wrapper .guilds .guild .guild-inner:hover,
.avatar-small:hover,
.avatar-small.animate:hover,
.avatar-large:hover,
.avatar-large.animate:hover,
.guilds-error:hover,
.guilds .guilds-add:hover,
.icon-friends:hover,
.avatar-popout:hover {
border-radius: 50px !important;
transition: all 400ms ease !important;
}
.guild-inner:hover {
background-color: rgba(0,100, 200, 1) !important;
}
.scroller.messages .avatar-large{
transform: translateX(5%);
}
.avatar-large, .avatar-profile, .avatar-small, .avatar-xlarge, .avatar-xsmall, .avatar-xxlarge {
filter: drop-shadow(0px 0px 5px rgba(0,0,0,0.7)) !important;
}
.chat .avatar-large {
width: 50px !important;
height: 50px !important;
background-size: cover !important;
}
/****************************************************************/
/****************************************************************/
.chat .messages-wrapper {
-webkit-mask-image: -webkit-linear-gradient(top, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 1) 8%, rgba(0, 0, 0, 1) 98%, rgba(0, 0, 0, 0) 100%);
}
.scroller.channel-members { padding-top: 0px; }
.flex-vertical.channels-wrap { padding-left: 3px; }
.guilds-wrapper { padding-left: 3px; }
.username { font-size: 90%; }
.account .btn-deafen:hover {
background-color: rgba(0, 0, 0, .5);
z-index: 2;
}
.account .username {
font-size:10px;
white-space: nowrap;
overflow: hidden;
text-overflow: ellipsis;
}
.guilds {
animation: fadeScreen 1s;
transition: all 900ms ease;
}
.voice-connection-quality-fine,
.discriminator,
.username {
transition: all 900ms ease;
}
.channel-members,
.channel-members-wrap {
transition: all 400ms ease;
}
/****************************************************************/
/****************************************************************/
/*Markdown*/
.markdown-modal {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 0, 0, 0));
}
.markdown-modal.selectable .markdown-modal-header {
border-bottom: none;
}
.markdown-modal.selectable .scroller-wrap.fade .scroller {
transform: translate(0%,-25%);
}
.modal-3HOjGZ.modal-KwRiOq.size-2pbXxj {
background: linear-gradient(to bottom, rgba(0, 110, 140, 0.6), rgba(0, 110, 140, 0.1));
}
/****************************************************************/
/****************************************************************/
/*Member Headers*/
.channel-members h2 {
color: #007272;
font-size: 10px;
text-transform: uppercase;
letter-spacing: .08em;
font-weight: 700;
padding: 4px 58px;
background-color: rgba(0, 114, 114, 0.5);
border: 1px solid;
border-color: rgba(0, 0, 0, 0.2);
border-radius: 5px;
width: 90px;
margin-left: 15px;
text-align: center;
transition: all 400ms ease;
}
.channel-members:hover h2 {
border-radius: 50px;
transition: all 400ms ease;
}
/***************************************************************
/****************************************************************/
/*Modal 8*/
.modal {
opacity: 1!important;
-webkit-transform: scale(1) translateZ(0px)!important;
transform: scale(1) translateZ(0px)!important;
-webkit-animation: modalanim 400ms ease;
animation: modalanim 400ms ease;
-webkit-transition: all 100ms;
transition: all 100ms;
-webkit-transition-delay: 5s;
transition-delay: 5s;
}
span:active .modal {
-webkit-transition-delay: 0s;
transition-delay: 0s;
-webkit-transform: scale(1)!important;
transform: scale(1)!important;
opacity: 0!important;
}
span:active .modal:hover {
-webkit-transform: scale(1)!important;
transform: scale(1)!important;
opacity: 1!important;
}
.callout-backdrop:active {
opacity: 0!important;
-webkit-transition: all 100ms!important;
transition: all 100ms!important;
-webkit-transition-delay: 0s;
transition-delay: 0s
}
.callout-backdrop {
-webkit-transition-delay: 5s;
transition-delay: 5s;
}
.callout-backdrop {
opacity: 0.9!important;
-webkit-transition: all 400ms ease;
transition: all 400ms ease;
-webkit-animation-name: bg-in;
animation-name: bg-in;
-webkit-animation-iteration-count: 1;
animation-iteration-count: 1;
-webkit-animation-timing-function: ease;
animation-timing-function: ease;
-webkit-animation-duration: 400ms;
animation-duration: 400ms;
-webkit-transition-delay: 100s!important;
transition-delay: 100s!important;
}
/****************************************************************/
/****************************************************************/
/*Need Help*/
.need-help-modal .header{
border-radius: 0;
}
.need-help-modal .footer{
border: 0;
border-radius: 0;
background-color: rgba(42, 42, 42, 0.8);
}
.need-help-modal .header input[type=text]{
border-radius: 0;
box-shadow: none;
}
.need-help-modal.deprecated{
background-color: rgba(42, 42, 42, 0.8);
}
.need-help-modal.deprecated .header{
background-color: rgba(0, 0, 0, 0.42);
border-radius: 0;
}
.need-help-modal.deprecated .header input[type=text]{
background-color: rgba(0, 0, 0, 0.8);
border: none;
border-radius: 0;
box-shadow: none;
}
.need-help-modal.deprecated .footer{
background: rgba(0, 0, 0, 0.42);
border-radius: 0;
border: none;
}
/****************************************************************/
/****************************************************************/
/*Popout*/
.popout.popout-bottom .popout-menu,
.context-menu,
.context-menu .item,
.status-picker.popout-menu,
.context-menu .scroller {
background-color: rgba(0,114,140,0.95) !important;
border-radius:;
}
.context-menu .item:hover {
background-color: rgba(0,70,140,0.95) !important;
}
.popout-menu-item:hover {
background-color: rgba(0,57,114,0.95) !important;
}
.context-menu .item{
background-color: rgba(0, 0, 0, 0) !important;
}
.context-menu{
box-shadow: none;
}
.context-menu .context-menu{
background-color: rgba(42, 42, 42, 0.8) !important;
}
.context-menu .item:hover{
background-color: rgba(255, 255, 255, 0.2) !important;
color: rgba(255, 255, 255, 0.8);
}
.avatar-1BXaQj,
.avatarWrapper-2Gfmp1 {
    border: none;
    border-radius: 3px;
}
.mask-2vyqAW {
    mask: none;
}
.popout:not(.popout-top),
#pubs-container,
#voice-connection-popout,
.incoming-call {
outline: 90vw solid rgba(8,8,8,.33);
outline-offset: -1px;
animation: backdrop 160ms ease-in;
}
#voice-connection-popout header,
#voice-connection-popout section {
background-color: rgba(0,114,114,0.8) !important;
}
#voice-connection-popout section::after {
display: none;
}
@keyframes backdrop {
0% {outline: 0vh solid rgba(8,8,8,0);}
55% {outline: 0vh solid rgba(8,8,8,.05);}
100% {outline: 90vw solid rgba(8,8,8,.35);}
}
.popout.popout-bottom.no-arrow {
outline: none;
animation: none;
}
.popout.popout-bottom-right {
background: transparent;
}
.popout.popout-bottom-right .header {
background: transparent;
background-color: rgba(0, 114, 114, 0.7);
}
.popout.popout-bottom-right .scroller-wrap{
background: transparent !important;
background-color: rgba(0, 114, 114, 0.4);
border: 1px solid #00cccc;
}
.popout.popout-bottom-right .scroller-wrap .scroller.messages-popout,
.popout.popout-bottom-right .scroller-wrap .scroller.messages-popout .message-group {
background: transparent;
background-color: rgba(0, 57, 57, 0.8);
border: 1px solid #00cccc;
}
[class*=userPopout] [class*=avatarWrapperNormal] [style*=image] {
    background-color:unset;
    width:100%;
    height:242px;
    width:242px;
    background-size:contain;
    background-position:center;
    background-repeat:no-repeat;
    border-radius:0;
    border:none;
    mask:unset;
    -webkit-mask:unset;
    box-shadow:unset;
    margin-bottom: 11px;
}
[class*=userPopout] [class*=avatarWrapperNormal] {
    margin:0;
    position:absolute;
    top:4px;
    left:4px;
    width:100%;
    height:250px;
    border-radius:0
}
[class*=userPopout] [class*=avatar-][class*=popout-] {
    width:100%;
    height:100%;
    border:none;
    border-radius:unset
}
[class*=userPopout] [class*=header]:hover [class*=avatarWrapperNormal] {
    -webkit-filter: grayscale(14%);
    transition: -webkit-filter 500ms ease-out;
}
[class*=userPopout] [class*=headerNormal],
[class*=userPopout] [class*=headerStreaming] {
    height:254px;
    transition: -webkit-filter 100ms;
    background:#fff;
    padding:0
}
[class*=userPopout] [class*=headerText] {
    height:236px;
    width:200px;
    overflow:hidden;
    position:absolute;
    top:2px;
    display:flex;
    flex-flow:column;
    pointer-events:none;
    justify-content:flex-end
}
[class*=userPopout] [class*=avatarWrapperNormal] [class*=avatarHint-] {
    background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);
    margin:0;
    box-shadow:none;
    opacity:0;
    border-radius:0;
    transition: opacity 180ms ease-out 100ms;
    -webkit-mask:unset;
}
[class*=userPopout] [class*=avatarWrapperNormal]:hover [class*=avatarHint-] {
    background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);
    transition:opacity 300ms ease-in 80ms;
    opacity:1;
}
[class*=userPopout] [class*=headerText] div[class*=header] {
    background: linear-gradient(to right, rgba(0,0,0,0) 0%,rgba(0,0,0,0.4) 15%,85%,rgba(0,0,0,0) 100%);
    width: 200px;
    max-width: 200px;
    padding:0;
    order:2;
    opacity:1;
    transition: opacity 200ms ease-in;
    transition-delay: 170ms;
    min-height:19px;
    pointer-events:auto
}
[class*=userPopout] .username-wrapper .nickname {
    margin-bottom:4px;
}
[class*=userPopout] [class*=headerText] [class*=ctivity] {
    height:auto;
    max-height:40px;
    overflow:hidden;
}
[class*=userPopout] [class*=tatus] {
    bottom:-4px;
    width:246px;
    height:8px;
    left:-4px;
    box-shadow: inset 0 0 0 1.8px rgba(255,255,255,.2);
    border-radius:0;
    pointer-events:none;
}
[class*=userPopout] [class*=header]:hover [class*=avatarWrapperNormal] [class*=tatus] {
    -webkit-filter: contrast(105%);
    transition: -webkit-filter 480ms ease-out;
}
[class*=userPopout] [class*=headerStreaming] [style*=image] [class*=tatus] {
    border:none;
}
[class*=userPopout] a[class*=Live] {
    position:fixed;
    left:0;
    right:0;
    top:20px;
    z-index:2;
    border:none !important;
    border-bottom:1px solid rgba(255,255,255,.08);
    padding:3px 25px;
    pointer-events:auto;
    width:200px;
    height:16px;
}
[class*=userPopout] a[class*=Live]:hover {
    background:transparent;
}
[class*=userPopout] a[class*=Live] [class*=con] {
    position:absolute;
    z-index:-1;
    width:200px;
    height:100%;
    border-radius:0;
    background:linear-gradient(to right,transparent,#f04747 15%,#f04747 85%,transparent);
    animation:l-p 1s ease-in-out infinite alternate;
}
@keyframes l-p {0%,20%{opacity:.6} 0%,10%,30% {opacity:1}}
[class*=userPopout] .member-roles {
    max-height: 90px;
    overflow-y: scroll;
}
[class*=userPopout] .member-roles::-webkit-scrollbar {
    width:0;
}
/****************************************************************/
/****************************************************************/
/*Public Servers*/
#pubs-container {
background: transparent;
background-color: rgba(0, 0, 0, 0.7) !important;
border-radius: 10px;
}
#pubs-header {
background: transparent !important;
border-top-right-radius: 5px;
border-top-left-radius: 5px;
}
.bda-dark .server-row {
background-color: rgba(0, 0, 0, 0.3) !important;
transition: all .3s ease-in-out;
}
.bda-light .server-row {
background-color: rgba(0, 0, 0, 0.3) !important;
transition: all .3s ease-in-out;
}
.server-row button {
background-color: rgba(0, 244, 244, 0.4) !important;
border-radius: 5px;
transition: all .3s ease-in-out;
}
.server-row button:hover {
background-color: rgba(0, 244, 244, 0.7) !important;
border-radius: 5px;
transition: all .3s ease-in-out;
}
.bd-dropdown-select {
background-color: rgba(0, 204, 204, 0.9) !important;
transition: all .3s ease-in-out;
color: #fff !important;
border-radius:5px;
}
div.bd-dropdown-list {
background: transparent;
}
input#pubs-sterm {
background-color: rgba(0, 204, 204, 0.9) !important;
transition: all .3s ease-in-out;
color: #fff;
padding-left:7px;
border-radius:5px;
width:120px;
margin-right:10px;
margin-left:-10px;
}
button#pubs-searchbtn {
background-color: rgba(0, 204, 204, 0.9) !important;
transition: all .3s ease-in-out;
color: #fff;
border-radius:5px;
}
.pubs-cat-select-li {
background: transparent;
background-color: rgba(0, 204, 204, 0.8) !important;
transition: all .3s ease-in-out;
color: #fff !important;
}
.server-row .server-icon {
border-radius: 5px !important;
border: 2px solid #00cccc;
}
#pubs-select-dropdown > div > ul {
border-bottom-left-radius: 5px;
margin-top:-2px;
}
div.bd-dropdown {
background: transparent;
transition: all .3s ease-in-out;
}
#pubs-footer {
background: transparent;
background-color: rgba(0, 204, 204, 0.5) !important;
border-bottom-right-radius: 10px;
border-bottom-left-radius: 10px;
border-top: 1px solid rgba(255,255,255,0.3);
}
#pubs-scroller::-webkit-scrollbar-thumb {
background-color: rgba(0, 0, 0, 0.3);
border: 2px solid rgba(0, 0, 0, 0.4);
}
#pubs-scroller::-webkit-scrollbar-track-piece {
background-color: rgba(0, 0, 0, 0.3);
border: 1px solid rgba(0, 0, 0, 0.2);
}
/****************************************************************/
/****************************************************************/
/*Region Select and server invite*/
.region-select-modal {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 57, 57, 1)) !important;
}
.region-select-modal-option {
background: linear-gradient(to bottom, rgba(0, 57, 57, 0.6), rgba(0, 0, 0, 1)) !important; 
}
.region-select-modal-option:hover {
background: linear-gradient(to bottom, rgba(0, 94, 94, 0.6), rgba(0, 0, 0, 1)) !important; 
}
.instant-invite-modal {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 57, 57, 1)) !important;
}
.form-header .blurb { 
color: white !important;
}
.instant-invite-modal .form-header, .instant-invite-modal .form-actions {
background: inherit !important
}
/****************************************************************/
/****************************************************************/
/*Search*/
.search-results-wrap .action-buttons .jump-button{
border-radius: 0;
}
.date-picker {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 57, 57, 1)) !important;
}
.react-datepicker {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 85, 85, 1)) !important;
}
.react-datepicker__header {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 85, 85, 1)) !important;
}
.search-popout:nth-child(1) {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 57, 57, 1)) !important;
}
.option.search-query.selected {
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.6), rgba(0, 57, 57, 1)) !important;
}
.results-group .option::after {
display: none;
}
.results-group .option:hover {
background: linear-gradient(to bottom, rgba(0, 57, 57, 0.6), rgba(0, 57, 57, 1)) !important;
}
.react-datepicker__current-month {
color: white !important;
}
.react-datepicker__day-name {
color: white !important;
}
.react-datepicker__day,
.react-datepicker__day.react-datepicker__day--disabled {
color: rgba(225, 225, 225, 1) !important;
}
.react-datepicker__day.react-datepicker__day--outside-month {
background: transparent !important;
}
.react-datepicker__day.react-datepicker__day--disabled.react-datepicker__day--outside-month {
color: rgba(180, 180, 180, 1) !important;
}
.option.search-option.selected {
background: linear-gradient(to right, rgba(0, 114, 114, 0.6), rgba(0, 85, 85, 1)) !important;
color: white !important;
}
.option.search-option.selected::after,
.option.search-option::after {
background: transparent !important;
}
.option.history::after {
display: none;
}
/****************************************************************/
/****************************************************************/
/*Select*/
.Select-option{
background-color: rgba(42, 42, 42, 0.8);
}
.Select .Select-menu{
border-radius: 0;
}
.Select .Select-control{
border-radius: 0;
}
.has-value.is-pseudo-focused.Select--single>.Select-control .Select-value .Select-value-label,
.has-value.Select--single>.Select-control .Select-value .Select-value-label{
color: rgba(255, 255, 255, 0.8);
}
.Select-option.is-selected{
background-color: rgba(255, 255, 255, 0.075);
}
/****************************************************************/
/****************************************************************/
/*Settings*/
.settings-header {
background: linear-gradient(to right, rgba(0, 57, 57, 0.8), rgba(0, 57, 57, 0.6)) !important;
border: none !important;
}
.settings-inner {
background: linear-gradient(to right, rgba(0, 57, 57, 0.6), rgba(0, 57, 57, 0.2)) !important;
border: none !important;
}
.scroller.user-settings-modal-games {
background: linear-gradient(to right, rgba(0, 57, 57, 0.6), rgba(0, 57, 57, 0.2)) !important;
color: #ffffff !important;
}
.settings-actions {
background: linear-gradient(to right, rgba(0, 57, 57, 0.6), rgba(0, 57, 57, 0.2)) !important;
border: none !important;
}
.form-inner {
background-color: rgba(0, 0, 0, 0.6);
}
.form-header header {
color: #00cccc !important;
}
.form-inner p {
color: #ffffff !important;
}
.btn.btn-default.close {
background-color: rgba(0, 0, 0, 0.0);
color: #00cccc;
}
.form-header {
background-color: rgba(0, 0, 0, 0.5) !important;
}
.form-actions {
background-color: rgba(0, 0, 0, 0.5) !important;
}
ul li a {
color: #00cccc !important;
}
.header.control-group {
background-color: #00cccc !important;
border-top-right-radius: 10px;
border-top-left-radius: 10px;
}
.avatar-uploader-inner {
background-color: rgba(0, 0, 0, 0.1);
border-radius: 20px !important;
}
#settings-username {
border-radius: 10px;
padding-left: 10px;
border-color: #00cccc;
}
#settings-email {
border-radius: 10px;
padding-left: 10px;
border-color: #00cccc;
}
#settings-current-password {
border-radius: 10px;
padding-left: 10px;
border-color: #00cccc;
}
button.btn.btn-primary {
background-color: #00cccc;
}
.settings-actions {
background-color: rgba(0, 57, 57, 0.7) !important;
}
a.remove-button {
color: #00cccc !important;
}
.control-group label a {
color: #00cccc !important;
}
.settings .settings-inner,
.settings .settings-actions {
background-color: rgba(0, 57, 57, 0.3) !important;
}
.settings .settings-header {
background-color: rgba(0, 57, 57, 0.7) !important;
}
.settings-wrapper.settings-panel {
background-color: rgba(0, 57, 57, 0.4) !important;
}
.settings .settings-inner,
.settings .settings-actions {
background: rgba(0, 57, 57, 0.5);
}
.radio-inner {
background-color: rgba(255, 255, 255, 0.3) !important;
}
.tab-bar-item {
margin-right: 10px !important;
}
div p a {
color: #00cccc !important;
}
.radio-theme.dark label {
border-color: #00cccc !important;
}
.radio-theme.light label {
border-color: #aaffff!important;
}
.user-settings-appearance .control-groups:nth-child(1) .control-group label:after {
content: " style: (Dark looks much better than light!)";
}
.user-settings-modal button.preview-sound:before {
-webkit-filter: hue-rotate(305deg) saturate(400%);
}
.action-icon:before {
-webkit-filter: hue-rotate(305deg) saturate(400%) !important;
}
.slider-bar-fill {
background: #00cccc !important;
}
.radio .radio-inner span:after {
background: #00cccc !important;
}
.tab-bar-item:hover {
background-color: transparent;
}
.tab-bar.TOP .tab-bar-item.selected {
border-bottom: 2px solid #00cccc !important;
}
#help-query {
border-color: #00cccc;
border-width: 3px;
}
.reset-voice-settings {
color: #00cccc !important;
}
.form-inner header {
color: #00cccc !important;
}
.form-inner {
background-color: rgba(0, 0, 0, 0.1) !important;
}
.scroller.guild-settings-modal-list.settings-panel-with-header .member .member-username {
color: white;
}
#overlay-explanation{
background-color: rgba(242, 101, 34, 0.8);
border-radius: 0;
}
.now-playing{
border-radius: 0;
}
.hover-roll div{
color: rgba(255, 255, 255, 0.6);
}
.deprecated-settings-modal .settings-header{
background-color: rgba(42, 42, 42, 0.3);
border-radius: 0;
}
.tab-bar.SIDE{
overflow: hidden;
}
.settings .settings-inner:first-child,
.settings .settings-actions{
background-color: rgba(42, 42, 42, 0.8);
border: 0;
border-radius: 0 !important;
}
.tab-bar.TOP{
border-color: rgba(255, 255, 255, 0.2);
}
.form .control-group input[type=text],
.form .control-group input[type=email],
.form .control-group input[type=password]{
padding-left: 8px;
color: rgba(255, 255, 255, 0.9);
background-color: rgba(255, 255, 255, 0.2);
border: 0;
}
.checkbox .checkbox-inner+span{
color: rgba(255, 255, 255, 0.9);
}
.form .control-group label+.radio-group{
color: rgba(255, 255, 255, 0.8);
}
.has-value>.Select-control>.Select-placeholder{
color: rgba(255, 255, 255, 0.8);
}
div.game-name,
input.game-input{
color: rgba(255, 255, 255, 0.8);
}
.theme-dark .user-settings-account .view-body{
color: rgba(255, 255, 255, 0.9);
}
.theme-dark .faded-1KRDbu{
color: rgba(255, 255, 255, 0.6);
}
.user-settings-modal-games{
background-color: rgba(42, 42, 42, 0.0);
border: 0;
box-shadow: none;
}
.user-settings-modal-games .games-table .games-row .item-game,
.user-settings-modal-games .games-table .games-row .item-overlay{
border-color: rgba(255, 255, 255, 0.2);
}
.user-settings-modal-locale .select-item .primary{
color: rgba(255, 255, 255, 0.9) !important;
}
.user-settings-locale .select-item .primary,
.user-settings-locale .select-item .localized
{
color: rgba(255, 255, 255, 0.8) !important;
}
.Select-control{
background-color: rgba(0, 0, 0, 0.2);
border: 0 !important;
border-radius: 0;
}
.is-open>.Select-control{
background-color: rgba(0, 0, 0, 0.2);
}
.Select-menu-outer{
margin-top: 0;
background-color: rgba(42, 42, 42, 0.8);
border: 0;
border-radius: 0;
}
.form .Select-option{
color: rgba(255, 255, 255, 0.8);
}
.form .Select-option.is-focused{
background-color: rgba(255, 255, 255, 0.3);
color: rgba(255, 255, 255, 0.8);
}
.form .control-group label{
color: rgba(255, 255, 255, 0.5);
}
.form .control-groups>.control-group{
color: rgba(255, 255, 255, 0.8);
}
.form hr{
border-color: rgba(255, 255, 255, 0.2);
}
.settings-connections-wrapper .user-settings-modal-connections .user-settings-modal-accounts-list h3{
color: rgba(255, 255, 255, 0.5);
}
.settings-connections-wrapper .user-settings-modal-connections .user-settings-modal-accounts-list .user-settings-modal-accounts-list-description .user-settings-modal-accounts-list-description-inner{
color: rgba(255, 255, 255, 0.3);
}
.settings-connections-wrapper .user-settings-modal-connections .user-settings-modal-connections-list{
box-shadow: none;
}
.connect-account-btn .connect-account-btn-inner{
border-radius: 0;
}
.settings-connections-wrapper .user-settings-modal-connections .user-settings-modal-connections-list .connection{
border-radius: 0;
}
.settings-connections-wrapper .user-settings-modal-connections .user-settings-modal-connections-list .connection .connection-header .btn-delete{
border-radius: 0;
}
.settings-connections-wrapper .authed-app{
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2);
border: 0;
}
.settings-connections-wrapper .authed-app .details .header{
color: rgba(255, 255, 255, 0.42);
}
.settings-connections-wrapper .authed-app .header .header-actions .action-btn{
border-radius: 0;
}
.settings-connections-wrapper .authed-app .details .body,
.settings-connections-wrapper .authed-app .details .body li,
.settings-connections-wrapper .authed-app .header .app-name{
color: rgba(255, 255, 255, 0.8);
}
.user-settings-modal .account-warning{
border-radius: 0;
border: 0;
background-color: rgba(253, 237, 237, 0.9);
}
.user-settings-modal-keybinds .user-settings-modal-keybinds-header{
border-color: rgba(255, 255, 255, 0.2);
}
.user-settings-authorized-apps .authed-app{
background-color: rgba(255, 255, 255, 0.1);
}
.settings .settings-inner .settings-panel{
background-color: rgba(0, 0, 0, 0);
}
.form .btn-default{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border: 0;
padding: 10px;
}
.form .btn-default:hover{
border: 0;
}
.form .btn-primary{
border-radius: 0;
color: rgba(255, 255, 255, 0.9);
}
.form header{
color: rgba(255, 255, 255, 0.8) !important;
}
.form.deprecated .btn-primary{
border-radius: 0;
}
#instant-invite-modal .blurb{
color: rgba(255, 255, 255, 0.5);
}
.instant-invite-modal{
background-color: rgba(42, 42, 42, 0.8);
border-radius: 0;
}
.instant-invites .instant-invites-list .instant-invite+.instant-invite{
border-color: rgba(255, 255, 255, 0.2);
}
.instant-invites .instant-invites-list .instant-invite .member{
color: rgba(255, 255, 255, 0.8);
}
.instant-invites .instant-invites-list .instant-invite .channel{
color: rgba(255, 255, 255, 0.3);
}
.checkbox .checkbox-inner span{
border-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
}
.checkbox .checkbox-inner+span{
color: rgba(255, 255, 255, 0.5);
}
#instant-invite-modal .form-inner,
#instant-invite-modal .form-header,
#instant-invite-modal .form-actions,
#instant-invite-modal-advanced .form-inner,
#instant-invite-modal-advanced .form-actions{
background-color: rgba(0, 0, 0, 0);
}
#permissions ul li{
color: rgba(255, 255, 255, 0.8);
}
#permissions .permission-actions>div{
background-color: rgba(255, 255, 255, 0.3);
border-color: rgba(0, 0, 0, 0);
border-radius: 0;
}
#permissions .permission-actions.disabled>div{
background-color: rgba(255, 255, 255, 0.1);
border-color: rgba(0, 0, 0, 0);
}
.form .control-group textarea{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border: 0;
}
.form .form-header,
.form .form-inner,
.form .form-actions
{
background-color: rgba(42, 42, 42, 0.8);
color: rgba(255, 255, 255, 0.9);
border-radius: 0;
border: 0;
}
.form .form-inner:first-child,
.form .form-inner:last-child{
border-radius: 0;
}
.alert.form .form-inner .cancel{
border-radius: 0;
}
.alert.form.has-icon:before{
border-radius: 0;
background-color: rgba(0, 0, 0, 0);
}
div.control-group .shortcut-recorder input[type=text]{
border: 0;
border-radius: 0;
background-color: rgba(255, 255, 255, 0.2) !important;
color: rgba(255, 255, 255, 0.8);
}
.notice.notice-streamer-mode{
background-color: rgba(89, 54, 149, 0.5);
}
.notice.notice-danger{
background-color: rgba(240, 71, 71, 0.5);
}
.notice{
background-color: rgba(242, 101, 34, 0.5);
color: rgba(255, 255, 255, 0.9);
}
.notice .btn{
background-color: rgba(255, 255, 255, 0.2);
color: rgba(255, 255, 255, 0.8);
border-radius: 0;
border: 0;
}
.notice .btn:hover{
background-color: rgba(255, 255, 255, 0.3);
color: rgba(255, 255, 255, 0.9) !important;
}
.channel-notice.invite{
background: url(/assets/bf625d222187f542b9d7179109422e2c.svg) center 20px no-repeat #282b30;
background-color: rgba(0, 0, 0, 0.3) !important;
}
.channel-notices .channel-notice{
box-shadow: none;
}
.channel-notices .channel-notice .message .btn,
.channel-notices .channel-notice.quickswitcher-notice,
.channel-notices .channel-notice.guild-mfa-warning{
color: rgba(255, 255, 255, 0.9);
background-color: rgba(0, 0, 0, 0.42);
}
.channel-notices .channel-notice .message .btn{
border-radius: 0;
border: none;
}
.account {
padding-top: 2px;
background-color: rgba(0, 0, 0, 0.42) !important;
border: 0 !important;
}
.account .btn-group,
.account .btn-group .btn {
border: 0 !important;
}
.account .btn-group .btn {
border-radius: 15px;
background: rgba(0, 0, 0, 0.3) !important;
box-shadow: none;
outline: 0;
border: 0 !important;
}
.account .btn-group .btn:hover {
border-radius: 15px;
background: rgba(0, 0, 0, 0.7) !important;
box-shadow: 0;
border: 0 !important;
}
.user-settings-security .btn-ghost{
padding-top: 10px;
padding-bottom: 10px;
background-color: rgba(255, 255, 255, 0.2);
border: 0;
border-radius: 0;
}
.btn-confirm{
border-radius: 0;
}
/****************************************************************/
/****************************************************************/
/*Smaller Channel Member Tab*/
.channel-members {
z-index:2;
transition:all 400ms ease;
transform: translateX(3%);
}
.channel-members:hover{
animation: member 400ms ease;
transform: translateX(-60%);
}
.app { overflow-x: hidden; }
.channel-members .member .member-activity,
.channel-members .member .member-username-inner{
opacity:0;
transition:all 400ms ease;
}
.channel-members .member .member-username-inner{
margin-bottom:10px;
}
.channel-members:hover .member .member-activity,
.channel-members:hover .member .member-username-inner{
opacity:1;
transition:all 400ms ease;
}
.channel-members h2 {
transform: scale(0.7) translateX(-33%) !important;
padding-left: 0px !important;
padding-right: 0px !important;
transition: all 400ms ease !important;
border-radius: 5px !important;
}
.channel-members:hover h2 {
transform: scale(1.0) translateX(8%) !important;
padding-left: 20% !important;
padding-right: 20% !important;
transition: all 400ms ease !important;
}
.header-toolbar button.active{
display:none;
}
.channel-members .avatar-small{
transform: scale(1) translateX(-30%) !important;
transition: all 400ms ease !important;
}
.channel-members:hover .avatar-small{
transform: translateX(0%) !important;
transition: all 400ms ease !important;
}
.chat.flex-vertical.flex-spacer.private>.content.flex-spacer.flex-horizontal>.flex-spacer.flex-vertical{
margin-right:0px !important;
z-index:0
}
.channel-members-wrap{
min-width:90px!important;
width:90px!important
}
/****************************************************************/
/****************************************************************/
/*Status*/
.status.status-typing {
    right: -2px !important;
}
.popout.popout-top .status-picker.popout-menu .popout-menu-item:hover {
background-color: rgba(0,57,57,0.8);
}
/*Dnd*/
.status-dnd ~ .status-text {
font-size: 0;
}
.status-dnd ~ .status-text::after {
content: "Busy";
font-size: 15px; 
}
.status-picker .popout-menu-item:nth-child(4) .helper{
font-size: 0; 
}
.status-picker .popout-menu-item:nth-child(4) .helper::after{
content: "Working...";
animation: working 3s linear infinite;
font-size: 12px;
}
.account:hover .status.status-dnd:after {content: "Working..."; animation: working 3s linear infinite;}
.status-dnd {
background-color: transparent !important;
border-color: #f04747 !important;
}
.popout-menu-item .status-dnd {
background: #f04747 !important;
}
/********************************/
/*Invisible*/
.status-invisible ~ .status-text {
font-size: 0; 
}
.status-invisible ~ .status-text::after {
content: "Invisible";
font-size: 15px; 
}
.status-picker .popout-menu-item:nth-child(5) .helper{
font-size: 0; 
}
.status-picker .popout-menu-item:nth-child(5) .helper::after{
content: "No one likes you so you decide to turn invisible because people don't notice you anyway." !important;
font-size: 12px;
}
.account:hover .status.status-invisible:after {content: "Invisible";}
.status-offline,
.status-invisible {
background-color: transparent !important;
border-color: #747f8d !important;
}
.popout-menu-item .status-invisible {
background: #747f8d !important;
}
/********************************/
/*Online*/
.account:hover .status.status-online:after {content: "Online";}
.popout-menu-item .status-online { background: #43b581 !important; }
.status-online {
background-color: transparent !important;
border-color: #43b581 !important;
}
/********************************/
/*Idle*/
.account:hover .status.status-idle:after {content: "Idle";}
.status-idle {
background-color: transparent !important;
border-color: #faa61a !important;
}
.popout-menu-item .status-idle {
background: #faa61a !important;
}
/********************************/
/*Account Hover*/
.account:hover .status.status-online:after,
.account:hover .status.status-idle:after,
.account:hover .status.status-dnd:after,
.account:hover .status.status-invisible:after {
text-align: center;
color: #00C8C8;
font-size: 11px;
position: absolute;
top: 110%;
left: 0%;
border-color: rgba(0,74,74,0.7);
border-bottom-left-radius: 5px;
border-bottom-right-radius: 5px;
z-index: -5;
transition-timing-function: ease-in;
transition: padding 0.25s, transform 0.25s, width 0.25s, border 0.25s, font-size 0.25s, top 0.25s, left 0.25s;
}
.account .status.status-online:after,
.account .status.status-idle:after,
.account .status.status-dnd:after,
.account .status.status-invisible:after {
top: 0%;
left: 0%;
content: "";
font-size: 11px;
transition-timing-function: ease-in;
transition: padding 0.25s, transform 0.25s, width 0.25s, border 0.25s, font-size 0.25s, top 0.25s, left 0.25s;
}
/********************************/
.avatar-small .status {
width: 30px !important;
height: 30px !important;
transition:all 400ms ease;
border-radius: 7px !important;
}
.avatar-small:hover .status {
border-radius: 50px !important;
transition:all 400ms ease;
}
.channel-members .avatar-small .status { right: -2px !important; }
/****************************************************************/
/****************************************************************/
/*Title bar*/
.titleBar-3_fDwJ {
height:32px!important;
background-size: cover;
background: transparent;
background: linear-gradient(to right, rgba(0, 0, 0, 1), rgba(0, 0, 0, 0.0)) !important;
}
svg[name="DiscordWordmark"] {
width: 82px;
height: 24px;
position: absolute;
top: 8px;
}
.popout-bottom[style*="overflow: hidden; visibility: visible;"] {
top:92px!important;
}
svg[name="TitleBarMaximize"], svg[name="TitleBarClose"], svg[name="TitleBarMinimize"] {
height:18px !important;
width:18px !important;
}
.winButton-U7zAqI {
height:36px;
}
.separator-win {
display:none
}
/****************************************************************/
/****************************************************************/
/*Tooltips*/
.tooltip.tooltip-right.tooltip-black {
background: rgba(0,114,114,0.8) !important;
transform: translateX(-30px) !important;
z-index: 0;
padding-top: 14px !important;
padding-bottom: 14px !important;
padding-left: 30px !important;
border-bottom-left-radius: 15px;
border-top-left-radius: 15px;
animation: guildtip 0.6s cubic-bezier(.65,1.79,.49,1.81) 0s, flash2 0.6s ease 0s;
filter:brightness(110%);
box-shadow: inset 4px 0 30px 10px rgba(180,180,220,.5)
transition:all 500ms ease;
}
.tooltip.tooltip-top.tooltip-black,
.tooltip.tooltip-bottom.tooltip-black {
background: rgba(0,114,114,0.8) !important;
z-index: 1;
animation: flash 0.5s;
-webkit-animation: flash 0.5s;
}
.tooltip.tooltip-right.tooltip-black:after {
border-right-color: rgba(0,114,114,0.8) !important;
}
.tooltip.tooltip-left.tooltip-black:after {
border-left-color: rgba(0,114,114,0.8) !important;
}
.tooltip.tooltip-top.tooltip-black:after {
border-top-color: rgba(0,114,114,0) !important;
}
.tooltip.tooltip-bottom.tooltip-black:after {
border-bottom-color: rgba(0,114,114,0) !important;
}
.tooltip.tooltip-right.tooltip-black.tooltip-error::after {
display: none;
}
.tooltip.tooltip-right.tooltip-black {
width: 0px !important;
transition: all 2s ease;
}
#app-mount:hover .tooltip.tooltip-right.tooltip-black {
width: initial !important;
transition: all 2s ease;
}
/****************************************************************/
/****************************************************************/
/*Topic*/
.topic.topic-expandable {
color: rgba(255, 255, 255, 0.8) !important;
font-size: 12px !important;
transition: all 400ms ease;
}
.topic.topic-expandable a {
color: #005555 !important;
transition: all 400ms ease;
}
.topic.topic-expandable:hover {
color: rgba(255, 255, 255, 0.8) !important;
font-size: 14px !important;
transition: all 400ms ease;
}
/****************************************************************/
/****************************************************************/
/*Voice connection*/
#voice-connection {
border-top: 1px solid rgba(255, 255, 255, 0.0);
}
#voice-connection .btn,
.account .btn {
border: none;
}
/****************************************************************/
/****************************************************************/
/*User popout*/
.user-popout .avatar-wrapper,
.user-popout .avatar-wrapper .avatar-popout {
border-color: transparent !important;
background-color: transparent !important;
margin: 0px 0px 0px;
width: 100%;
height: 242px;
display: flex;
flex: 1;
background-size: 242px 242px;
border-radius: 5px;
background-position: 0px !important;
background-repeat: no-repeat;
position: relative;
}
.user-popout .header:hover .avatar-wrapper {
-webkit-filter: grayscale(14%);
transition: -webkit-filter 500ms ease-out;
}
.user-popout .header {
height: 232px;
transition: -webkit-filter 100ms;
background: #fff;
border-bottom: 8px solid;
color: transparent;
z-index: 2;
}
.user-popout .avatar-wrapper.no-hover {
min-height: 250px;
top: 9px;
}
.user-popout .header:hover .username-wrapper {
width: 200px;
margin-top: -180px;
border-radius: 50px;
position: absolute;
top: 342px;
transition: top 170ms ease-out;
}
.user-popout .username-wrapper {
width: 200px;
margin-top: -180px;
position: absolute;
top: 366px;
transition: top 270ms ease-in-out;
z-index: 0;
}
.user-popout .header.streaming .live-on-twitch:hover {
background-color: transparent;
}
.user-popout .avatar-wrapper:hover .avatar-hint {
background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);
border-radius: 0px;
transition: opacity 400ms ease-in 80ms;
}
.user-popout .avatar-wrapper .avatar-hint {
background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);
box-shadow: none;
opacity: 0;
border-radius: 0px;
transition: opacity 180ms ease-out 100ms;
}
.user-popout :-webkit-any(.nickname, .activity, .discord-tag), .creation-date-wrapper {
background: linear-gradient(to right, rgba(0,0,0,0) 0%,rgba(0,0,0,0.4) 15%,rgba(0,0,0,0.4) 85%,rgba(0,0,0,0) 100%);
width: 200px;
max-width: 200px;
padding: 0 !important;
}
.user-popout .username-wrapper .nickname {
margin-bottom: 4px;
}
.user-popout .username-wrapper .activity {
height: 0px;
overflow: hidden;
word-break: break-all;
}
.user-popout .header:hover .username-wrapper .activity {
height: auto;
max-height: 35px;
}
.user-popout .avatar-wrapper .avatar-popout .status {
bottom: -8px;
width: 242px;
height: 8px;
left: 0px;
box-shadow: inset 0 0 0 1.8px rgba(255,255,255,.2);
border-radius: 5px;
z-index: 4;
}
.user-popout .header:hover .avatar-wrapper .avatar-popout .status {
-webkit-filter: contrast(105%);
transition: -webkit-filter 480ms ease-out;
}
.user-popout .body .section .label {
margin-top: 10px;
margin-bottom: 4px;
}
.user-popout .username-wrapper .nickname,
.user-popout .username-wrapper .discord-tag,
.user-popout .header:hover .username-wrapper .activty,
.user-popout .header:hover .creation-date-wrapper  {
opacity: 1;
overflow: hidden;
transition: opacity 200ms ease-in;
transition-delay: 170ms;
}
.user-popout .username-wrapper .actiity,
.user-popout .creation-date-wrapper {
opacity: 0;
transition: opacity 200ms;
}
.creation-date-wrapper {
text-align: center;
top: 2px;
position: absolute;
padding: 3px 0 !important;
}
.user-popout .header.streaming .live-on-twitch {
position: fixed;
top: 20px;
left: 34px;
border-top: none;
border-bottom: 1px solid rgba(255,255,255,.08);
background: linear-gradient(to right, rgba(250,250,250,0) 0%,rgba(250,250,250,0.05) 15%,rgba(250,250,250,0.05) 85%,rgba(250,250,250,0) 100%);
padding: 4px 25px;
}
.user-popout .header.streaming {
padding-bottom: 6px;
}
.user-popout .header.streaming .status {
bottom: -6px;
}
.user-popout .header.streaming .avatar-popout {
padding-bottom: 4px;
top: -2px;
}
.user-popout .member-roles {
max-height: 90px;
overflow-y: scroll;
}
.user-popout .member-roles::-webkit-scrollbar {
width: 0px;
}
.user-popout .body {
z-index: 1;
padding-top: 4px;
background: linear-gradient(to bottom, rgba(0, 114, 114, 1), rgba(0, 114, 114, 0.7)) !important;
}
.user-popout .footer {
z-index: 1;
border: none;
background: linear-gradient(to bottom, rgba(0, 114, 114, 0.7), rgba(0, 114, 114, 0.4)) !important;
}
.user-popout .status {
display: none !important;
}
/****************************************************************/
/****************************************************************/
/*User Profile Modal*/
#user-profile-modal .avatar-wrapper {
    border: 3px solid white;
    border-radius: 3px;
    top: 37px;
    left: 16px;
    box-shadow: 1px 0px 8px 0px rgba(50,56,97,.24);
}
#user-profile-modal .avatar-profile {
    border-radius: 3px;
}
#user-profile-modal .header .header-info .header-info-inner {
    padding: 5px;
    margin: -5px;
    border-radius: 4px;
    box-shadow: 1px 2px 3px 0 rgba(20,20,50,.14);
    word-break: break-all;
    background-color: rgba(0,0,0,0.2);
}
#user-profile-modal .header .header-info .header-info-inner .activity {
    color: rgba(180,180,190, 0.98);
    width: auto;
    max-width: 304px;
}
#user-profile-modal .header .header-info .header-info-inner .discord-tag .username,
#user-profile-modal .header .header-info .header-info-inner .discord-tag .discriminator {
    color: white !important;
}
#user-profile-modal .header .header-info .header-info-inner .discord-tag .discriminator::before {
    content: " ";
}
#user-profile-modal .header:after {
    background: transparent;
}
#user-profile-modal .header .additional-actions-icon {
    -webkit-filter: brightness(200%);
    border: 1px rgba(255,255,255,.4);
    border-radius: 5px;
    top: 14px;
    right: 14px;
    padding: 2px 2px;
    transition: .2s ease-in;
}
#user-profile-modal .header .additional-actions-icon:hover {
box-shadow: 0 0 20px -4px rgba(255,255,255,.2) inset;
}
#user-profile-modal .header .additional-actions-icon:active {
-webkit-filter: brightness(145%);
}
#user-profile-modal .actions .btn.add-friend:-webkit-any(:active, :hover:active) {
background: #64c599 !important;
}
#user-profile-modal .actions .btn.add-friend:hover {
background: #71cea3;
}
#user-profile-modal .actions .btn.add-friend {
margin-left: -5px;
box-shadow: 1px 2px 3px 0 rgba(20,20,45,.06);
background: #48c78d;
}
#user-profile-modal .actions .btn:-webkit-any(.disabled, .disabled:hover) {
opacity: 1;
margin-left: -5px;
background: rgba(250,250,250,.1) !important;
color: #0bb;
border: 1px dashed rgba(210,210,210,.6);
}
#user-profile-modal .header .header-info,
#user-profile-modal .actions {
margin-left: -44px;
}
#user-profile-modal .header .header-info {
padding-top: 6px;
}
#user-profile-modal .status {
border: 3px solid #fff;
box-shadow: 1px 2px 5px 0px rgba(50,56,97,.08);
}
#user-profile-modal .tab-bar-container {
padding-left: 170px;
padding-right: 64px;
background: linear-gradient(to bottom, rgba(0, 57, 57, 0.4), rgba(0, 0, 0, 0)) !important;
border-bottom: 0px;
}
#user-profile-modal .empty {
display: none !important;
}
#user-profile-modal .tab-bar {
width: 100%;
justify-content: space-between;
}
#user-profile-modal .tab-bar .tab-bar-item {
padding: 0 10px 20px;
}
#user-profile-modal .tab-bar.TOP .tab-bar-item+.tab-bar-item {
margin-left: 0px;
}
#user-profile-modal .scroller {
background: #f9f9f9;
}
#user-profile-modal .guilds .section .connected-accounts .connected-account {
background: linear-gradient(to right, rgba(0, 114, 140, 0.6), rgba(0, 57, 57, 1)) !important;
}
.connected-account-name {
color: white !important;
}
#user-profile-modal .header .actions .btn.add-friend {
background-color: rgba(0,114,140,0.8);
}
#user-profile-modal .status {
display: none;
}
#user-profile-modal .header {
background: linear-gradient(to bottom, rgba(0, 57, 57, 0.7), rgba(0, 57, 57, 0.4)) !important;
}
#user-profile-modal .scroller {
background: #fff;
padding-top: 0px;
border-top-right-radius: 0px;
border-bottom-right-radius: 0px;
border-right: 0px solid transparent;
margin-top: 0px;
margin-bottom: 0px;
}
#user-profile-modal{
border-radius: 0;
}
#user-profile-modal .btn{
border-radius: 0;
}
.note textarea,
#user-profile-modal .tab-bar .tab-bar-item.selected{
border-bottom-color: rgba(255, 255, 255, 0.8);
color: rgba(255, 255, 255, 0.8);
}
.note textarea:focus{
background-color: rgba(255, 255, 255, 0.2);
}
#user-profile-modal .guilds .section .section-header,
#user-profile-modal .tab-bar .tab-bar-item{
color: rgba(255, 255, 255, 0.3);
}
#user-profile-modal .guilds .section+.section{
border-color: rgba(255, 255, 255, 0.2);
}
#user-profile-modal .guilds .section .connected-accounts .connected-account{
background-color: rgba(255, 255, 255, 0.2);
border-radius: 0;
border: 0;
}
#user-profile-modal .guilds .section .connected-accounts .connected-account .connected-account-name-inner .connected-account-name{
color: rgba(255, 255, 255, 0.8);
}
#user-profile-modal .tab-bar-container {
background-color: rgba(100, 100, 100, 0.42) !important;
border: 0 !important;
}
#user-profile-modal .empty,
#user-profile-modal .scroller{
background-color: rgba(42, 42, 42, 0.42);
}
#user-profile-modal header {
background: rgba(114, 137, 218, 0.5) !important;
border: 0 !important;
}
#user-profile-modal footer {
background: rgba(255, 255, 255, 0.1) !important;
border: 0 !important;
}
/****************************************************************/
/**********************************************************************************************************************************/
/**********************************************************************************************************************************/
/****************************************************************/
/*Other*/
.live-on-twitch {
background-color: rgba(0,0,0,0.4) !important;
border-radius: 50px;
}
.scroller-wrap .scroller.settings-wrapper.settings-panel::-webkit-scrollbar,
.scroller-wrap .scroller.settings-wrapper.settings-panel::-webkit-scrollbar-track,
.scroller-wrap .scroller.settings-wrapper.settings-panel::-webkit-scroll-track-piece,
.scroller.guild-settings-modal-list.settings-panel-with-header::-webkit-scrollbar,
.scroller.guild-settings-modal-list.settings-panel-with-header::-webkit-scroll-track,
.scroller.guild-settings-modal-list.settings-panel-with-header::-webkit-scroll-track,-piece,
.guild-settings-modal-emoji .scroller::-webkit-scrollbar,
.guild-settings-modal-emoji .scroller::-webkit-scroll-track,
.guild-settings-modal-emoji .scroller::-webkit-scroll-track-piece,
.scroller.settings-panel::-webkit-scrollbar,
.scroller.settings-panel::-webkit-scroll-track,
.scroller.settings-panel::-webkit-scroll-track-piece,
.scroller.webhooks-list::-webkit-scrollbar,
.scroller.webhooks-list::-webkit-scroll-track,
.scroller.webhooks-list::-webkit-scroll-track-piece,
.scroller-wrap.fade .scroller::-webkit-scrollbar,
.scroller-wrap.fade .scroller::-webkit-scroll-track,
.scroller-wrap.fade .scroller::-webkit-scroll-track-piece,
.scroller-fzNley::-webkit-scrollbar,
.scroller-fzNley::-webkit-scroll-track,
.scroller-fzNley::-webkit-scroll-track-piece {
display: none;
}
.bda-dark #bda-qem-twitch-container .scroller::-webkit-scrollbar,
.bda-dark #bda-qem-twitch-container .scroller::-webkit-scrollbar-track,
.bda-dark #bda-qem-twitch-container .scroller::-webkit-scrollbar-track-piece,
.bda-dark #pubs-container .scroller::-webkit-scrollbar,
.bda-dark #pubs-container .scroller::-webkit-scrollbar-track,
.bda-dark #pubs-container .scroller::-webkit-scrollbar-track-piece {
background-color: rgba(0, 0, 0, 0.3) !important;
border: 1px solid rgba(0, 0, 0, 0.2) !important;
}
.bda-dark #bda-qem-favourite-container .scroller::-webkit-scrollbar-thumb,
.bda-dark #bda-qem-twitch-container .scroller::-webkit-scrollbar-thumb,
.bda-dark #pubs-container .scroller::-webkit-scrollbar-thumb,
.bda-dark .emoji-picker .scroller::-webkit-scrollbar-thumb {
background-color: rgba(0, 0, 0, 0.3) !important;
border: 2px solid rgba(0, 0, 0, 0.4) !important;
}
.bda-dark #bda-qem-favourite-container .scroller::-webkit-scrollbar-thumb:active,
.bda-dark #bda-qem-twitch-container .scroller::-webkit-scrollbar-thumb:active,
.bda-dark #pubs-container .scroller::-webkit-scrollbar-thumb:active,
.bda-dark .emoji-picker .scroller::-webkit-scrollbar-thumb:active {
background-color: rgba(0, 0, 0, 0.3) !important;
border: 1px solid rgba(0, 0, 0, 0.2) !important;
}
.bda-dark #bda-qem-favourite-container .scroller::-webkit-scrollbar,
.bda-dark #bda-qem-favourite-container .scroller::-webkit-scrollbar-track,
.bda-dark #bda-qem-favourite-container .scroller::-webkit-scrollbar-track-piece {
background-color: rgba(0, 0, 0, 0.3) !important;
border: 1px solid rgba(0, 0, 0, 0.2) !important;
}
.guild-settings-modal-members {
border: 1px solid #3DA9A9 !important;
background: rgba(0,57,57,0.8) !important;
}
.spinner-wandering-cubes .spinner-item {
background-color:#25ACE8;
width:15px;
height:15px;
border-radius:4px;
}
.form-inner.loading {
background-color: rgba(0, 0, 0, 0.5) !important;
}
.channel-members-loading {
display: none;
}
.countdown {
color: #00cccc !important;
}
.empty-message h1 {
color: rgba(255, 255, 255, 0) !important;
}
.empty-message {
display: none !important;
}
label.subtitle {
color: #00cccc !important;
}
label.title {
color: #00cccc !important;
}
div.control-group label {
color: #00cccc !important;
}
div.checkbox span {
color: #a6a6a6 !important;
}
div.help-text {
color: #ffffff !important;
}
.guild-channels header {
opacity: 0.9;
}
.guild-channels .channel a {
opacity: 0.7;
}
/****************************************************************/
/****************************************************************/
/*Extras*/
.avatar-large[style*="/168216897450541056/"] + .comment .message.first .body .username-wrapper:after {
content: 'Anonymous';
color: white;
margin-left: 5px;
background: #00a3d9;
border-radius: 5px;
padding: 1px 2px;
font-size: 10px;
font-weight: 600;
}
/****************************************************************/
/**********************************************************************************************************************************/
/**********************************************************************************************************************************/
/****************************************************************/
/****************************************/
/*  Quoter, Replyer                     */
/*======================================*/
/*            Plugin Support            */
/*======================================*/
/*                                      */
/****************************************/
/*Quoter*/
.quoter {
border-radius: 5px !important;
background-color: #007272 !important;
border-color: #007272 !important;
border-width: 5px !important;
}
/*Replyer*/
.replyer {
border-radius: 5px !important;
background-color: #005555 !important;
border-color: #005555 !important;
border-width: 5px !important;
}
/****************************************************************/
/*Background*/
:root {
--GCB: url(https://hansanonymous.github.io/files/bg.png);
--GC-version: "Glossy Cyan 5.1.0 by HansAnonymous";
}
.app, #pubslayerroot .layer .ui-standard-sidebar-view, body {
background: url(https://hansanonymous.github.io/files/bg.png) no-repeat center center fixed;
background-size: cover;
background-color: rgba(0,0,0,0) !important;
}
/*Custom Font*/
*:not(code) {
/*font-family: 'NF?????? Std W1', 'Open Sans', Whitney, Helvetica, Arial, sans-serif !important;*/
}ahttps://hansanonymous.github.io/files/bg.png
/****************************************************************/
/**********************************************************************************************************************************/
