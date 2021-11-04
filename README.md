/**
 * @name Discord Theme Toma awa
 * @version 3.1.1
 * @author Toma awa
 * @authorLink https://tinkypinky123321.wixsite.com/hackertinkypinky
 * @donate https://www.paypal.me/TomaawaCL
 * @description A sleek, customizable Discord theme. Discord server: https://discord.gg/4zYtNm2W24  Donate: https://www.paypal.me/TomaawaCL
 * @website https://tinkypinky123321.wixsite.com/hackertinkypinky
 * @source https://github.com/Tomaawa123/extras.css
 * @invite https://discord.gg/4zYtNm2W24
*/
@import url(https://plusinsta.xyz/discord-plus/assets/plugins.css);
@import url(https://plusinsta.xyz/discord-plus/assets/extras.css);
/* Main fonts */
@import url(https://fonts.googleapis.com/css?family=Poppins:400,700|Roboto:400,700|Righteous);
/* Localized fonts */
@import url(https://fonts.googleapis.com/css2?family=Kosugi&family=RocknRoll+One&family=Gothic+A1&family=Black+Han+Sans&family=PT+Sans+Caption&family=Russo+One&family=Palanquin+Dark&family=Raleway:wght@500&family=Commissioner&family=Alegreya+Sans:wght@700&family=Mitr&family=Lalezar&display=swap);

:root {
	--dplus-background: url(https://i.imgur.com/3AiL3yN.png);

	/* Accent colors */
	--dplus-accent-ui: #802060;
	--dplus-accent-ui-hover: #601545;

	/* Fonts */
	--dplus-font-ui: 'Poppins';
	--dplus-font-ui-ja: 'Kosugi';
	--dplus-font-ui-ko: 'Gothic A1';
	--dplus-font-ui-ru: 'PT Sans Caption';
	--dplus-font-ui-vi: 'Raleway';
	--dplus-font-ui-el: 'Commissioner';
	--dplus-font-body: 'Roboto';
	--dplus-font-header: 'Righteous';
	--dplus-font-header-ja: 'RocknRoll One';
	--dplus-font-header-ko: 'Black Han Sans';
	--dplus-font-header-ru: 'Russo One';
	--dplus-font-header-hi: 'Palanquin Dark';
	--dplus-font-header-th: 'Mitr';
	--dplus-font-header-el: 'Alegreya Sans';

	/* Radiuses */
	--dplus-radius-ui: 10px;
	--dplus-radius-avatar: 20%;
	--dplus-radius-server: 20%;

	/* Spacing */
	--dplus-spacing-ui: 10px;
	--dplus-spacing-app: 10px;

	/* Icons */
	--dplus-icon-home-dark: url(https://cdn.discordapp.com/attachments/895316639027986463/905801318705295381/home_dark.svg.jpg);
	--dplus-icon-home-light: url(https://cdn.discordapp.com/attachments/895316639027986463/905801318705295381/home_dark.svg.jpg);

		/* Icon sizes*/
	--dplus-icon-avatar-chat: 64px;
	--dplus-icon-avatar-list: 32px;
	--dplus-icon-avatar-profile: 80px;
	--dplus-icon-server-sidebar: 48px;
	--dplus-icon-server-list: 32px;

	/* Animation lengths */
	--dplus-anim-short: .2s;
	--dplus-anim-long: .5s;
	--dplus-anim-sticky: .2s;
	--dplus-anim-button: .25s;
	--dplus-anim-button-appear: .25s;

	/* Widths */
	--dplus-channels-width: 240px;
	--dplus-members-width: 240px;
	--dplus-scrollbar-width: 10px;

	/* Scales */
	--dplus-blur-scale: 100;
}

/* Disable animations for reduce-motion */
:root.reduce-motion {
	--dplus-anim-short: 0s;
	--dplus-anim-long: 0s;
	--dplus-anim-sticky: 0s;
	--dplus-anim-button: 0s;
	--dplus-anim-button-appear: 0s;
}

/* Background covers */
	/* Defaults */
:root {
	--dplus-dark-bgc-ui-base: hsla(0, 0%, 0%, 0.74);
	--dplus-dark-bgc-ui-base-hover: hsla(0, 0%, 0%, 0.82);
	--dplus-dark-bgc-ui-card: hsla(0, 0%, 7%, 0.75);
	--dplus-dark-bgc-ui-card-hover: hsla(0, 0%, 15%, 0.50);
	--dplus-dark-bgc-chatmsg: hsla(0, 0%, 0%, 0.74);
	--dplus-dark-bgc-chatmsg-hover: hsla(0, 0%, 0%, 0.82);
	--dplus-dark-bgc-popout: hsla(0, 0%, 0%, 0.75);
	--dplus-dark-bgc-button: hsla(0, 0%, 15%, 0.50);
	--dplus-dark-bgc-button-hover: hsla(0, 0%, 20%, 0.60);
	--dplus-dark-bgc-server-button: hsla(0, 0%, 15%, 0.50);
	--dplus-dark-bgc-server-button-hover: hsla(0, 0%, 20%, 0.60);
	--dplus-light-bgc-ui-base: hsla(0, 0%, 97%, 0.88);
	--dplus-light-bgc-ui-base-hover: hsla(0, 0%, 100%, 0.90);
	--dplus-light-bgc-ui-card: hsla(0, 0%, 93%, 0.75);
	--dplus-light-bgc-ui-card-hover: hsla(0, 0%, 50%, 0.25);
	--dplus-light-bgc-chatmsg: hsla(0, 0%, 97%, 0.88);
	--dplus-light-bgc-chatmsg-hover: hsla(0, 0%, 100%, 0.90);
	--dplus-light-bgc-popout: hsla(0, 0%, 100%, 0.80);
	--dplus-light-bgc-button: hsla(0, 0%, 50%, 0.80);
	--dplus-light-bgc-button-hover: hsla(0, 0%, 40%, 0.50);
	--dplus-light-bgc-server-button: hsla(0, 0%, 95%, 0.75);
	--dplus-light-bgc-server-button-hover: hsla(0, 0%, 100%, 1);
}

	/* Apply to corresponding theme */
	/* any values explicitly defined here are not meant to be changed by users */
.theme-dark {
	--dplus-bgc-ui-base: var(--dplus-dark-bgc-ui-base);
	--dplus-bgc-ui-base-hover: var(--dplus-dark-bgc-base-hover);
	--dplus-bgc-ui-card: var(--dplus-dark-bgc-ui-card);
	--dplus-bgc-ui-card-hover: var(--dplus-dark-bgc-ui-card-hover);
	--dplus-bgc-chatmsg: var(--dplus-dark-bgc-chatmsg);
	--dplus-bgc-chatmsg-hover: var(--dplus-dark-bgc-chatmsg-hover);
	--dplus-bgc-popout: var(--dplus-dark-bgc-popout);
	--dplus-bgc-button: var(--dplus-dark-bgc-button);
	--dplus-bgc-button-hover: var(--dplus-dark-bgc-button-hover);
	--dplus-bgc-server-button: var(--dplus-dark-bgc-server-button);
	--dplus-bgc-server-button-hover: var(--dplus-dark-bgc-server-button-hover);
	--dplus-bgc-radiobar-hover: hsla(0, 0%, 15%, 0.50);
	--dplus-bgc-radiobar-selected: hsla(0, 0%, 20%, 0.60);
}
.theme-light {
	--dplus-bgc-ui-base: var(--dplus-light-bgc-ui-base);
	--dplus-bgc-ui-base-hover: var(--dplus-light-bgc-base-hover);
	--dplus-bgc-ui-card: var(--dplus-light-bgc-ui-card);
	--dplus-bgc-ui-card-hover: var(--dplus-light-bgc-ui-card-hover);
	--dplus-bgc-chatmsg: var(--dplus-light-bgc-chatmsg);
	--dplus-bgc-chatmsg-hover: var(--dplus-light-bgc-chatmsg-hover);
	--dplus-bgc-popout: var(--dplus-light-bgc-popout);
	--dplus-bgc-button: var(--dplus-light-bgc-button);
	--dplus-bgc-button-hover: var(--dplus-light-bgc-button-hover);
	--dplus-bgc-server-button: var(--dplus-light-bgc-server-button);
	--dplus-bgc-server-button-hover: var(--dplus-light-bgc-server-button-hover);
	--dplus-bgc-radiobar-hover: hsla(0, 0%, 92%, 0.70);
	--dplus-bgc-radiobar-selected: hsla(0, 0%, 80%, 0.60);
}

/* Blur */
:root {
	--dplus-blur-ui: 2px;
	--dplus-blur-popout: 3px;
	--blurcalc-popout: blur(calc(var(--dplus-blur-popout) / 100 * var(--dplus-blur-scale)));
	--blurcalc-ui: blur(calc(var(--dplus-blur-ui) / 100 * var(--dplus-blur-scale)));
}


/* Discord's variables */
body {
	--brand-color: var(--dplus-accent-ui);
	--brand-color-hover:  var(--dplus-accent-ui-hover);
}
.theme-dark, .theme-light {
	--background-primary: var(--dplus-bgc-ui-base) !important;
	--background-secondary: var(--dplus-bgc-ui-card) !important;
	--background-tertiary: transparent !important; /* if this is not transparent, background breaks */
	--background-secondary-alt: transparent ! important; /* bottom-left account details */
	--channelbodyarea-background: transparent !important;
	--background-floating: var(--dplus-bgc-popout) !important;
	--radio-group-dot-foreground: white;
	--brand-experiment: var(--dplus-accent-ui); /* remove the weird new branding colour with a much better accent colour */
}

.theme-dark {
	--bd-blue: var(--dplus-accent-ui) !important;
	--background-accent: var(--dplus-accent-ui);
}

.theme-light {
	--background-secondary:	hsla(0, 0%, 97%, 0.88) !important;
	--header-primary: #060607;
	--header-secondary: #4f5660;
	--text-normal: #000;
	--text-muted: #747f8d;
	--text-link: #0067e0;
  --channels-default: #1f1f1f;
  --interactive-normal: #1f1f1f;
	--interactive-hover: #2e3338;
	--interactive-active: black;
	--interactive-muted: #8f99a3;
	--bd-blue: var(--dplus-accent-ui) !important;
	--background-accent: var(--dplus-accent-ui);
}


/* Quick and dirty fix for create a new server in dark mode */
.theme-dark .layer-2KE1M9 .theme-light { /* the ones i actually need */
	--header-primary: #060607;
	--header-secondary: #4f5660;
	--text-normal: #2e3338;
	--interactive-normal: #4f5660;
}


/* Background image */
#app-mount {
	background: var(--dplus-background) !important;
	background-size: cover !important;
	background-position: center !important;
}
html { background-color: var(--dplus-accent-ui); }


/* Fonts */
	/* Display font */
:root {
	--font-display: var(--dplus-font-ui), 'Poppins', var(--dplus-font-ui-ru), 'Comfortaa', var(--dplus-font-ui-vi), 'Raleway', var(--dplus-font-ui-ja), 'Kosugi',  var(--dplus-font-ui-ko), 'Gothic A1', var(--dplus-font-ui-el), 'Commissioner', '-apple-system', 'Helvetica Neue', 'system-ui', 'Tahoma', 'Segoe UI', 'Helvetica', 'Whitney', sans-serif !important;
	--font-primary: var(--font-display);
	--font-japanese: var(--font-display);
	--font-korean: var(--font-display);
	--font-chinese-simplified: var(--font-display);
	--font-chinese-traditional: var(--font-display);
}
body, button, select {
	font-family: var(--font-display);
}

	/* Text font */
::placeholder, ::-webkit-input-placeholder, p, bodyarea, input, select, textarea,
.message-2qnXI6, .markup-2BOw-j, /*chat messages*/
.subText-1KtqkB, /*member list body*/
.customStatusText-2opeSw, /*user's custom status*/
.modeDefault-3a2Ph1, /*settings small body*/
.emojiInput-1aLNse, .emojiAliasPlaceholder-3H_iZA, /*server settings: emoji name*/
.topic-TCb_qw, /*channel topic in chat header*/
.content-38qMG0, /*channel topic popup body*/
.bd-description /*BD: plugin/theme desc*/ {
	font-family: var(--dplus-font-body), 'Roboto', '-apple-system', 'Helvetica Neue', 'system-ui', 'Arial', 'Helvetica', 'Whitney', sans-serif !important;
}

	/* Names, titles, and headers font */
header, h1,
.nameAndDecorators-5FJ2dg, /*name in member list*/
.headerNameWrapper-3res2c, /*nickname in profile popup*/
.username-1A8OIy, /*username in chat*/
.headerText-15Q25Z, /*username#tag in profile popup*/
.nickname-2gQ76l, /*nickname in profile popup*/
.nameTag-3uD-yy, /*your username in the bottom-left*/
.detailsInner-1VPlWl, /*settings: your username in My Account*/
.activityName-1IaRLn, /*user's activity name, includes song and author titles*/
.emojiUploader-1f0pVx, /*server settings: emoji's uploader*/
.userHook-3AdCBF, /*server settings: username in audit log*/
.secondaryHeader-2oeRPO, /*server settings: integrations row headers such as bot names*/
.roleName-32vpEy, /*role name in profile*/
.roleName-1vjSQR, .roleName-2IkRdr, /*role name in server settings*/
.membersGroup-v9BXpm, /*role name in member list*/
.roleRow-1iQo_1, /*role name in context menu*/
.roleMention-2Bj0ju, /*role name mention in chat*/
.wrapper-3WhCwL, /*username or channel name mention in chat*/
[data-slate-object="inline"] .mention, /*mention in message box*/
.systemMessage-1I9LCe .anchorUnderlineOnHover-2ESHQB, /* links / usernames in system messages */
.name-3l27Hl, /*category name in sidebar*/
.name-23GUGE, /*channel name in sidebar*/
.title-29uC1r, /*channel name in chat header*/
.title-3sZWYQ, /*channel name in channel topic popup*/
.bd-author, .bd-meta .bd-link, /*BD: plugin/theme author*/
.timestamp-3ZCmNB /*chat message hover timestamp (counts as a header)*/ {
	font-family: var(--dplus-font-header), 'Righteous', var(--dplus-font-header-ja), 'RocknRoll One', var(--dplus-font-header-ko), 'Black Han Sans', var(--dplus-font-header-ru), 'Russo One', var(--dplus-font-header-hi), 'Palanquin Dark', var(--dplus-font-header-th), 'Mitr', var(--dplus-font-header-el), 'Alegreya Sans', 'Lalezar', 'Century Gothic', 'Franklin Gothic Medium', 'Britannic', 'Helvetica Neue', 'Helvetica', 'Whitney', sans-serif !important;
}

/* App margins */
.app-2rEoOp, .app-1q1i1E {
	left:		calc(var(--dplus-spacing-app) - 5px) !important;
	top:		calc(var(--dplus-spacing-app) - 5px) !important;
	right:	calc(var(--dplus-spacing-app) + 5px) !important;
	bottom:	calc(var(--dplus-spacing-app) + 5px) !important;
}

/* Loading page (disconnect error) */
.container-16j22k { background-color: hsla(0, 0%, 0%, 0.68) }
.quote-3aooyW {
	font-size: 20px !important;
	margin-bottom: 0px !important;
}
.status-1JTY3j, .problemsText-1Yx-Kl {
	color: white;
	text-transform: none;
	font-size: 16px !important;
}
.attribution-aTC3hS, .links-3Ldd4A {
	font-size: 0px !important;
}
.twitterLink-3NsWMp:before,
.statusLink-gFXhrL:before {
	background-size: 24px 24px;
	height: 24px;
	width: 24px;
}

/* Crash error */
.errorPage-u8SYh4 {
	width: calc(100% - var(--dplus-spacing-app) * 2)
}
.wrapper-1prNyd {
	min-height: calc(100vh - var(--dplus-spacing-app) * 2)
}

.theme-dark .wrapper-1prNyd,
.theme-light .wrapper-1prNyd {
	background: var(--dplus-bgc-ui-base);
	margin: var(--dplus-spacing-app) calc(var(--dplus-spacing-app) * 2) var(--dplus-spacing-app) var(--dplus-spacing-app);
	border-radius: var(--dplus-radius-ui);
}

.theme-dark .image-3zK3Wt,
.theme-light .image-3zK3Wt {
	background-image: url('https://cdn.discordapp.com/attachments/560369937084973067/853659649340473414/28.webp')
}
.image-3zK3Wt {
    width: 256px;
    height: 256px;
    margin-bottom: 40px;
    background-size: 256px 256px;
}

.title-3trS3_,
.note-450gs3 div p {
	font-size: 0px;
}

.title-3trS3_:after {
	font-size: 24px;
	content: "Congratulations!";
}

.note-450gs3 div p:first-child:after {
	font-size: 16px;
	content: "You just unlocked Discord Minus!";
	color: white;
}
.note-450gs3 div p:nth-child(2):after {
	font-size: 16px;
	content: "...actually, Discord just crashed. Oops."
}

/* Scrollbar */
.theme-dark ::-webkit-scrollbar-track-piece,
.theme-dark .theme-light ::-webkit-scrollbar-track-piece,
.theme-light .theme-dark ::-webkit-scrollbar-track-piece {
  background:  hsla(0,0%,0%,0.3)!important;
}
.theme-light ::-webkit-scrollbar-track-piece {
  background:  hsla(0,0%,100%,0.3)!important;
  border: none!important;
}
::-webkit-scrollbar-thumb {
  background: var(--dplus-accent-ui)!important;
  border: none!important;
  border-radius: var(--dplus-radius-ui);
}
::-webkit-scrollbar {
  width: var(--dplus-scrollbar-width) !important;
}
.scroller-2TZvBN::-webkit-scrollbar, .scroller-1Bvpku::-webkit-scrollbar {
	width: 0!important;
}
::-webkit-scrollbar-track {
  background: transparent!important;
  border: none!important;
}


/* Modals */
.root-1gCeng {
	background-color: var(--dplus-bgc-popout) !important;
	border-radius: var(--dplus-radius-ui) !important; 
	backdrop-filter: var(--blurcalc-popout);
}
#app-mount .footer-2gL1pp {
	background-color: transparent;
	box-shadow: none;
}
iframe {
	border-radius: var(--dplus-radius-ui);
}
.modal-yWgWj- {background-color: transparent; box-shadow: none;}
.backdrop-1wrmKB, .backdropWithLayer-3_uhz4 {
	background-color: rgba(0, 0, 0, 0.6) !important;
	backdrop-filter: var(--blurcalc-ui);
}

	/* Create/Join Server Modal */
.theme-dark .theme-light .root-1gCeng {background: var(--dplus-bgc-popout) !important;}
.theme-dark .theme-light .container-UC8Ug1 {background: var(--dplus-bgc-ui-card);}
.filledIcon-2eb7eA { border-radius: var(--dplus-radius-ui); }
.container-UC8Ug1:hover {background: var(--dplus-bgc-ui-card-hover) !important;}
.theme-dark .theme-light {
	--header-primary: #fff;
	--header-secondary: #b9bbbe;
	--text-normal: #dcddde;
	--text-muted: #72767d;
	--text-link: #00b0f4;
	--channels-default: #8e9297;
	--interactive-normal: #b9bbbe;
	--interactive-hover: #dcddde;
	--interactive-active: #fff;
	--interactive-muted: #4f545c;
}
.header-3msK0M {overflow: hidden;}

.optionContainer-15srkc {
	background-color: var(--dplus-bgc-ui-card);
}
.optionContainer-15srkc:hover {
	background-color: var(--dplus-bgc-ui-card-hover);
}

	/* Custom status modal */
.input-cIJ7To.focused-1mmYsC, .input-cIJ7To:focus, .lookFilled-1h1y05.select-1Pkeg4:focus,
.lookFilled-1h1y05.select-1Pkeg4:hover.selectOpen-hQuR6b, .lookFilled-1h1y05.selectOpen-hQuR6b {border-color: var(--dplus-accent-ui);}

	/* Quick switcher modal */
#app-mount .quickswitcher-3JagVE {
	background-color: var(--dplus-bgc-popups);
	box-shadow: none;
	height: 300px;
}
.container-3qKHyN {height: auto;}

	/* Keyboard Combos modal*/
#app-mount .keyboardShortcutsModal-3piNz7 {background-color: transparent;}
#app-mount .keybindShortcut-1BD6Z1 span {background-color: var(--dplus-accent-ui); border-color: black;}

	/* Region select modal */
.regionSelectModal-12e-57 {
	background: transparent;
}
	/* Pin message modal */
#app-mount .message-2qRu38 {
	background-color: var(--dplus-bgc-chatmsg);
	border-radius: var(--dplus-radius-ui);
	border: 1px solid var(--dplus-accent-ui);
	box-shadow: none;
	padding: 0;
	min-height: 70px;
}
	/* Upload modal */
.uploadModal-2ifh8j { background-color: var(--dplus-bgc-ui-base) !important; }
.uploadModal-2ifh8j, #app-mount .footer-3mqk7D {
	border-radius: var(--dplus-radius-ui) !important;
	box-shadow: none;
}
.uploadModal-2ifh8j, .uploadModal-2ifh8j .channelbodyArea-2VhZ6z {	border: 2px dashed var(--dplus-accent-ui); }
.footer-3mqk7D { background-color: var(--dplus-bgc-ui-base) !important; }


/* Popouts */
.layer-v9HyYc > div > div:not(.tooltipPointer-3ZfirK) {
	background-color: var(--dplus-bgc-popout);
	border-radius: var(--dplus-radius-ui);
}

.popouts-2bnG9Z {
    z-index: 1000 !important;
}

	/* Context menu */
.scroller-3BxosC, .submenuPaddingContainer-fiOCHc {
	padding: 0;
}
.scroller-3BxosC::-webkit-scrollbar, .submenuPaddingContainer-fiOCHc::-webkit-scrollbar {
	width: 0 !important;
}
.submenuPaddingContainer-fiOCHc {margin-right: -4px;margin-left: -4px;} /* fixes the submenu being four pixels off */

.labelContainer-1BLJti {
	padding: calc(var(--dplus-spacing-ui) / 1.25) var(--dplus-spacing-ui);
}

.item-1tOPte:not([aria-haspopup="true"]),
.item-1tOPte[aria-haspopup="true"],
.wrapper-3_530D,
.separator-2I32lJ { backdrop-filter: var(--blurcalc-popout) }
/* the context menu backdrop blur has to be applied separately for elements
that have popups, or else the menu breaks when you hover over them */

.wrapper-3_530D { padding: 0; }
.customItem-a8hq58 .button-38aScr { padding: calc(var(--dplus-spacing-ui) / 2); }
.separator-2I32lJ { margin: 0; }

.item-1tOPte,
.button-38aScr {
	border-radius: var(--dplus-radius-ui);
}
.item-1tOPte {
	margin: 0;
	transition: background-color var(--dplus-anim-button);
}

.button-38aScr:not(.lookBlank-3eh9lL):not(.lookLink-9FtZy-):not(.lookOutlined-3sRXeN):not(.colorRed-1TFJan):not(.colorWhite-rEQuAQ), /* non-special buttons */
.colorDefault-2K3EoJ:not(.labelContainer-1BLJti) /* regular buttons, except context menu */ {
	background-color: var(--dplus-bgc-button);
	transition: var(--dplus-anim-button);
}

[id^="status-picker-"] /* status picker (who would've guessed?) */ {
	background-color: transparent !important;
}

.button-38aScr:not(.lookBlank-3eh9lL):not(.lookLink-9FtZy-):not(.lookOutlined-3sRXeN):not(.colorRed-1TFJan):not(.colorWhite-rEQuAQ):hover, /* buttons hovered over */
.button-38aScr.focused-3ZzkKr, /* focused but not hovered over */
.colorDefault-2K3EoJ:not(.labelContainer-1BLJti).focused-3afm-j, /* regular buttons, focused */
.colorDefault-2K3EoJ:hover:not(.labelContainer-1BLJti):not(.hideInteraction-1iHO1O) /* regular buttons but only if clickable */ {
	background-color: var(--dplus-bgc-button-hover);
	transition: var(--dplus-anim-button);
}
.lookFilled-1Gx00P.colorBrand-3pXr91, /* branded buttons */
.labelContainer-1BLJti:hover, /* context menu buttons */
[id^="status-picker-"]:hover /* status picker hovered */  {
	background-color: var(--dplus-accent-ui) !important;
}
.lookFilled-1Gx00P.colorBrand-3pXr91:hover, /* branded buttons, hovered over */
.labelContainer-1BLJti.focused-3afm-j:not(:hover), /* context menu button w/ submenu */
.colorDefault-2K3EoJ:active:not(.hideInteraction-1iHO1O) /* status picker drag-click */ {
	background-color: var(--dplus-accent-ui-hover) !important;
}


.item-1tOPte.colorDanger-2qLCe1:hover {background-color: #f04747;}

	/* Profile Popout */
.root-SR8cQa {
	background-color: transparent;
	backdrop-filter: var(--blurcalc-popout);
}

.headerNormal-1mX3KY,
.body-3HBlXn,
.bodyInnerWrapper-26fQXj {
	background-color: transparent;
}

.headerTop-2cWpdB {
	background-color: var(--dplus-bgc-ui-card);
}

.translate-2dAEQ6,
.popout-2iWAc- {
	backdrop-filter: var(--blurcalc-popout);
}
.userPopout-xaxa6l {
	background-color: var(--dplus-bgc-popout);
	border-radius: var(--dplus-radius-ui);
	box-shadow: none !important;
}

.avatarPositionNormal-aZjAsn {
	left: var(--dplus-spacing-ui);
}

/* this link doesn't do much other than take up space */
.setIdentityLink-1t8Ahd {
	display: none;
}

.customStatus-oN4ZZY {
	padding-top: var(--dplus-spacing-ui)
}

.avatarWrapper-3r9PdD:before {
	content: "";
	position: absolute;
	width: 100%;
	height: 100%;
	z-index: 0;
	background-color: var(--dplus-bgc-ui-card);
	backdrop-filter: var(--blurcalc-ui);
	border-radius: var(--dplus-radius-avatar);
	clip: rect(auto,auto,44px,auto);
}

.avatar-37jOim {
	border-width: 6px;
	border-style: solid;
	border-color: transparent;
	border-radius: var(--dplus-radius-ui);
	background-color: transparent;
}

.userPopout-xaxa6l .wrapper-3t9DeA:not(.baseAvatar-3Nvk7n),
.container-3RCQyg .wrapper-3t9DeA,
.avatarUploaderInner-2EvNMg,
.avatarHint-2A3RNb {
	width: var(--dplus-icon-avatar-profile) !important;
	height: var(--dplus-icon-avatar-profile) !important;
}

.assetsLargeImage-eYwpTX {
	border-radius: var(--dplus-radius-ui);
}

	/* Profile modal */
.avatar-AvHqJA {
	width: calc(var(--dplus-icon-avatar-profile) * 1.5) !important;
	height: calc(var(--dplus-icon-avatar-profile) * 1.5) !important;
	border-radius: var(--dplus-radius-avatar);
	border-width: 8px;
	border-style: solid;
	border-color: transparent;
	background-color: transparent;
}

.avatar-AvHqJA:before {
	content: "";
	position: absolute;
	width: 100%;
	height: 100%;
	right: -8px;
	top: -8px;
	border-width: 8px;
	border-style: solid;
	border-color: transparent;
	background-color: var(--dplus-bgc-popout);
	border-radius: calc(var(--dplus-radius-avatar) + 5px);
	clip: rect(auto,auto,68px,auto);
}

.top-28JiJ- .item-PXvHYJ {
	border-radius: 0 !important;
}

.listRow-hutiT_ {
margin: var(--dplus-spacing-ui);
padding: var(--dplus-spacing-ui);
}
.listRow-hutiT_ .iconInactive-98JN5i {
	border-radius: var(--dplus-radius-server);
	width: var(--dplus-icon-server-list);
	height: var(--dplus-icon-server-list);
}
.listAvatar-1NlAhb {
	margin-right: var(--dplus-spacing-ui);
}
.body-r6_QPy, .topSection-y3p-_D {
	background-color: transparent;
}

.aboutMeSection---MkQa {
	background-color: transparent;
}

.nickname-322DbL {
	font-family: inherit;
}

.disabledButtonWrapper-3wH6-b { display: none; /* Remove Spotify buttons for yourself */ }
.button-2IFFQ4 { margin-top: var(--dplus-spacing-ui); }

[style="background-color: rgb(114, 137, 218);"] {
	background-color: var(--dplus-accent-ui) !important;
}
.theme-dark .path-92Hmty,
.theme-light .path-92Hmty {
    stroke: var(--dplus-accent-ui) !important;
}

.activity-fViXj7 {
	border-bottom: 0;
}

	/* Roles */
.role-2irmRk {
	border-radius: var(--dplus-radius-ui);
	position: relative;
	overflow: hidden;
}
.roleCircle-3xAZ1j::after {
	content: "";
	background: inherit;
	height: 24px; width: 100%;
	position: absolute;
	left: 0;
	opacity: 0.72;
	z-index: -1;
}

	/* Tooltips */
.tooltip-2QfLtc {
	backdrop-filter: var(--blurcalc-popout);
}
.tooltipContent-bqVLWK {
	padding: var(--dplus-spacing-ui);
	background-color: transparent !important;
}

	/* Search */
.search-2oPWTC .searchBar-3dMhjb {
	transition-duration: var(--dplus-anim-short);
}
#app-mount .container-3ayLPN {
	background-color: var(--dplus-bgc-popout);
	border-radius: var(--dplus-radius-ui);
	width: 404px!important;
	margin-left: -68px;
}
#app-mount .option-96V44q.selected-rZcOL- {
	background-color: var(--dplus-accent-ui);
	border-radius: var(--dplus-radius-ui);
}
#app-mount .searchAnswer-3Dz2-q, #app-mount .searchFilter-2ESiM3,  #app-mount .jumpButton-JkYoYK {
	background-color: var(--dplus-accent-ui)!important;
	color: white;
}
.channelName-1JRO3C {
	background: var(--dplus-accent-ui);
	color: white;
	border-radius: var(--dplus-radius-ui);
	padding: 8px;
	opacity: 0.6;
}
.content-1x5b-n {
	margin-left: 0;
	margin: 0 var(--dplus-spacing-ui);
	padding: 0 calc(var(--dplus-spacing-ui) / 2);
	border-radius: var(--dplus-radius-ui);
}
.channelSeparator-1DOiGt:before {
	background-color: var(--dplus-accent-ui);
	opacity: 0.3;
}
.searchResult-9tQ1uo.expanded-w_LCGl {
	border: 1px solid var(--dplus-accent-ui) !important;
	border-radius: var(--dplus-radius-ui) !important;
}
.searchResultMessage-1fxgXh, #app-mount .option-96V44q:after, .searchResult-9tQ1uo:after, .searchResult-9tQ1uo:before {
	background: none;
	border: none !important;
	border-radius: var(--dplus-radius-ui) !important;
	box-shadow: none !important;
}
.search-2oPWTC .searchBar-3dMhjb, .queryContainer-RKFJW-.focused-2bY0OD {
  background: var(--dplus-bgc-ui-base);
}
#app-mount .searchResultMessage-1fxgXh.sibling-1eJVjd {
  opacity: .3;
  filter: blur(calc(var(--blur-small) / 100 * var(--dplus-blur-scale)));
}
#app-mount .elevationBorderHigh-2WYJ09 {box-shadow: none;}

	/* Calendar picker */
