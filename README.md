<!DOCTYPE html>
<!-- saved from url=(0050)https://cryptodeeptech.ru/blockchain-google-drive/ -->
<html lang="ru-RU"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
	
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="profile" href="https://gmpg.org/xfn/11">

	<meta name="robots" content="index, follow, max-image-preview:large, max-snippet:-1, max-video-preview:-1">

	<!-- This site is optimized with the Yoast SEO plugin v19.2 - https://yoast.com/wordpress/plugins/seo/ -->
	<style type="text/css"></style><title>How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»</title>
	<meta name="description" content="Blockchain parsing save everything in one file in Google Drive folder bash script finds unspent transaction output (UTXO) via API">
	<link rel="canonical" href="https://cryptodeeptech.ru/blockchain-google-drive/">
	<meta property="og:locale" content="ru_RU">
	<meta property="og:type" content="article">
	<meta property="og:title" content="How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»">
	<meta property="og:description" content="Blockchain parsing save everything in one file in Google Drive folder bash script finds unspent transaction output (UTXO) via API">
	<meta property="og:url" content="https://cryptodeeptech.ru/blockchain-google-drive/">
	<meta property="og:site_name" content="«CRYPTO DEEP TECH»">
	<meta property="article:published_time" content="2022-07-04T18:13:48+00:00">
	<meta property="article:modified_time" content="2022-08-25T19:23:09+00:00">
	<meta property="og:image" content="https://habrastorage.org/r/w1560/getpro/habr/upload_files/7e4/268/a3a/7e4268a3ab7e36fc45020c6b222b7611.png">
	<meta name="author" content="Crypto Deep Tech">
	<meta name="twitter:card" content="summary_large_image">
	<meta name="twitter:label1" content="Написано автором">
	<meta name="twitter:data1" content="Crypto Deep Tech">
	<meta name="twitter:label2" content="Примерное время для чтения">
	<meta name="twitter:data2" content="7 минут">
	<script async="" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/tag.js"></script><script type="application/ld+json" class="yoast-schema-graph">{"@context":"https://schema.org","@graph":[{"@type":"WebSite","@id":"https://cryptodeeptech.ru/#website","url":"https://cryptodeeptech.ru/","name":"«CRYPTO DEEP TECH»","description":"Cryptanalysis and data financial security services","potentialAction":[{"@type":"SearchAction","target":{"@type":"EntryPoint","urlTemplate":"https://cryptodeeptech.ru/?s={search_term_string}"},"query-input":"required name=search_term_string"}],"inLanguage":"ru-RU"},{"@type":"ImageObject","inLanguage":"ru-RU","@id":"https://cryptodeeptech.ru/blockchain-google-drive/#primaryimage","url":"https://habrastorage.org/r/w1560/getpro/habr/upload_files/7e4/268/a3a/7e4268a3ab7e36fc45020c6b222b7611.png","contentUrl":"https://habrastorage.org/r/w1560/getpro/habr/upload_files/7e4/268/a3a/7e4268a3ab7e36fc45020c6b222b7611.png"},{"@type":"WebPage","@id":"https://cryptodeeptech.ru/blockchain-google-drive/#webpage","url":"https://cryptodeeptech.ru/blockchain-google-drive/","name":"How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»","isPartOf":{"@id":"https://cryptodeeptech.ru/#website"},"primaryImageOfPage":{"@id":"https://cryptodeeptech.ru/blockchain-google-drive/#primaryimage"},"datePublished":"2022-07-04T18:13:48+00:00","dateModified":"2022-08-25T19:23:09+00:00","author":{"@id":"https://cryptodeeptech.ru/#/schema/person/0ef8ac0f63991970628a3a6587f9e6c0"},"description":"Blockchain parsing save everything in one file in Google Drive folder bash script finds unspent transaction output (UTXO) via API","breadcrumb":{"@id":"https://cryptodeeptech.ru/blockchain-google-drive/#breadcrumb"},"inLanguage":"ru-RU","potentialAction":[{"@type":"ReadAction","target":["https://cryptodeeptech.ru/blockchain-google-drive/"]}]},{"@type":"BreadcrumbList","@id":"https://cryptodeeptech.ru/blockchain-google-drive/#breadcrumb","itemListElement":[{"@type":"ListItem","position":1,"name":"Главная страница","item":"https://cryptodeeptech.ru/"},{"@type":"ListItem","position":2,"name":"How to Parse Blockchain Transactions to a Google Drive Folder"}]},{"@type":"Person","@id":"https://cryptodeeptech.ru/#/schema/person/0ef8ac0f63991970628a3a6587f9e6c0","name":"Crypto Deep Tech","sameAs":["https://cryptodeeptech.ru","https://www.youtube.com/channel/UCd8W6qtRSiBn0Q0wy6HuNkQ/"],"url":"https://cryptodeeptech.ru/author/cryptodeeptech/"}]}</script>
	<!-- / Yoast SEO plugin. -->


