Штош, это репозиторий с разными полезными материалами для оформления документов в Homebrewery. Для шрифтов надо вставить в стиль документа во это (я взял это из одного крутейшего документа "Божественный гримуар"):

@import url('https://rawcdn.githack.com/spechurkin/fonts/5803193c6919fc9e1390cae05d7127e39f3fb8fe/fantasy-fonts.css');

body {
  counter-reset: page-numbers -1;
}

.page {
	width: 210mm;
	height: 296.8mm;
}

.page:nth-child(even) {
  background-image: url(https://i.imgur.com/TiA3pDd.png);
  background-size: 100% 100%;
}

.page:nth-child(odd) {
  background-image: url(https://i.imgur.com/vS5uHJn.png);
  background-size: 100% 100%;
}

.page:nth-child(even) .pageNumber {
  right: 2px;
  left: auto;
}

.page:nth-child(odd) .pageNumber {
  left: 2px;
  right: auto;
}

.page:nth-child(even) .inside {
  right: 80px;
  left: auto;
  text-align: right;
}

.page:nth-child(odd) .inside {
  left: 80px;
  right: auto;
  text-align: left;
}

.page:after {
  display: none;
}

.page:has(.frontCover) .logo img {
  width: 3cm;
  height: 3cm;
}

.page h1, .page h2, .page h3, .page h4, .page h5, .page h6, .page .artist h5,
.page .monster h1, .page .monster h2, .page .monster h3, .page .monster h4, .page .monster h5, .page .monster h6 {
  font-family: 'Alegreya SC';
}

.page h2 {
  font-size: 26px;
}

.page h3 {
  font-size: 20px;
}

.page p, .page a, .page dl, .page li, .page td, .page th, .page .artist {
  font-family: 'Mookmania';
  font-size: 11px;
}

.page .inside, .page .pageNumber {
  font-family: 'Mookmania';
  font-size: 14px;
  color: #58180D;
  text-shadow: 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white, 0 0 5px white;
}

.page .inside {
  width: 350px;
}

.page:has(.frontCover) .footnote p {
  font-size: 22px;
  filter: drop-shadow(0 0 1px black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black) drop-shadow(0 0 0 black);
}

.page:has(.frontCover) h1, .page:has(.frontCover) h2, .page:has(.frontCover) .banner,
.page:has(.insideCover) h1, .page:has(.insideCover) h2, .page:has(.insideCover) .banner {
  font-family: 'Nodesto';
}

.page:has(.frontCover) .banner {
  padding-left: 20px;
  padding-bottom: 12px;
}

.page h1+p::first-letter {
  font-family: 'Volbera';
  margin-bottom: -7px;
  color: black;
}

.page h1+p::first-line {
  font-size: inherit;
  font-style: initial;
  font-variant: none;
}

.page:has(.insideCover) h2 {
  letter-spacing: .2cm;
}

.page .quote>p {
  font-family: 'Mookmania Italic';
}

.page .quote>p:first-child::first-line {
  font-size: inherit;
  font-style: initial;
  font-variant: none;
}

.page a {
  text-decoration: none;
  color: black;
}

.page a:hover {
  text-decoration: underline;
}

.footer p {
  text-align: center;
  font-size:  10.5px;
}

.page .toc h5{
  color: #58180D;
}

.diary p {
  font-family: "Gunny Rewritten";
  font-size: 22px;
  color: #3c3a37;
}

.page .note {
  background-color: #f6e5d4;
}

.page table tbody tr:nth-child(odd) {
  background-color: #fbe9b5;
}

.page .spells p {
  font-size: 11.75px;
}

.big_table table tbody tr td {
  padding: 2px 11.5px;
}

.page .lastStage h1 {
  color: #ff2a1a;
  font-size: 4em;
  text-align: center;
  text-decoration: none;
}

.page .lastStage .artists a {
	color: #ac8f66;
}

.page .lastStage a, .page .lastStage p, .page .lastStage h5 {
	color: white;
	font-size: 1.1em;
}