#app-mount .calendarPicker-2yf6Ci .react-datepicker {
	background-color: var(--dplus-bgc-ui-base) !important;
	margin-left: 46px;
}
#app-mount .calendarPicker-2yf6Ci .react-datepicker__day:not(.react-datepicker__day--disabled):hover,
#app-mount .calendarPicker-2yf6Ci .react-datepicker__day.react-datepicker__day--selected:after,
#app-mount .datePicker--XZbmJ .datePickerHint-3Q1Udw .hintValue-29ny8Z {
	background-color: var(--dplus-accent-ui) !important;
}
#app-mount .calendarPicker-2yf6Ci .react-datepicker__day {
	border-color: black !important;
}
#app-mount .calendarPicker-2yf6Ci div {
	background-color: transparent !important;
}
.react-datepicker__day {
	transition: var(--dplus-anim-short);
}

	/* Pinned messages Popout */
.messagesPopoutWrap-1MQ1bW {
	width: calc(440px + var(--dplus-icon-avatar-chat) + var(--dplus-spacing-ui));
}
.header-ykumBX { padding: var(--dplus-spacing-ui); }
.messagesPopoutWrap-1MQ1bW {
	background-color: transparent !important;
	border: none !important;
	max-height: 560px !important;
	backdrop-filter: var(--blurcalc-popout);
}
.messageGroupWrapper-o-Zw7G {
	border-radius: var(--dplus-radius-ui);
	min-height: 70px;
	background: transparent;
}
.messageGroupWrapper-o-Zw7G .cozy-3raOZG.wrapper-2a6GCs {
	padding-top: var(--dplus-spacing-ui);
	padding-bottom: var(--dplus-spacing-ui);
}