<link rel="dns-prefetch" href="https://fonts.googleapis.com/">
<link rel="alternate" type="application/rss+xml" title="«CRYPTO DEEP TECH» » Лента" href="https://cryptodeeptech.ru/feed/">
<link rel="alternate" type="application/rss+xml" title="«CRYPTO DEEP TECH» » Лента комментариев" href="https://cryptodeeptech.ru/comments/feed/">
<link rel="alternate" type="application/rss+xml" title="«CRYPTO DEEP TECH» » Лента комментариев к «How to Parse Blockchain Transactions to a Google Drive Folder»" href="https://cryptodeeptech.ru/blockchain-google-drive/feed/">
<link rel="stylesheet" id="itng-block-style-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_8f426a1779caff96bb3f2afbcff86bc9.css" media="all">
<link rel="stylesheet" id="wp-block-library-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/style.min.css" media="all">
<style id="global-styles-inline-css">
body{--wp--preset--color--black: #000000;--wp--preset--color--cyan-bluish-gray: #abb8c3;--wp--preset--color--white: #ffffff;--wp--preset--color--pale-pink: #f78da7;--wp--preset--color--vivid-red: #cf2e2e;--wp--preset--color--luminous-vivid-orange: #ff6900;--wp--preset--color--luminous-vivid-amber: #fcb900;--wp--preset--color--light-green-cyan: #7bdcb5;--wp--preset--color--vivid-green-cyan: #00d084;--wp--preset--color--pale-cyan-blue: #8ed1fc;--wp--preset--color--vivid-cyan-blue: #0693e3;--wp--preset--color--vivid-purple: #9b51e0;--wp--preset--gradient--vivid-cyan-blue-to-vivid-purple: linear-gradient(135deg,rgba(6,147,227,1) 0%,rgb(155,81,224) 100%);--wp--preset--gradient--light-green-cyan-to-vivid-green-cyan: linear-gradient(135deg,rgb(122,220,180) 0%,rgb(0,208,130) 100%);--wp--preset--gradient--luminous-vivid-amber-to-luminous-vivid-orange: linear-gradient(135deg,rgba(252,185,0,1) 0%,rgba(255,105,0,1) 100%);--wp--preset--gradient--luminous-vivid-orange-to-vivid-red: linear-gradient(135deg,rgba(255,105,0,1) 0%,rgb(207,46,46) 100%);--wp--preset--gradient--very-light-gray-to-cyan-bluish-gray: linear-gradient(135deg,rgb(238,238,238) 0%,rgb(169,184,195) 100%);--wp--preset--gradient--cool-to-warm-spectrum: linear-gradient(135deg,rgb(74,234,220) 0%,rgb(151,120,209) 20%,rgb(207,42,186) 40%,rgb(238,44,130) 60%,rgb(251,105,98) 80%,rgb(254,248,76) 100%);--wp--preset--gradient--blush-light-purple: linear-gradient(135deg,rgb(255,206,236) 0%,rgb(152,150,240) 100%);--wp--preset--gradient--blush-bordeaux: linear-gradient(135deg,rgb(254,205,165) 0%,rgb(254,45,45) 50%,rgb(107,0,62) 100%);--wp--preset--gradient--luminous-dusk: linear-gradient(135deg,rgb(255,203,112) 0%,rgb(199,81,192) 50%,rgb(65,88,208) 100%);--wp--preset--gradient--pale-ocean: linear-gradient(135deg,rgb(255,245,203) 0%,rgb(182,227,212) 50%,rgb(51,167,181) 100%);--wp--preset--gradient--electric-grass: linear-gradient(135deg,rgb(202,248,128) 0%,rgb(113,206,126) 100%);--wp--preset--gradient--midnight: linear-gradient(135deg,rgb(2,3,129) 0%,rgb(40,116,252) 100%);--wp--preset--duotone--dark-grayscale: url('#wp-duotone-dark-grayscale');--wp--preset--duotone--grayscale: url('#wp-duotone-grayscale');--wp--preset--duotone--purple-yellow: url('#wp-duotone-purple-yellow');--wp--preset--duotone--blue-red: url('#wp-duotone-blue-red');--wp--preset--duotone--midnight: url('#wp-duotone-midnight');--wp--preset--duotone--magenta-yellow: url('#wp-duotone-magenta-yellow');--wp--preset--duotone--purple-green: url('#wp-duotone-purple-green');--wp--preset--duotone--blue-orange: url('#wp-duotone-blue-orange');--wp--preset--font-size--small: 13px;--wp--preset--font-size--medium: 20px;--wp--preset--font-size--large: 36px;--wp--preset--font-size--x-large: 42px;}.has-black-color{color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-color{color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-color{color: var(--wp--preset--color--white) !important;}.has-pale-pink-color{color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-color{color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-color{color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-color{color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-color{color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-color{color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-color{color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-color{color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-color{color: var(--wp--preset--color--vivid-purple) !important;}.has-black-background-color{background-color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-background-color{background-color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-background-color{background-color: var(--wp--preset--color--white) !important;}.has-pale-pink-background-color{background-color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-background-color{background-color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-background-color{background-color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-background-color{background-color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-background-color{background-color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-background-color{background-color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-background-color{background-color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-background-color{background-color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-background-color{background-color: var(--wp--preset--color--vivid-purple) !important;}.has-black-border-color{border-color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-border-color{border-color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-border-color{border-color: var(--wp--preset--color--white) !important;}.has-pale-pink-border-color{border-color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-border-color{border-color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-border-color{border-color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-border-color{border-color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-border-color{border-color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-border-color{border-color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-border-color{border-color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-border-color{border-color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-border-color{border-color: var(--wp--preset--color--vivid-purple) !important;}.has-vivid-cyan-blue-to-vivid-purple-gradient-background{background: var(--wp--preset--gradient--vivid-cyan-blue-to-vivid-purple) !important;}.has-light-green-cyan-to-vivid-green-cyan-gradient-background{background: var(--wp--preset--gradient--light-green-cyan-to-vivid-green-cyan) !important;}.has-luminous-vivid-amber-to-luminous-vivid-orange-gradient-background{background: var(--wp--preset--gradient--luminous-vivid-amber-to-luminous-vivid-orange) !important;}.has-luminous-vivid-orange-to-vivid-red-gradient-background{background: var(--wp--preset--gradient--luminous-vivid-orange-to-vivid-red) !important;}.has-very-light-gray-to-cyan-bluish-gray-gradient-background{background: var(--wp--preset--gradient--very-light-gray-to-cyan-bluish-gray) !important;}.has-cool-to-warm-spectrum-gradient-background{background: var(--wp--preset--gradient--cool-to-warm-spectrum) !important;}.has-blush-light-purple-gradient-background{background: var(--wp--preset--gradient--blush-light-purple) !important;}.has-blush-bordeaux-gradient-background{background: var(--wp--preset--gradient--blush-bordeaux) !important;}.has-luminous-dusk-gradient-background{background: var(--wp--preset--gradient--luminous-dusk) !important;}.has-pale-ocean-gradient-background{background: var(--wp--preset--gradient--pale-ocean) !important;}.has-electric-grass-gradient-background{background: var(--wp--preset--gradient--electric-grass) !important;}.has-midnight-gradient-background{background: var(--wp--preset--gradient--midnight) !important;}.has-small-font-size{font-size: var(--wp--preset--font-size--small) !important;}.has-medium-font-size{font-size: var(--wp--preset--font-size--medium) !important;}.has-large-font-size{font-size: var(--wp--preset--font-size--large) !important;}.has-x-large-font-size{font-size: var(--wp--preset--font-size--x-large) !important;}
</style>
<link rel="stylesheet" id="wp-date-remover-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_e6094661d8923e95b233019ebff7c8f0.css" media="all">
<link rel="stylesheet" id="itng-fonts-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/css" media="all">
<link rel="stylesheet" id="itng-style-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_8de4505c66a21eefd3c1c98b6400e4e1.css" media="all">
<link rel="stylesheet" id="itng-main-style-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_d1cf6f49400112d539e59eee9b75e10d.css" media="all">
<style id="itng-main-style-inline-css">
.custom-logo-link img {width: 400px;}@media screen and (min-width: 992px) {#header-image .header-overlay {
            opacity: 0.01;
        }}