.messagesPopout-24nkyi .messageGroupWrapper-o-Zw7G .wrapper-2a6GCs {
	background-color: var(--dplus-bgc-ui-card) !important;
}
.messagesPopout-24nkyi .messageGroupWrapper-o-Zw7G:hover .wrapper-2a6GCs {
	background-color: var(--dplus-bgc-ui-card-hover) !important;
}
.messagesPopoutWrap-1MQ1bW .messagesPopout-24nkyi .wrapper-2a6GCs {
	transition: background-color var(--dplus-anim-short);
}


/* Inbox */
.container-enaOkj {background-color: transparent;}


/* Autocomplete */
.autocomplete-1vrmpx {
	background-color: var(--dplus-bgc-popout) !important;
	border-radius: var(--dplus-radius-ui);
}
#app-mount .selected-1Tbx07 {background-color: var(--dplus-accent-ui);}


/* Emoji/GIF/Sticker Picker */
.result-3w1ZcL, .wrapper-1-Fsb8 {
	background-color: var(--dplus-accent-ui)!important;
	border-radius: var(--dplus-radius-ui);
}
#app-mount .focused-1En8bG:after, .theme-dark .result-3w1ZcL:hover:after {
    box-shadow: inset 0 0 0 2px var(--dplus-accent-ui), inset 0 0 0 3px #2f3136;
}
.scroller-3gAZLs::-webkit-scrollbar {
  width: calc(var(--dplus-scrollbar-width) / 2) !important;
}

/* Light theme stuff */
.theme-light .emoji, .theme-light .emoji.jumboable {
  filter: drop-shadow(0 0 1px #00000055);
}

.bd-pfbtn,
.bda-settings-button,
.wrapper-232cHJ,
.rtc-connection-status {
	padding-bottom: 2px;
}


/* Windows titlebar */
.typeWindows-1za-n7 {
	background-color: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui);
	height: 20px;
	padding-bottom: 4px;
	margin-right: calc(var(--dplus-spacing-app) * 2);
	position: relative;
	left: var(--dplus-spacing-app);
	align-items: center;
}
.withFrame-haYltI {
	margin-top: var(--dplus-spacing-app);
}
.wordmark-2iDDfm svg {display: none;}
.winButton-iRh8-Z {
	height: 24px;
	top: 2px;
}
.winButtonClose-1HsbF- {
	border-radius: 0 10px 10px 0;
}
.wordmark-2iDDfm {
	display: block;
	background: no-repeat url(https://plusinsta.xyz/discord-plus/assets/wordmark_white.svg);
	background-size: 65px 16px;
	background-position: 6px 4px !important;
	height: 16px; width: 65px;
	opacity: 0.6;

}
.theme-light .wordmark-2iDDfm {filter: brightness(0);}
.theme-light .theme-dark .wordmark-2iDDfm {filter: none;}

/* macOS window buttons */
.typeMacOS-3EmCyP {
	margin-left: 10px;
	margin-top: 10px;
	background: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui);
}
.platform-osx .wrapper-1Rf91z {
	margin-top: 0px !important;
	padding-top: 32px;
}

/* Sidebar */
	/* Servers */
		/* Home Icon */
.platform-win .scroller-1Bvpku {
	padding-top: var(--dplus-spacing-ui);
}
.homeIcon-AaowEC {display: none !important;}
.wrapper-1BJsBx.selected-bZ3Lue .childWrapper-anI2G9,
.wrapper-1BJsBx:hover .childWrapper-anI2G9 {
	background-color: transparent;
}
.theme-dark .tutorialContainer-11ICd5 .childWrapper-anI2G9,
.theme-light .theme-dark .tutorialContainer-11ICd5 .childWrapper-anI2G9,
.theme-light .tutorialContainer-11ICd5 .childWrapper-anI2G9 {
	background-image: var(--dplus-icon-home-dark);
	background-repeat: no-repeat;
	background-size: cover;
	background-position: center;
}

.theme-light .tutorialContainer-11ICd5 .childWrapper-anI2G9 {
	background-image: var(--dplus-icon-home-light);
}

		/* Server list */
.guilds-1SWlCJ foreignObject {mask: none;}
.guildSeparator-3s64Iy, .guildSeparator-33mFX6 {display: none}
.folder-1hbNCn {background-color: transparent;}
.folder-1hbNCn.hover-qTxTR_ {background-color: var(--dplus-bgc-server-button-hover)}
#app-mount .childWrapper-anI2G9, #bd-pub-button {background-color: var(--dplus-bgc-server-button);}
#bd-pub-button { border-radius: var(--dplus-radius-ui); }
#app-mount .guilds-1SWlCJ {
	background: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui);
}
.guilds-1SWlCJ, .listItem-GuPuDH, .listItem-1hlISG, .wrapper-3Njo_c {
	width: calc(var(--dplus-icon-server-sidebar) + var(--dplus-spacing-ui) * 2)
}
.listItem-GuPuDH, .listItem-1hlISG {
	margin: 0 0 var(--dplus-spacing-ui);
}
.svg-1X37T1, .wrapper-25eVIn {
	width: var(--dplus-icon-server-sidebar);
	height: var(--dplus-icon-server-sidebar);
}
.scroller-1Bvpku {
	padding: var(--dplus-spacing-ui) 0 0;
}
.expandedFolderBackground-1cujaW {
	width: var(--dplus-icon-server-sidebar);
	border-radius: var(--dplus-radius-ui);
	left: var(--dplus-spacing-ui);
	bottom: 0;
	background: var(--dplus-bgc-server-button);
}
.wrapper-3Njo_c ul {
	height: calc(inherit + var(--dplus-spacing-ui)) !important;
}

.listItem-2q53zr :not(span), .listItem-2Ig28I :not(span) {border-radius: var(--dplus-radius-server);}
.item-2hkk8m[style="opacity: 1; height: 40px; transform: none;"], .wrapper-sa6paO { height: calc(var(--dplus-icon-server-sidebar) / 10 * 8) !important; }
.pill-1z4sAY { top: calc(var(--dplus-icon-server-sidebar) / 10) }

.expandedFolderBackground-2sPsd- {border-radius: var(--dplus-radius-ui);}
.circleIconButton-1QV--U {
	background-color: var(--dplus-bgc-server-button);
	color: var(--dplus-accent-ui);
}
.circleIconButton-1QV--U {
	transition: color, background-color;
	transition-duration: var(--dplus-anim-button);
	transition-timing-function: ease-out;
}
.circleIconButton-1QV--U.selected-1JjBPm,
#app-mount .childWrapper-anI2G9:hover,
#bd-pub-button:hover {
	background-color: var(--dplus-bgc-server-button-hover);
}

.circleIconButton-1QV--U.selected-1JjBPm {
	color: var(--dplus-accent-ui);
}

		/* Server Discovery */