ins,
	.nav-wrapper,
	#menu,
	.main-navigation ul#menu-desktop ul,
	#itng-featured-news .slider-post-wrapper .posted-on a,
	#itng-featured-news #itng-featured-news-list-container .posted-on a,
	#itng-featured-posts .itng-featured-post-date,
	#itng-featured-news #itng-featured-news-carousel-container .posted-on a,
	#colophon,
	[class^=itng-search] form,
	#itng-featured-cat .featured-cat-thumb h2,
	#itng-featured-cat .featured-cat-thumb h3
	{background-color: #008bca}article .entry-meta a,
	article .blog-footer,
	article .blog-footer a,
	.widget a,
	.nav-links a,
	.itng-pagination .nav-links > a,
	.itng-pagination .dots
	{color: #008bca !important}blockquote,
	#itng-content-title span
	{border-color: #008bca}button.top-menu-mobile
	{background-color: #43bdf2 !important}#footer-sidebar .widget-title
	{color: #43bdf2 !important}
</style>
<link rel="stylesheet" id="bootstrap-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_d26191bd0380b0cf97525a613b8b566c.css" media="all">
<link rel="stylesheet" id="owl-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_c8322bd5bffc8e2856f2cbcd03c61d18.css" media="all">
<link rel="stylesheet" id="mag-popup-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_30b593b71d7672658f89bfea0ab360c9.css" media="all">
<link rel="stylesheet" id="font-awesome-css" href="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_c495654869785bc3df60216616814ad1.css" media="all">
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/jquery.min.js" id="jquery-core-js"></script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/jquery-migrate.min.js" id="jquery-migrate-js"></script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_49cea0a781874a962879c2caca9bc322.js" id="wp-date-remover-js"></script>
<link rel="https://api.w.org/" href="https://cryptodeeptech.ru/wp-json/"><link rel="alternate" type="application/json" href="https://cryptodeeptech.ru/wp-json/wp/v2/posts/97"><meta name="generator" content="WordPress 6.0.1">
<link rel="alternate" type="application/json+oembed" href="https://cryptodeeptech.ru/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fcryptodeeptech.ru%2Fblockchain-google-drive%2F">
<link rel="alternate" type="text/xml+oembed" href="https://cryptodeeptech.ru/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fcryptodeeptech.ru%2Fblockchain-google-drive%2F&amp;format=xml">
<link rel="pingback" href="https://cryptodeeptech.ru/xmlrpc.php">		<style type="text/css">
						#header-image {
						background-image: url(https://cryptodeeptech.ru/wp-content/uploads/2022/07/header3.jpg);
						background-size: cover;
						background-repeat: repeat;
						background-position: center center;
				}
							.site-title, .site-description {
				display: none;
				position: absolute;
				clip: rect(1px, 1px, 1px, 1px);
				}
					</style>
		<style id="custom-background-css">
body.custom-background { background-color: #eff3fd; }
</style>
	<link rel="icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-32x32.png" sizes="32x32">
<link rel="icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-192x192.png" sizes="192x192">
<link rel="apple-touch-icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-180x180.png">
<meta name="msapplication-TileImage" content="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-270x270.png">
</head>

<body data-rsssl="1" class="post-template-default single single-post postid-97 single-format-standard custom-background wp-custom-logo no-sidebar">
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-dark-grayscale"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 0.49803921568627"></fefuncr><fefuncg type="table" tableValues="0 0.49803921568627"></fefuncg><fefuncb type="table" tableValues="0 0.49803921568627"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-grayscale"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 1"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0 1"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-purple-yellow"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.54901960784314 0.98823529411765"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0.71764705882353 0.25490196078431"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-blue-red"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 1"></fefuncr><fefuncg type="table" tableValues="0 0.27843137254902"></fefuncg><fefuncb type="table" tableValues="0.5921568627451 0.27843137254902"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-midnight"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 0"></fefuncr><fefuncg type="table" tableValues="0 0.64705882352941"></fefuncg><fefuncb type="table" tableValues="0 1"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-magenta-yellow"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.78039215686275 1"></fefuncr><fefuncg type="table" tableValues="0 0.94901960784314"></fefuncg><fefuncb type="table" tableValues="0.35294117647059 0.47058823529412"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-purple-green"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.65098039215686 0.40392156862745"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0.44705882352941 0.4"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-blue-orange"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.098039215686275 1"></fefuncr><fefuncg type="table" tableValues="0 0.66274509803922"></fefuncg><fefuncb type="table" tableValues="0.84705882352941 0.41960784313725"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><div id="page" class="site">
	<a class="skip-link screen-reader-text" href="https://cryptodeeptech.ru/blockchain-google-drive/#primary">Skip to content</a>

	
	    <header id="masthead" class="site-header style-1">

		    
	        <div id="header-image">
		        <div class="site-branding">
					<a href="https://cryptodeeptech.ru/" class="custom-logo-link" rel="home"><img width="1279" height="319" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/cropped-header4.png" class="custom-logo" alt="«CRYPTO DEEP TECH»" srcset="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4.png 1279w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-300x75.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-1024x255.png 1024w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-768x192.png 768w" sizes="(max-width: 1279px) 100vw, 1279px" title="How to Parse Blockchain Transactions to a Google Drive Folder"></a>	<h2 class="site-title"><a href="https://cryptodeeptech.ru/" rel="home">«CRYPTO DEEP TECH»</a></h2>
		<p class="site-description">Cryptanalysis and data financial security services</p>
	        	</div>
				<div class="header-overlay"></div>
	        </div>

			<div class="nav-wrapper">
				 <div class="container">
					 <div class="d-flex">

						<div id="site-navigation" class="main-navigation col-lg-11" role="navigation">
							<ul id="menu-desktop" class="menu"><li id="menu-item-229" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-229"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li id="menu-item-225" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-225"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li id="menu-item-226" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-226"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li id="menu-item-227" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-227"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li id="menu-item-228" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-228"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li id="menu-item-240" class="menu-item menu-item-type-post_type menu-item-object-post menu-item-240"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
</ul>						</div>

						<button href="#menu" class="menu-link mobile-nav-btn col-auto"><i class="fa fa-bars" aria-hidden="true"></i></button>

						<div id="search-wrapper" class="ml-auto col-auto d-flex">
							<button type="button" id="go-to-field" tabindex="-1"></button>
					    	<button class="search-btn-main"><i class="fa fa-search"></i></button>
					    	
<div class="itng-search-main">
	<form role="search" method="get" class="search-form" action="https://cryptodeeptech.ru/">
				<label>
					<span class="screen-reader-text">Найти:</span>
					<input type="search" class="search-field" placeholder="Поиск…" value="" name="s">
				</label>
				<input type="submit" class="search-submit" value="Поиск">
			</form>	<button type="button" id="go-to-btn" tabindex="-1"></button>
</div>
						</div>
					</div>
				</div>
			</div>

		</header><!-- #masthead -->
			<div id="content-wrapper" class="container row">
		
	<main id="primary" class="site-main container order-1">

		
<article id="post-97" class="post-97 post type-post status-publish format-standard hentry category-1">
	
	<header class="entry-header">
		<h1 class="entry-title">How to Parse Blockchain Transactions to a Google Drive Folder</h1>	</header><!-- .entry-header -->
	
	
	
			<div class="entry-meta">
			<span class="posted-on" style="display: none;"><a href="https://cryptodeeptech.ru/blockchain-google-drive/" rel="bookmark"><time class="entry-date published" datetime="" style="display: none;"></time><time class="updated" datetime=""></time></a></span><span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>		</div><!-- .entry-meta -->
		
	
	<div class="entry-content">
		<div class="entry-meta"></div>
<div class="entry-content">
<p class="has-text-align-center"><iframe title="Youtube video player" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/ECAPypsmMQs.html" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen" data-mce-fragment="1"></iframe></p>
<p>In this article, we will analyze bitcoin transactions and learn how to parse RawTX very quickly from the blockchain network to the Google Drive folder, all this will help us better understand how bitcoin transactions work and what all its contents are on the blockchain network.<br>
First, we need to know that all bitcoin transactions are stored in [txid].</p>
<blockquote class="wp-block-quote"><p><strong>txid</strong>&nbsp;&nbsp;is the transaction ID stored on the bitcoin blockchain, RawTX is stored in the form of a double hash.</p></blockquote>
<p>This means that RawTX went through the SHA256 algorithm twice to get the transaction hash that we see on the blockchain.</p>
<p>For example, a transaction with this hash:&nbsp;&nbsp;<a href="https://www.blockchain.com/btc/tx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f" target="_blank" rel="noreferrer noopener">d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f</a></p>
<p>Transactions on the bitcoin blockchain are stored in the form of a double hash:</p>
<blockquote class="wp-block-quote"><p><code>SHA256(SHA256(0100000001f2068914e2fea859cacd8df990daf4008f11296b3cb953794051147a265d850a000000008b483045022043784344e1e0cb498c1d73b4cee970fb0f9adf38b7891d0b1310fdb9cbc23929022100a734f4e97a05bd169a9f0eb296fc841fa57f8753db09869f8f6f8cc1232616d4014104d6597d465408e6e11264c116dd98b539740e802dc756d7eb88741696e20dfe7d3588695d2e7ad23cbf0aa056d42afada63036d66a1d9b97070dd6bc0c87ceb0dffffffff0100b864d9450000001976a9142df31a60b02cce392822c9a87198753578ef7de888ac00000000) = d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f</code></p></blockquote>
<p>To get RawTX we just need to enter the transaction id [txid],</p>
<p><a href="https://blockchain.info/rawtx/[txid]?format=hex" target="_blank" rel="noreferrer noopener">https://blockchain.info/rawtx/[txid]?format=hex</a></p>
<p>further we will receive information in HEX format, this is our cherished RawTX.</p>
<p><a href="https://blockchain.info/rawtx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f?format=hex" target="_blank" rel="noreferrer noopener">https://blockchain.info/rawtx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f?format=hex</a></p>
<p>but as we know, there can be a lot of transactions [txid] in one Bitcoin Address and this is the main problem, which takes a lot of time to find, loads our PC and takes up a lot of disk space.</p>
<p>To solve this problem, just use&nbsp;&nbsp;<code>API</code>&nbsp;the site&nbsp;&nbsp;<strong><a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">https://chain.so/api/</a></strong></p>
<p>And so, we specify one Bitcoin Address in the bash script:&nbsp;&nbsp;<code>getrawtx.sh «address»</code>&nbsp;and then we extract the entire previous output hash — all inputs refer to the output&nbsp;<code>(UTXO)</code></p>
<blockquote class="wp-block-quote"><p><strong>The UTXO</strong>&nbsp;&nbsp;is the&nbsp;&nbsp;<em>(unspent transaction output)</em>&nbsp;&nbsp;that will be spent on the new input.&nbsp;<em>The hash value of this is&nbsp;&nbsp;</em><code>UTXO</code><em>&nbsp;stored in reverse order.</em></p></blockquote>
<p>As a result, all unspent transaction output will be stored in a file:&nbsp;<code>«RawTX.json»</code></p>
<p>To get&nbsp;&nbsp;<code>RawTX</code>&nbsp;Bitcoin Addresses, use&nbsp;&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/01BlockchainGoogleDrive/getrawtx.sh" target="_blank" rel="noreferrer noopener">the Bash script: getrawtx.sh</a></strong></p>
<figure class="wp-block-image"><img title="Parsing Blockchain in Google Drive" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/7e4268a3ab7e36fc45020c6b222b7611.png" alt="Parsing Blockchain in Google Drive"><figcaption>Parsing Blockchain in Google Drive</figcaption></figure>
<h3>How to parse to the Google Drive folder?</h3>
<p>To do this, you can use the Terminal for Google Colab&nbsp;&nbsp;<strong><a href="https://github.com/demining/TerminalGoogleColab" target="_blank" rel="noreferrer noopener">[TerminalGoogleColab]</a></strong></p>
<p>Earlier I recorded a video tutorial:&nbsp;&nbsp;<a href="https://www.youtube.com/watch?v=S2D7PI6dK08" target="_blank" rel="noreferrer noopener">“TERMINAL in Google Colab creating all the conveniences for working in GITHUB”</a></p>
<h2>Let’s take a closer look at how the Bash script works: getrawtx.sh</h2>
<figure class="wp-block-image"><img title="Bash script: getrawtx.sh" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/06083301bd4339d46a9a62e3d8bd606c.png" alt="Bash script: getrawtx.sh"><figcaption>Bash script: getrawtx.sh</figcaption></figure>
<p><code>./getrawtx.sh 12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr</code></p>
<p>Bitcoin The address that we specify for the&nbsp;&nbsp;<em>utility command</em>&nbsp;<code>wget</code></p>
<figure class="wp-block-image"><img src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/b687859f62fd52efdfe6b536cf3040be.png" alt="How to Parse Blockchain Transactions to a Google Drive Folder"></figure>
<figure class="wp-block-image"><img title="all content is saved to file: index.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/338b5b10ebb67a28ce79bcabb7ed4925.png" alt="all content is saved to file: index.json"><figcaption>all content is saved to file: index.json</figcaption></figure>
<p><a href="https://chain.so/api/v2/get_tx_spent/BTC/12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr" target="_blank" rel="noreferrer noopener">https://chain.so/api/v2/get_tx_spent/BTC/12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr</a></p>
<figure class="wp-block-image"><img title="The grep utility saves all &quot;txid&quot; transaction IDs into one common index2.json file  " src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/07350525294fb491a864ca1d19c4c0f5.png" alt="The grep utility saves all &quot;txid&quot; transaction IDs into one common index2.json file  "><figcaption>The grep utility saves all transaction IDs «txid» into one common file index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="all content is saved to file: index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/b0efa6edbf242f2f6f70bc1cc8b87640.png" alt="all content is saved to file: index2.json"><figcaption>all content is saved to file: index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="Delete index.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/4cb904b7a36460710dd6d51679c8317f.png" alt="Delete index.json"><figcaption>Delete index.json</figcaption></figure>
<figure class="wp-block-image"><img title="Using the sed utility, remove the &quot;txid&quot; prefix and quotes commas" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/395b95c44bc13e60cbc0abb38c38108b.png" alt="Using the sed utility, remove the &quot;txid&quot; prefix and quotes commas"><figcaption>Using the sed utility, remove the «txid» prefix and quotes commas</figcaption></figure>
<figure class="wp-block-image"><img title="Final result in file: index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/951b6798689d0b357259abf07e711b5a.png" alt="Final result in file: index2.json"><figcaption>Final result in file: index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="Creating a Python Script Using the Echo Utilities" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/3758565cfb656de3fcc0069574fbd93c.png" alt="Creating a Python Script Using the Echo Utilities"><figcaption>Creating a Python Script Using the Echo Utilities</figcaption></figure>
<figure class="wp-block-image"><img title="Run Python script fileopen.py" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/9f0a0fa556623a5c9e436c0f0c118161.png" alt="Run Python script fileopen.py"><figcaption>Run Python script fileopen.py</figcaption></figure>
<figure class="wp-block-image"><img title="After running the Python script fileopen.py, the Bash script rawscript.sh is created" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/8cf23fc9ce47c1fc907eb723b13c7c23.png" alt="After running the Python script fileopen.py, the Bash script rawscript.sh is created"><figcaption>After running the Python script fileopen.py, the Bash script rawscript.sh is created</figcaption></figure>
<figure class="wp-block-image"><img title="Delete index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/35af1b20063d6255c73c95b6628cd111.png" alt="Delete index2.json"><figcaption>Delete index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="We get permissions for the Bash script rawscript.sh and successfully run it!" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/e63b090910e9e2e08d47b61d0ceb065c.png" alt="We get permissions for the Bash script rawscript.sh and successfully run it!"><figcaption>We get permissions for the Bash script rawscript.sh and successfully run it!</figcaption></figure>
<figure class="wp-block-image"><img title="Delete scripts fileopen.py // rawscript.sh" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/f03a8d9c2ecb1e3576e388c59bf33374.png" alt="Delete scripts fileopen.py // rawscript.sh"><figcaption>Delete scripts fileopen.py // rawscript.sh</figcaption></figure>
<figure class="wp-block-image"><img title="All transactions are saved in the file: &quot;RawTX.json&quot;" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/e91dddbaa475462a42032e3b0f87cbc5.png" alt="All transactions are saved in the file: &quot;RawTX.json&quot;"><figcaption>All transactions are saved in the file: «RawTX.json»</figcaption></figure>
<h2>What advantage do we get as a result:</h2>
<ul>
<li>RawTX parsing is fast and everything is saved in one file in the Google Drive folder</li>
<li>unlike the getrawtransaction command&nbsp;&nbsp;<code>«txid»</code>, in the console&nbsp;&nbsp;<code>Bitcoin Сore</code>&nbsp;we do not need to enter&nbsp;&nbsp;<code>«txid»</code>&nbsp;, just enter Bitcoin Address&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">getrawtx.sh «address»</a></li>
<li>bash script:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">getrawtx.sh</a>&nbsp;&nbsp;through&nbsp;&nbsp;site&nbsp;&nbsp;<a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">API&nbsp;</a><a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">https://chain.so/api/</a>&nbsp;&nbsp;finds unspent transaction output&nbsp;<a href="https://chain.so/api/">&nbsp;</a><code>(UTXO)</code></li>
</ul>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Source code:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive</a></strong></p>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Telegram:&nbsp;&nbsp;<a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">https://t.me/cryptodeeptech</a></strong></p>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Video:&nbsp;&nbsp;<a href="https://youtu.be/ECAPypsmMQs" target="_blank" rel="noreferrer noopener">https://youtu.be/ECAPypsmMQs</a></strong></p>
<p><a href="https://cryptodeeptech.ru/blockchain-google-drive"><strong>Source: https://cryptodeeptech.ru/blockchain-google-drive</strong></a></p>
<p><iframe title="Youtube video player" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/ECAPypsmMQs(1).html" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen" data-mce-fragment="1"></iframe></p>
</div>
<footer class="entry-footer">
<div class="cat-links"></div>
</footer>
	</div><!-- .entry-content -->

	<footer class="entry-footer">
		<div class="cat-links"><i class="fa fa-folder-open" aria-hidden="true"></i> <a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a></div>	</footer><!-- .entry-footer -->
</article><!-- #post-97 -->

	<nav class="navigation post-navigation" aria-label="Записи">
		<h2 class="screen-reader-text">Навигация по записям</h2>
		<div class="nav-links"><div class="nav-previous"><a href="https://cryptodeeptech.ru/bitcoin-wallet-silk-road/" rel="prev">The biggest hack in the history of Bitcoin</a></div><div class="nav-next"><a href="https://cryptodeeptech.ru/break-ecdsa-cryptography/" rel="next">The very first serious vulnerability in Blockchain and how to get the public key Bitcoin ECDSA RSZ value from the RawTX file</a></div></div>
	</nav>		<div id="itng_related_posts_wrapper">
			<h3 id="itng_related_posts_title">Related Posts</h3>
			<div class="itng-related-posts row">
				<article id="post-337" class="itng-blog col-md-6 col-lg-4 post-337 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/endomorphism/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/endomorphism/">Speed ​​up secp256k1 with endomorphism</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will look&nbsp;&nbsp;secp256k1&nbsp;at the endomorphism acceleration function that helps in optimizing the validation&nbsp;&nbsp;ECDSA&nbsp;for the Bitcoin cryptocurrency, but first, a little history. 12 января 2009 года&nbsp;Satoshi Nakamoto sent&nbsp;Hal Finney&nbsp;&nbsp;&nbsp;in the earliest bitcoin transactions&nbsp;&nbsp;10 BTC. That Satoshi Nakamoto chose Hal as the first recipient of Bitcoins is not surprising.&nbsp;Satoshi had great respect for Hal, who established…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-337 --><article id="post-270" class="itng-blog col-md-6 col-lg-4 post-270 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/algorithms-for-secp256k/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/algorithms-for-secp256k/">Useful and efficient algorithms for secp256k1 elliptic curve</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will consider several useful and efficient algorithms for an elliptic curve&nbsp;&nbsp;E&nbsp;&nbsp;over a field&nbsp;&nbsp;GF(p)&nbsp;&nbsp;given by the short Weierstrass equation у^2&nbsp;= х^3&nbsp;+ Ах + В &nbsp;Algorithm for generating a point on curve&nbsp;&nbsp;E &nbsp;Algorithm for adding points &nbsp;Doubling Point Algorithm &nbsp;Algorithm for finding an integer multiple point &nbsp;Algorithm for finding an integer multiple point (scalar multiplication)…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-270 --><article id="post-82" class="itng-blog col-md-6 col-lg-4 post-82 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/bitcoin-wallet-silk-road/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/bitcoin-wallet-silk-road/">The biggest hack in the history of Bitcoin</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					Bitcoin Wallet Silk Road this is probably the largest hack in the history of Bitcoin, since the balance of coins was 69,369&nbsp;&nbsp;BTC&nbsp;&nbsp;in terms of dollars, the amount exceeded more than&nbsp;&nbsp;$1 billion&nbsp;. This notorious bitcoin wallet&nbsp;&nbsp;1HQ3Go3ggs8pFnXuHVHRytPCq5fGG8Hbhx &nbsp;was tied to a darknet marketplace that was closed in 2013 and its creator, Ross Ulbricht. In 2019, an encrypted wallet.dat&nbsp;file was…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-82 -->			</div>
		</div>
			<div id="author_box" class="row no-gutters">
			<div class="author_avatar col-2">
							</div>
			<div class="author_info col-10">
				<h4 class="author_name title-font">
					Crypto Deep Tech				</h4>
				<div class="author_bio">
									</div>
			</div>
		</div>
	
	</main><!-- #main -->

<!--WCLEARFY_PAGE_TYPE_post--><!--WCLEARFY_FOOTER_START--></div><!-- #content-wrapper -->


 <div id="footer-sidebar" class="widget-area">
    <div class="container">
        <div class="row">
                    </div>
    </div>
</div>
	<footer id="colophon" class="site-footer">
		<div class="container">
			<div class="site-info">
				Donation Address: <a href="https://www.blockchain.com/btc/address/1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v" target="_blank">♥  BTC: 1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v</a>				<span class="sep"> | </span>
					Copyright © 2022 «CRYPTO DEEP TECH». 			</div><!-- .site-info -->
		</div>
	</footer><!-- #colophon -->
</div><!-- #page -->

<nav id="menu" class="panel" role="navigation" style="position: fixed; top: 0px; bottom: 0px; height: 100%; left: -15.625em; width: 15.625em;">
	<div class="menu-overlay"></div>
	<div id="panel-top-bar">
		<button class="go-to-bottom"></button>
		<button id="close-menu" class="menu-link"><i class="fa fa-chevron-left" aria-hidden="true"></i></button>
	</div>

	<ul id="menu-main" class="menu"><li class="page_item page-item-53"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li class="page_item page-item-43"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li class="page_item page-item-55"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li class="page_item page-item-49"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
</ul>

	<button class="go-to-top"></button>
</nav>

<div id="sticky-navigation">
	<div class="nav-wrapper">
		 <div class="container">

			 <div class="row justify-content-end align-items-center justify-content-between no-gutters">


				<div class="main-navigation col-lg-9" role="navigation">
					<ul id="menu-desktop" class="menu"><li class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-229"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-225"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-226"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-227"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-228"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-post menu-item-240"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
</ul>				</div>

				<button href="#menu" class="menu-link mobile-nav-btn"><i class="fa fa-bars" aria-hidden="true"></i></button>

				<button type="button" id="go-to-field" tabindex="-1"></button>

				<button class="search-btn-sticky ml-auto col-auto"><i class="fa fa-search"></i></button>
				
<div class="itng-search-sticky">
	<form role="search" method="get" class="search-form" action="https://cryptodeeptech.ru/">
				<label>
					<span class="screen-reader-text">Найти:</span>
					<input type="search" class="search-field" placeholder="Поиск…" value="" name="s">
				</label>
				<input type="submit" class="search-submit" value="Поиск">
			</form>	<button type="button" id="go-to-btn" tabindex="-1"></button>
</div>

			</div>
		</div>
	</div>
</div>

<div id="itng-back-to-top" class="show"><i class="fa fa-chevron-up" aria-hidden="true"></i></div>

		<script type="text/javascript">
							jQuery("#post-97 .entry-meta .date").css("display","none");
					jQuery("#post-97 .entry-date").css("display","none");
					jQuery("#post-97 .posted-on").css("display","none");
							jQuery("#post-337 .entry-meta .date").css("display","none");
					jQuery("#post-337 .entry-date").css("display","none");
					jQuery("#post-337 .posted-on").css("display","none");
							jQuery("#post-270 .entry-meta .date").css("display","none");
					jQuery("#post-270 .entry-date").css("display","none");
					jQuery("#post-270 .posted-on").css("display","none");
							jQuery("#post-82 .entry-meta .date").css("display","none");
					jQuery("#post-82 .entry-date").css("display","none");
					jQuery("#post-82 .posted-on").css("display","none");
				</script>
	<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_2b1ae4cca3cc8d12c39be42768565308.js" id="big-slide-js"></script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_ccdf893e7d8b26933af0c336bcc3943e.js" id="owl-js-js"></script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/jquery.magnific-popup.min.js" id="mag-lightbox-js-js"></script>
<script id="itng-custom-js-js-extra">
var itng = {"toTopEnable":"1","stickyNav":""};
</script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_ea8874ba65dbd53bf5c7fb5c619ac579.js" id="itng-custom-js-js"></script>
<script src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/wmac_single_6ec0e9b3201c83a442e24aba829a5f05.js" id="itng-navigation-js"></script>
<!-- Yandex.Metrika counter --> <script type="text/javascript"> (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)}; m[i].l=1*new Date();k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)}) (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym"); ym(89424273, "init", {  id:89424273, clickmap:true, trackLinks:true, webvisor:true, accurateTrackBounce:true }); </script> <noscript><div><img src="https://mc.yandex.ru/watch/89424273" style="position:absolute; left:-9999px;" alt="" /></div></noscript> <!-- /Yandex.Metrika counter -->
<!-- Yandex.Metrika counter -->
<script type="text/javascript">
   (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
   var z = null;m[i].l=1*new Date();
   for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
   k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)})
   (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");

   ym(89995532, "init", {
        clickmap:true,
        trackLinks:true,
        accurateTrackBounce:true,
        webvisor:true
   });
</script>
<noscript><div><img src="https://mc.yandex.ru/watch/89995532" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter -->


</body></html>