.scroller-1d5FgU { padding: 16px !important; }
.pageWrapper-1PgVDX { background-color: var(--dplus-bgc-ui-base) !important; }
#app-mount .guildIcon-3W0pfo {
	background-color: var(--dplus-accent-ui);
	border-radius: var(--dplus-radius-ui);
}
.card-3DjzTQ {
	background-color: var(--dplus-bgc-ui-card) !important;
}
.card-3DjzTQ:hover {
	background-color: var(--dplus-bgc-ui-card-hover) !important;
}
.categoryPill-34fszg.selected-1dONk0 {
	background-color: var(--dplus-accent-ui);
}

		/* Server Boost */
.root-3R2ngo {
	border-radius: var(--dplus-radius-ui);
	margin: var(--dplus-spacing-app);
	margin-top: calc(var(--dplus-spacing-app) * 2 + 24px);
}
#app-mount .perksModal-fSYqOq, #app-mount .tierBody-16Chc9, #app-mount .perk-2WeBWW {background-color: var(--dplus-bgc-ui-base);}
#app-mount .tierHeaderLocked-1s2JJz {
	background-color: var(--dplus-accent-ui);
	color: var(--text-muted);
}

	/* Channel list */
.sidebar-2K8pFh,
.bannerImage-3KhIJ6 {
	width: var(--dplus-channels-width);
}

.scroller-1JbKMe, .privateChannels-1nO12o, .container-3w7J-x {background: transparent;}
.sidebar-2K8pFh {
	background: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui) !important;
	margin: 0 var(--dplus-spacing-app);
}
.layout-2DM8Md, .content-3at_AU {
	padding: 0 calc(var(--dplus-spacing-ui) / 2) !important;
	border-radius: var(--dplus-radius-ui);
}

.privateChannelsHeaderContainer-3NB1K1 {
	padding: var(--dplus-spacing-ui);
	margin: calc(var(--dplus-spacing-ui) / 2);
}

.privateChannelRecipientsInviteButtonIcon-3A3uTc {
	margin-right: 0;
}

.privateChannelsHeaderContainer-3NB1K1 {height: min-content;}
.headerText-2F0828, .container-2ax-kl {text-transform: none;}
.privateChannels-1nO12o .channel-2QD9_O {margin: var(--dplus-spacing-ui);}
.closeButton-2GCmT5 {
	display: block;
	opacity: 0;
	margin-right: calc(var(--dplus-spacing-ui) - var(--dplus-spacing-ui) * 1.5);
}

.closeButton-2GCmT5 {
	transition: var(--dplus-anim-button-appear);
}

.channel-2QD9_O:hover .closeButton-2GCmT5 {
	opacity: 0.6;
	margin-right: 0;
}
.menu-3sdvDG {
	border-radius: var(--dplus-radius-ui);
	background: transparent;
}
		/* Animated channel buttons */
.iconItem-F7GRxr {
	display: block !important;
}
.iconVisibility-sTNpHs .children-3rEycc {
	margin-right: calc(0px - var(--dplus-spacing-ui));
}
.iconVisibility-sTNpHs .iconItem-F7GRxr {
	opacity: 0;
	z-index: 1;
}

.containerDefault--pIXnN.selected-3LIHYU .children-3rEycc,
.iconVisibility-sTNpHs:hover .children-3rEycc {
margin-right: 0;
}
.containerDefault--pIXnN.selected-3LIHYU .iconItem-F7GRxr,
.iconVisibility-sTNpHs:hover .iconItem-F7GRxr {
	opacity: 1;
}

.iconVisibility-sTNpHs .children-3rEycc,
.iconVisibility-sTNpHs .iconItem-F7GRxr,
.iconVisibility-sTNpHs .userLimit-3aerPX,
.iconVisibility-sTNpHs:hover .wrapper-2tAnRe {
	transition-duration: var(--dplus-anim-button-appear);
}

		/* User limit */
.containerDefault--pIXnN.selected-3LIHYU .userLimit-3aerPX, .iconVisibility-sTNpHs:focus-within .userLimit-3aerPX, .iconVisibility-sTNpHs:focus .userLimit-3aerPX, .iconVisibility-sTNpHs:hover .userLimit-3aerPX {
	display: block;
}
.wrapper-2tAnRe {
	border-radius: var(--dplus-radius-ui);
	margin-right: var(--dplus-spacing-ui);
}
.userLimit-3aerPX .users-3kndPl {
	width: calc(15px + var(--dplus-spacing-ui));
	padding: 0 calc(var(--dplus-spacing-ui) / 2);
	background-color: var(--dplus-bgc-ui-card-hover);
}
.userLimit-3aerPX .total-i6us2n {
	width: calc(12px + var(--dplus-spacing-ui));
	padding: 0 calc(var(--dplus-spacing-ui) / 2) 0 0;
	background-color: var(--dplus-bgc-ui-card);
}
.userLimit-3aerPX .total-i6us2n:after {
  border-right-color: var(--dplus-bgc-ui-card);
}
.wrapper-2tAnRe {
	border-radius: var(--dplus-radius-ui);
	margin-right: var(--dplus-spacing-ui);
}

				/* Animate user limit */
.userLimit-3aerPX {
	opacity: 1;
	position: absolute;
}
.iconVisibility-sTNpHs:hover .wrapper-2tAnRe {
	margin-right: var(--dplus-spacing-ui);
}
.iconVisibility-sTNpHs:hover .userLimit-3aerPX {
	margin-right: -50px;
	opacity: 0;
}

/* Home */
	/* Friends List */
#app-mount .container-1D34oG, #app-mount .outer-1AjyKL {
	background-color: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui);
	overflow: hidden;
}
.nowPlayingColumn-2sl4cE, .container-1D34oG .container-1r6BKw.themed-ANHk51, .container-lRFx4q {background-color: transparent;}
.actionButton-uPB8Fs, #app-mount .inset-3sAvek,  #app-mount .separator-XqIyoz, .wrapper-3Rixsz:hover, .memberListContainer-13tNU9 div:hover {
	background-color: var(--dplus-accent-ui)!important;
	border-radius: var(--dplus-radius-ui);
}
.itemCard-v9viV7, #app-mount .outer-1AjyKL.active-1xchHY, #app-mount .outer-1AjyKL.interactive-3B9GmY:hover, #app-mount .memberListItem-31QoHj:not(.popoutDisabled-2RK7MF):hover, #app-mount .enabled-1t_Gxm:hover { background: var(--dplus-bgc-ui-base-hover);}

	/* Game Library + Nitro Tab */
.playButton-1fMNjH, .actionButtonSize-1Znp1q:hover, .rowWrapperActive-2L7i9f button {
	background-color: var(--dplus-accent-ui)!important;
}
.gameUpdates-2GPqBU {background: var(--dplus-bg-dark-2);}
#app-mount .applicationStore-1pNvnv, .header-39GIC8 {background: transparent;}
.container-3Mxszk, .applicationStore-1pNvnv {border-radius: var(--dplus-radius-ui);}


/* Chat */
.chat-3bRxxu, .wrapper-3vR61M {
	background-color: transparent;
	border-radius: var(--dplus-radius-ui);
}
.wrapper-1F5TKx, #app-mount .children-19S4PO:after {display: none;}

	/* Avatars */
.wrapper-3t9DeA foreignObject, .callAvatarMask-1SLlRi foreignObject, .wrapper-3t9DeA + svg foreignObject, .avatarContainerMasked-PIJ-3L foreignObject {mask: none;}
.wrapper-3t9DeA img, .voiceAvatar-14IynY, .border-Jn5IOt, .avatarHint-2A3RNb, .wrapper-2QE8vf.ringingIncoming-38YcLn:after, .wrapper-2QE8vf.ringingOutgoing-mbXhhQ:after, .avatar-1BDn8e, .option-96V44q.user-O3Czj0 .displayAvatar-1wWlVM  {
	border-radius: var(--dplus-radius-avatar) !important; }
.avatar-1BDn8e.clickable-1bVtEA:active {translate: none;}

.avatar-1BDn8e {
	position: absolute;
	margin-top: 0;
	top: var(--dplus-spacing-ui) !important;
	left: var(--dplus-spacing-ui) !important;
	height: var(--dplus-icon-avatar-chat) !important;
	width: var(--dplus-icon-avatar-chat) !important;
}
.cozy-3raOZG.wrapper-2a6GCs {
	padding-left: calc(var(--dplus-icon-avatar-chat) + var(--dplus-spacing-ui) * 2);
}

.avatar-3uk_u9 .wrapper-3t9DeA {
	width: var(--dplus-icon-avatar-list) !important;
	height: var(--dplus-icon-avatar-list) !important;
}

.avatar-3uk_u9 {
	margin-right: var(--dplus-spacing-ui);
}

.layout-2DM8Md {
	height: calc(var(--dplus-icon-avatar-list) + var(--dplus-spacing-ui));
}

.container-1r6BKw.themed-ANHk51 {
	background: var(--dplus-bgc-ui-base);
}

	/* Messages */
.scrollerContent-WzeG7R {
	min-height: 0;
}
.container-3RCQyg {
	padding: 0 !important;
  border-bottom: none;
}
.container-3RCQyg .wrapper-3t9DeA {
	margin-left: var(--dplus-spacing-ui);
	margin-top: var(--dplus-spacing-ui);
}
.emptyChannelIcon-cc932w {
	border-radius: var(--dplus-radius-ui);
	margin-left: var(--dplus-spacing-ui);
}
.container-3RCQyg .header-3uLluP,
.container-3RCQyg .description-1sDbzZ {
	margin-left: var(--dplus-spacing-ui);
}
.buttonContainer-2GVjL_ {
	margin: var(--dplus-spacing-ui);
}
.reaction-1hd86g.reactionMe-wv5HKu {border-color: var(--dplus-accent-ui);}
#app-mount .backgroundFlash-24qWLN {background: transparent!important;}
.theme-dark .backgroundFlash-24qWLN .message-2qnXI6
	{ background-color: rgba(250, 166, 26, 0.50) !important; }
.theme-light .backgroundFlash-24qWLN .message-2qnXI6
	{ background-color: #ffe9c9de !important; }

.cozyMessage-3V1Y8y.groupStart-23k01U + .backgroundFlash-24qWLN.groupStart-23k01U {
	margin-top: 48px !important;
	padding-top: 0 !important;
	border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0 !important;
}

.cozyMessage-3V1Y8y:not(.groupStart-23k01U) + .hasContent-1cNJDh + .backgroundFlash-24qWLN.groupStart-23k01U {
	margin-top: 0 !important;
	padding-top: 0 !important;
	border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0 !important;
}

.backgroundFlash-24qWLN .groupStart-23k01U:before {
    top: calc(-11px - var(--group-spacing) - var(--dplus-radius-ui) - var(--dplus-calc-chatmsg-spacing) - var(--dplus-spacing-ui)) !important;
    height: calc(var(--dplus-radius-ui) + var(--dplus-calc-chatmsg-spacing) + var(--dplus-spacing-ui));
}


	/* Embeds */
.embed-IeVjo6 {
	border-radius: var(--dplus-radius-ui);
}

	/* Timestamps */
.timestampVisibleOnHover-2bQeI4 {
	transition: var(--dplus-anim-short);
}

.timestampVisibleOnHover-2bQeI4 time {
	padding: calc(var(--dplus-spacing-ui) / 2);
	background: var(--dplus-bgc-popout);
	border-radius: var(--dplus-radius-ui);
}
.timestampVisibleOnHover-2bQeI4 time:nth-child(2) {
	margin-left: var(--dplus-spacing-ui);
}

.timestampVisibleOnHover-2bQeI4.alt-1uNpEt {
	left: calc(-5px + var(--dplus-spacing-ui) / 2) !important
}

.timestamp-3ZCmNB.alt-1uNpEt,
.compact-T3H92H .timestamp-3ZCmNB {
	width: 64px !important;
}

.wrapper-2a6GCs:not(.disableInteraction-286MMw), .scrollerSpacer-avRLaA, .groupStart-23k01U:before, .container-3RCQyg {
	background-color: var(--dplus-bgc-chatmsg);
	box-shadow: none;
}
.groupStart-23k01U {
	border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0;
	padding-top: var(--dplus-spacing-ui) !important;
}

.username-1A8OIy {
	font-size: 1.125rem;
}

.wrapper-2aW0bm {
	border-radius: var(--dplus-radius-ui);
}

.scrollerSpacer-avRLaA, .groupStart-23k01U:before {
	border-radius:  0 0 var(--dplus-radius-ui) var(--dplus-radius-ui);
	width: 100%;
}
.wrapper-2a6GCs:hover, .wrapper-2a6GCs.selected-2P5D_Z {
	background: var(--dplus-bgc-chatmsg-hover) !important;
}
.compact-T3H92H.wrapper-2a6GCs, .cozy-3raOZG.wrapper-2a6GCs, .message-2qnXI6:hover {
	padding-top: 0px;
	padding-bottom: 0px;
}
.systemMessage-1I9LCe {
	padding-top: var(--dplus-spacing-ui) !important;
}
.groupStart-23k01U.systemMessage-1I9LCe {
	padding-top: calc(var(--dplus-radius-ui) + var(--dplus-spacing-ui)) !important;
}
.systemMessage-1I9LCe .iconContainer-3GkGRf {
	width: var(--dplus-icon-avatar-chat);
	margin-right: var(--dplus-spacing-ui);
}

.chatContent-a9vAAp {
	--dplus-calc-chatmsg-spacing: calc(var(--dplus-icon-avatar-chat) / 10);
}

.group-spacing-0 { --group-spacing: 0px; }
.group-spacing-4 { --group-spacing: 4px; }
.group-spacing-8 { --group-spacing: 8px; }
.group-spacing-16 { --group-spacing: 10px; }
.group-spacing-24 { --group-spacing: var(--dplus-spacing-ui); }

[aria-valuemin="0"][aria-valuemax="24"] [style="left: 0%;"] .markValue-2DwdXI,
[aria-valuemin="0"][aria-valuemax="24"] [style="left: 66.6667%;"] .markValue-2DwdXI,
[aria-valuemin="0"][aria-valuemax="24"] [style="left: 100%;"] .markValue-2DwdXI {
	font-size: 0px;
}
[aria-valuemin="0"][aria-valuemax="24"] [style="left: 0%;"] .markValue-2DwdXI::before {
	display: block;
	color: inherit;
	font-size: 10px;
	content: "OFF";
}

[aria-valuemin="0"][aria-valuemax="24"] [style="left: 66.6667%;"] .markValue-2DwdXI::before {
	display: block;
	color: inherit;
	font-size: 10px;
	content: "10px";
}

[aria-valuemin="0"][aria-valuemax="24"] [style="left: 100%;"] .markValue-2DwdXI::before {
	display: block;
	color: inherit;
	width: 50px;
	font-size: 10px;
	content: "Spacing variable";
}

.groupStart-23k01U {
	margin-top: calc(var(--group-spacing) + var(--dplus-radius-ui) + var(--dplus-calc-chatmsg-spacing) + var(--dplus-spacing-ui)) !important;
}
.groupStart-23k01U:before {
	content: "";
	position: absolute;
	top: calc(0px - var(--group-spacing) - var(--dplus-radius-ui) - var(--dplus-calc-chatmsg-spacing) - var(--dplus-spacing-ui)) !important;
	left: 0;
	pointer-events: none;
	height: calc(var(--dplus-radius-ui) + var(--dplus-calc-chatmsg-spacing)  + var(--dplus-spacing-ui));
}

/* very last message in chat */
.scrollerSpacer-avRLaA {
	height: calc(var(--dplus-calc-chatmsg-spacing) + var(--dplus-radius-ui) + var(--dplus-spacing-ui))!important;
}

.cozyMessage-3V1Y8y .scroller-2LSbBU {
	border-bottom-left-radius: var(--dplus-radius-ui);
	border-bottom-right-radius: var(--dplus-radius-ui);
}

.divider-3_HH5L { margin-bottom: 0px !important; }
.divider-JfaTT5, .container-3RCQyg {
	margin-top: -1px !important;
}

.divider-3_HH5L.isUnread-3Ef-o9.beforeGroup-1rH1F0 {
	top: 32px !important;
}

.imageWrapper-2p5ogY {
	border-radius: var(--dplus-radius-ui);
}

.group-spacing-0,
.group-spacing-4,
.group-spacing-8,
.group-spacing-16,
.group-spacing-24 {
	--hascontent-correction-groupstart: calc(0px - var(--group-spacing) + 4px);
	--hascontent-correction-groupstart-before: calc(var(--group-spacing));
}

.hasContent-1cNJDh {
	position: relative;
	top: calc(3px + var(--dplus-radius-ui));
	margin-left: 0px;
	margin-top: var(--dplus-spacing-ui) !important;
}

.hasContent-1cNJDh + .groupStart-23k01U { border-top-left-radius: 0; }


/* Message groups with more than one message */
.cozyMessage-3V1Y8y:not(.groupStart-23k01U) + .hasContent-1cNJDh
	{ top: calc(-2px + var(--group-spacing) + var(--dplus-radius-ui)); }
.cozyMessage-3V1Y8y:not(.groupStart-23k01U) + .hasContent-1cNJDh + .cozyMessage-3V1Y8y.groupStart-23k01U
	{ margin-top: calc(6px + var(--group-spacing) + var(--dplus-radius-ui)) !important; }
.hasContent-1cNJDh + .cozyMessage-3V1Y8y.groupStart-23k01U:before
	{ top: calc(-7px - var(--group-spacing) - var(--dplus-radius-ui) - var(--dplus-spacing-ui)) !important;
	height: var(--dplus-radius-ui); }

/* Message groups with only one message */
.groupStart-23k01U + .hasContent-1cNJDh {
	top: calc(-2px + var(--group-spacing) * 2 + var(--dplus-radius-ui));
}
.groupStart-23k01U + .hasContent-1cNJDh {
	margin-top: calc(-10px - var(--hascontent-correction-groupstart) + var(--group-spacing) + var(--dplus-radius-ui)) !important;
}
.groupStart-23k01U + .hasContent-1cNJDh + .cozyMessage-3V1Y8y.groupStart-23k01U:before {
	top: calc(-4px - var(--hascontent-correction-groupstart-before) - var(--group-spacing) * 2 - var(--dplus-radius-ui) - var(--dplus-spacing-ui)) !important;
	height: calc(var(--dplus-radius-ui) + var(--dplus-calc-chatmsg-spacing) + var(--dplus-spacing-ui)) !important;
}


.content-1o0f9g {
	background: var(--dplus-bgc-chatmsg);
	color: var(--text-normal);
	margin-top: 0px;
	border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0;
}

.divider-JfaTT5 {
	justify-content: flex-start;
}

.messageListItem-1-jvGY:hover + li .groupStart-23k01U:before,
.messageListItem-1-jvGY:hover + .scrollerSpacer-avRLaA,
.wrapper-2a6GCs:hover + .hasContent-1cNJDh + .groupStart-23k01U:before {
	background-color: var(--dplus-bgc-chatmsg-hover);
}

.container-3RCQyg { margin: 0; padding-left: 5px; }

	/* Pings */
.mentioned-xhSam7 {background: var(--dplus-bg-1);}
.mentioned-xhSam7 .messageContent-2qWWxC:not(.repliedbodyContent-1R3vnK) {
	background: rgba(250, 166, 26, 0.18);;
	border-radius: 8px;
	z-index: 2;
	margin-left: 0px;
    padding-left: 0px;
    width: calc(100% + 48px);
}
.theme-light .mentioned-xhSam7 .messageContent-2qWWxC {background-color: #ffe9c9de;}
.wrapper-3WhCwL, #app-mount .mentioned-xhSam7 .mention {background: rgba(114,137,218,0.1)!important;}
.mentioned-xhSam7:not(.groupStart-23k01U)::before {display: none;}

	/* @everyone warning */
.theme-dark .contentWarningPopout-n5JsIs,
.theme-light .contentWarningPopout-n5JsIs {
	background-color: var(--dplus-bgc-ui-base);
}
.contentWarningPopout-n5JsIs { border-radius: var(--dplus-radius-ui); }
.contentWarningPopout-n5JsIs .footer-3N9rgh { border-radius: 0 0 var(--dplus-radius-ui) var(--dplus-radius-ui)}

	/* Replies */
.cozy-3raOZG .repliedMessage-VokQwo {margin-left: 13px;}

	/* Message box */
.form-2fGMdU {
	border-top: none;
	padding: 0; margin: 0 10px;
}
#app-mount .channelbodyArea-rNsIhG {margin-top: var(--dplus-spacing-ui);}
.form-2fGMdU:before {display: none;}
.chat-3bRxxu form {
	box-shadow: none;
	margin: 0 10px -24px 0px;
}
.wrapper-39oAo3 {
	height: 12px;
	background: var(--dplus-bgc-ui-card);
	margin-top: var(--dplus-spacing-ui);
	border-radius: var(--dplus-radius-ui);
}

.channelbodyAreaDisabled-8rmlrp {
	background: var(--dplus-bgc-ui-card);
}

.scrollableContainer-2NUZem {
	overflow-y: auto;
	background-color: transparent;
	border-radius: var(--dplus-radius-ui);
	margin-top: var(--dplus-spacing-ui);
}
.webkit-HjD9Er .buttons-3JBrkn {
	margin-right: calc(var(--dplus-spacing-ui) - 6px);
}

	/* Typing indicator */
.base-gE7OpD {
	background: transparent!important;
	font-size: 12px;
	top: calc(5% - var(--dplus-spacing-ui));
}
.theme-light .dots-3Bkt3k.themed-IQiCm3, .theme-light .base-gE7OpD {color: #fff;}

	/* Calling */
.controlButton-2MhVEL foreignObject {mask: none;}
#app-mount .wrapper-2qzCYF {
	background-color: var(--dplus-bgc-ui-base)!important;
}
.videoWrapper-2v09vt, :not(:root):-webkit-full-screen::backdrop, .callContainer-36WRfH {background-color: transparent;}

.videoHeight-Qp_9vC.noChat-3nt48u {
	height: 100%;
}
.streamPreviewWrapper-2DSWOK {padding: 0;}
.centerButton-3CaNcJ, .avatarSpeaking-2c8-9i {border-radius: var(--dplus-radius-avatar);}
.colorable-1bkp8v.primaryDark-3mSFDl {background-color: var(--dplus-bgc-ui-base);}
.colorable-1bkp8v.primaryDark-3mSFDl:hover {background-color: var(--background-accent);}
.tile-2naSqK {background: transparent!important;}
.background-ujHpbY {background-color: var(--dplus-bg-1)!important;}
.avatarSpeaking-2IGMRN, .border-3dQmSY.speaking-WDn8Wm, .border-Jn5IOt.speaking-B2MXPi, .avatarSpeaking-2c8-9i {
    -webkit-box-shadow: inset 0 0 0 2px var(--dplus-accent-ui),inset 0 0 0 3px var(--background-secondary);
    box-shadow: inset 0 0 0 2px var(--dplus-accent-ui),inset 0 0 0 3px var(--background-secondary);
}

	/* Attachments */
#app-mount .attachment-33OFj0,
#app-mount .wrapper-2TxpI8 {
	background-color: var(--dplus-bgc-popout)!important;
	border-color: var(--dplus-accent-ui) !important;
}
.attachment-33OFj0,
.wrapper-2TxpI8,
.audioControls-2HsaU6,
.videoControls-2kcYic {
	border-radius: var(--dplus-radius-ui) !important;
}
.small-1CUeBa[style*="transform"] {background-color: var(--background-accent)!important;}

	/* New/Old/Load messages bar */
.newMessagesBar-265mhP {
	background-color: var(--dplus-accent-ui) !important;
	border-radius: 0 0 var(--dplus-radius-ui) var(--dplus-radius-ui) !important;
	width: 100%;
}
.newMessagesBar-265mhP button:last-child {
	font-size: 12px;
	text-transform: lowercase;
}
.barBase-1c2Rfb {
	padding: 0;
	left: 0; right: 0;
}
#app-mount .jumpToPresentBar-9P20AM {
	background-color: var(--dplus-accent-ui);
	border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0;
	bottom: 0;
	padding: 0;
	cursor: pointer;
	z-index: 2;
}
.hasMore-3e72_v {
	background: var(--dplus-bg-1);
	color: var(--dplus-accent-ui);
	border: 2px solid var(--dplus-accent-ui);
	margin: 0
}

	/* Server members */
.members-1998pB {
	width: var(--dplus-members-width);
}
.member-3-YXUe.clickable-1JJAn8:hover .layout-2DM8Md {
	transition: background-color var(--dplus-anim-short);
}
.members-1998pB>div { background:transparent;}
.members-1998pB {
	background: var(--dplus-bgc-ui-base);
}

.roleColor-rz2vM0 { /* prevent tags from flowing into a new line */
	display: inline !important;
}
.name-3_Dsmg {
	-webkit-mask-image: -webkit-linear-gradient( left, rgba(255,255,255,1), rgba(255,255,255,1), rgba(255,255,255,1), rgba(255,255,255,0) );
	mask-image: linear-gradient( left, rgba(255,255,255,1), rgba(255,255,255,1), rgba(255,255,255,1), rgba(255,255,255,0) );
}

/* Notices */
.app-2rEoOp .noticeWrapper-8z511t {
	margin-left: -10px;
	margin-right: calc(var(--dplus-spacing-app));
	margin-bottom: var(--dplus-spacing-app);
	border-radius: var(--dplus-radius-ui) !important;
}

/* Settings */
.layer-3QrUeG, .standardSidebarView-3F1I7i, .contentRegionScroller-26nc1e, .sidebarRegionScroller-3MXcoP {background-color: transparent;}
.contentColumn-2hrIYH, .customColumn-Rb6toI {
	max-width: 100%;
}
.sidebarRegion-VFTUkN {
  max-width: 218px;
	margin-right: var(--dplus-spacing-app);
}
.standardSidebarView-3F1I7i .contentRegion-3nDuYy,
.standardSidebarView-3F1I7i .contentRegion-3nDuYy {
	max-width: 100%;
}
.standardSidebarView-3F1I7i .contentRegion-3nDuYy.default,
.standardSidebarView-3F1I7i .sidebarRegion-VFTUkN .sidebar {
	padding-top: 45px;
}
.sidebar-CFHs9e {
	padding: calc(30px + var(--dplus-spacing-ui)) var(--dplus-spacing-ui) var(--dplus-spacing-ui) calc(var(--dplus-spacing-ui) * 2)
}
.contentColumnDefault-1VQkGM {
  padding: calc(30px + var(--dplus-spacing-ui)) calc(var(--dplus-spacing-ui) * 2) calc(var(--dplus-spacing-ui) * 2);
}
.horizontal-1ae9ci>.flex-1xMQg5, .horizontal-1ae9ci>.flexChild-faoVW3 {
	margin-left: var(--dplus-spacing-ui);
}

.marginBottom8-AtZOdT {
	margin-bottom: var(--dplus-spacing-ui);
}
.marginBottom40-2vIwTv {
	margin-bottom: calc(10px + var(--dplus-spacing-ui));
}
.marginTop40-i-78cZ {
	margin-top: calc(10px + var(--dplus-spacing-ui));
}

.preview-2nSL_2 {
	height: calc(180px + var(--dplus-spacing-ui));
}

.profileBannerPreview-3_l0Wd
{ border-radius: var(--dplus-radius-ui); }

.banner-hcPdsd
{ border-radius: var(--dplus-radius-ui) var(--dplus-radius-ui) 0 0; }

.h1-1qdNzo, .h2-2gWE-o,
.h4-AQvcAz, .h5-18_1nd {
	font-weight: 500;
}

.platform-osx [id="user-settings"] {
	left: -5px !important;
	top: -5px !important;
	right: -5px !important;
	bottom: -5px !important;
}

.platform-win [id="user-settings"] {
	left: -5px !important;
	top: -27px !important;
	right: -5px !important;
	bottom: -5px !important;
}

.platform-linux [id="user-settings"] {
	left: -5px !important;
	top: -5px !important;
	right: -5px !important;
	bottom: -5px !important;
}

#app-mount .standardSidebarView-3F1I7i .contentRegion-3nDuYy,
#app-mount .standardSidebarView-3F1I7i .sidebarRegion-VFTUkN {
	background-color: var(--dplus-bgc-ui-base);
	border-radius: var(--dplus-radius-ui);
}
#app-mount .standardSidebarView-3F1I7i .contentRegion-3nDuYy,
#app-mount .standardSidebarView-3F1I7i .sidebarRegion-VFTUkN,
.itemDefault-3Jdr52,
.itemHover-EnbcjT,
.ui-tab-bar-item,
#app-mount .side-8zPYf6 .itemDefault-3Jdr52:hover,
#app-mount .side-8zPYf6 .itemHover-EnbcjT:hover,
#app-mount #bd-settings-sidebar .ui-tab-bar-item:hover,
#app-mount .closeButton-1tv5uR {
	transition: background-color;
	transition-duration: var(--dplus-anim-short);
}

.item-PXvHYJ {
	transition: background-color, color, border;
	transition-duration: var(--dplus-anim-short);
}

.cardPrimary-1Hv-to, .cardPrimaryOutline-29Ujqw {
	background-color: var(--dplus-bgc-button);
	border-radius: var(--dplus-radius-ui);
}

#app-mount .closeButton-1tv5uR {
	border-color: var(--dplus-accent-ui);
	border-radius: var(--dplus-radius-ui);
}
#app-mount .closeButton-1tv5uR:hover {
	background-color: var(--dplus-bgc-button-hover);
}
.item-26Dhrx {
	background-color: var(--dplus-bgc-ui-base);
	transition: var(--dplus-anim-button);
	border-radius: var(--dplus-radius-ui);
}
.item-26Dhrx:hover:not([aria-checked=true]) {
	background-color: var(--dplus-bgc-radiobar-hover);
}
.item-26Dhrx[aria-checked=true] {
	background-color: var(--dplus-bgc-radiobar-selected);
}
#app-mount .closeButton-1tv5uR path {fill: var(--dplus-accent-ui);}
#app-mount .closeButton-1tv5uR:hover path {fill: white}
#app-mount .closeButton-1tv5uR + .keybind-KpFkfr {color: var(--text-normal);}
.background-1QDuV2 { border-radius: var(--dplus-radius-ui); }
.background-1QDuV2 .avatarUploaderInner-3UNxY3 {border-radius: var(--dplus-radius-avatar);}

	/* Avatar Preview */
.overlay-4k_Q4-:after {
	content: "";
	box-shadow: 0 0 0 9999px rgba(0,0,0,.6);
	border: 5px solid var(--dplus-accent-ui);
	border-radius: var(--dplus-radius-avatar);
	height: 100%; width: 100%;
	position: absolute;
	left: -5px; top: -5px;
	z-index: 1;
	pointer-events: none;
}
.overlay-4k_Q4- {box-shadow: 0 0 0 9999px rgba(0, 0, 0, 0.3);}
.sliderContainer-1N1-Pn::after {
	content: "Accent coloured box previews how much is visible with the theme on.";
	color: var(--text-normal);
	position: absolute;
	bottom: 10px;
}
	/* Billing */
#app-mount .expandedInfo-3kfShd, #app-mount .codeRedemptionRedirect-1wVR4b {
	background-color: var(--dplus-bg-1) !important;
	border-radius: var(--dplus-radius-ui);
}
.bottomDivider-1K9Gao.scrollerBase-289Jih{overflow: hidden!important;}
#app-mount .paginator-166-09 {background-color: transparent!important;}
#app-mount .bottomDivider-1K9Gao {border-color: var(--dplus-accent-ui);}
	/* Voice and Video */
.css-gvi9bl-control, .css-6fzn47-control, .css-17e1tep-control {border-color: var(--dplus-accent-ui)!important;}
.css-3vaxre-menu {
	background-color: var(--dplus-bgc-popout);
	box-shadow: none; border: none;
}
#app-mount .bar-2Qqk5Z:not(.sliderBar-3DezvM) {background-color: var(--dplus-bg-1);}
.bar-2Qqk5Z.sliderBar-3DezvM {opacity: 0.8;}
.css-1ba14n5-option:hover, .css-rzbxvl-option:hover, .barFill-23-gu- {
	background-color: var(--dplus-accent-ui);
}
.container-3PXSwK { /* Fix for Mic Test being long */
	max-width: 560px;
	-webkit-mask: url('data:image/svg+xml;base64,PHN2ZyB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB3aWR0aD0iOCIgaGVpZ2h0PSIyMCIgZmlsbD0iIzM2MzkzZiI+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBkPSJNNCAyYTIgMiAwIDAgMC0yIDJ2MTJhMiAyIDAgMSAwIDQgMFY0YTIgMiAwIDAgMC0yLTJ6Ii8+PC9zdmc+');
	mask: url('data:image/svg+xml;base64,PHN2ZyB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB3aWR0aD0iOCIgaGVpZ2h0PSIyMCIgZmlsbD0iIzM2MzkzZiI+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBkPSJNNCAyYTIgMiAwIDAgMC0yIDJ2MTJhMiAyIDAgMSAwIDQgMFY0YTIgMiAwIDAgMC0yLTJ6Ii8+PC9zdmc+');;
}
.progress-1IcQ3A {
	height: 20px !important;
}
#app-mount .userSettingsVoice-iwdUCU .previewOverlay-2O7_KC {
	background-color: transparent;
	border-color: var(--background-accent);
}
.userSettingsVoice-iwdUCU .media-engine-video {background-color: var(--dplus-bg-1);}

	/* Overlay */
.option-n0icdO, .wrapper-3jrx9n, .selected-mKYnfr.option-n0icdO {border-radius: var(--dplus-radius-ui);}
.option-n0icdO {background-color: var(--dplus-bg-1);}
.wrapper-3jrx9n {border-color: var(--dplus-accent-ui);}
.selected-mKYnfr.option-n0icdO, .option-n0icdO:hover {background-color: var(--dplus-accent-ui);}
	/* Keybinds */
.removeKeybind-39dSFj { right: -17px; top: 2px;}
#app-mount .card-FDVird .button-2CgfFz {
	background-color: transparent;
	border-radius: var(--dplus-radius-ui);
	box-shadow: none;
}
#app-mount .card-FDVird .removeKeybind-39dSFj:hover {background-color: var(--dplus-accent-ui);}

/* Switches, Checkboxes, Buttons */
button, [type="button"] {
border-radius: var(--dplus-radius-ui) !important;
}
button,
[type="button"] {
transition: var(--dplus-anim-button) !important;
}

.container-3auIfb svg path, svg.bd-switch-symbol {display:none;}
.container-3auIfb, .bd-switch-checked .bd-switch-body {background-color: var(--dplus-accent-ui) !important;}

.container-3auIfb[style*="218"] {
	background-color: hsl(218, calc(var(--saturation-factor, 1) * 4.6%), 46.9%) !important;
}

.container-3auIfb[style*="rgb(114, 118, 125)"] {
	background-color: rgb(114, 118, 125) !important;
}

/* Server settings */
.avatarUploaderInner-Oiob_P {border-radius: var(--dplus-radius-avatar);}
.avatarUploader-2yeaMv .avatarUploaderInnerSquare-2UOXj4, .avatarUploaderDisabled-310UAf .avatarUploaderInnerSquare-2UOXj4 {
background-size: contain;
}
.fieldList-21DyL8 {
background-color: transparent;
}
.scroller-305q3I, #app-mount .headerClickable-2IVFo9, #app-mount .headerDefault-1wrJcN {background: transparent;}
.select-2TCrqx .Select-menu-outer, #app-mount .auditLog-3jNbM6 {
background: var(--dplus-bg-dark-3) !important;
border-color: var(--dplus-accent-ui) !important;
border-radius: var(--dplus-radius-ui) !important;
}
.regionSelectModal-12e-57 {background-color: var(--dplus-accent-ui)!important;}
.regionSelectModal-12e-57 .regionSelectModalOption-2DSIZ3 {background-color: transparent; border: none;}
.regionSelectModal-12e-57 .regionSelectModalOption-2DSIZ3:hover {background-color: var(--dplus-bg-1);}

.viewAsRoleButton-1ZpPlO {
background-color: var(--dplus-accent-ui)!important;
}
.input-cIJ7To:hover {border-color: var(--dplus-accent-ui);}
.item-PXvHYJ,
.input-cIJ7To,
.copyInput-2rOSt7,
.Select .Select-control,
.Select.is-open .Select-control {
border-radius: var(--dplus-radius-ui) !important;
}

#app-mount .colorPickerCustom-2CWBn2 {
background: transparent;
border-color: var(--dplus-accent-ui); border-radius: var(--dplus-radius-ui);
}

/* Accessibility / a11y */
	/* Font sizes */
html[style^="font-size: 75%;"] { --chat-font-scaling: 0.75; }
html[style^="font-size: 87.5%;"] { --chat-font-scaling: 0.875; }
html[style^="font-size: 93.75%;"] { --chat-font-scaling: 0.9375; }
.a11y-font-scaled-down .cozy-3raOZG.wrapper-2a6GCs {
	padding-left: calc(var(--dplus-icon-avatar-chat) * var(--chat-font-scaling) + var(--dplus-spacing-ui) * 2);
}
.a11y-font-scaled-down .cozy-3raOZG.wrapper-2a6GCs .avatar-1BDn8e {
	width: calc(var(--dplus-icon-avatar-chat) * var(--chat-font-scaling)) !important;
	height: calc(var(--dplus-icon-avatar-chat) * var(--chat-font-scaling)) !important;
}


/* Client mod specific */
	/* BetterDiscord */
		/* Addon lists */
.bd-addon-list.bd-grid-view {
  column-gap: var(--dplus-spacing-ui);
  row-gap: var(--dplus-spacing-ui);
}
.bd-addon-list .bd-addon-card {
	background: var(--dplus-bgc-ui-card);
	border: none; border-radius: var(--dplus-radius-ui) !important;
	max-height: 100%;
	padding: var(--dplus-spacing-ui);
	margin-bottom: var(--dplus-spacing-ui);
}
.bd-addon-list .bd-addon-header,
.bd-description-wrap,
.bd-addon-list .bd-footer {
	padding: var(--dplus-spacing-ui);
}

.bd-select .bd-select-options {background: var(--dplus-bg-2); backdrop-filter: var(--blurcalc-popout);}
.bd-select-transparent .bd-select-options { border-radius: var(--dplus-radius-ui) !important; border-color: var(--dplus-bg-1);}
.bd-search-wrapper, .bd-select .bd-select-option:hover, .bd-select .bd-select-option.selected { background: var(--dplus-bg-1);}
.bda-slist .bda-header {
	font-size: 14px;
	line-height: 1.25;
	padding-bottom: 5px;
}
.bda-slist .bda-description {
	max-height: 100%;
	overflow-y: hidden;
	padding: 0;
	padding-bottom: 2px;
}
.bda-slist .bda-footer, .bda-slist .bda-header {border: none;}
.bda-name, .bda-author {
	font-size: 16px;
}
.bda-author {
	color: var(--dplus-accent-ui);
}
.bda-links {
	font-size: 0;
}
.bda-links .bda-link {
	font-size: 12px;
}
.bda-link:not(:first-of-type) {
	margin-left: 10px;
}
.theme-dark .bda-slist .bda-header, .theme-dark .bda-slist .bda-description  { color: white; }

		/* Toast Notifications */
.toast, .bd-toast {
    background: var(--dplus-bg-3)!important;
    border: 2px solid var(--dplus-accent-ui)!important;
    border-radius: var(--dplus-radius-ui)!important;
    color: var(--dplus-accent-ui)!important;
    box-shadow: none!important;
}

	/* GooseMod */
		/* Addons tabs */
.tabBody-3YRQ8W .scrollerBase-289Jih.auto-Ge5KZx {
	background-color: transparent !important;
	padding: var(--dplus-spacing-ui) !important;
}
.DOM.CSS {
	border-radius: var(--dplus-radius-ui) !important;
	margin: calc(var(--dplus-spacing-ui) / 2) !important;
}
