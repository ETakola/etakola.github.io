
---
layout: default
title: Curriculum Vitae
permalink: /resume/
---

<style>
/* AUTUMN FIELD JOURNAL — complete, self-contained design */

.atn-cv {
  --atn-ink: #352f2d;
  --atn-muted: #70665f;
  --atn-wine: #593f43;
  --atn-rust: #9d543c;
  --atn-rust-dark: #753e34;
  --atn-ochre: #b27b40;
  --atn-olive: #61704d;
  --atn-paper: #fffefa;
  --atn-cream: #faf4eb;
  --atn-stroke: #e7d9c8;
  box-sizing: border-box;
  width: min(100% - 34px, 1040px);
  margin: 32px auto 70px;
  padding: 0 0 26px;
  color: var(--atn-ink);
  background: var(--atn-paper);
  font: 400 15.5px/1.72 -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}

.atn-cv *,
.atn-cv *::before,
.atn-cv *::after { box-sizing: border-box; }

.atn-cv h1,
.atn-cv h2,
.atn-cv h3,
.atn-cv p,
.atn-cv ul { margin-top: 0; }

.atn-cv h2, .atn-cv h3 { border: 0; }
.atn-cv p { margin-bottom: 12px; }

.atn-cv a {
  color: var(--atn-rust-dark);
  text-decoration: none;
  border-bottom: 1px solid #cba88d;
  transition: color .18s ease, border-color .18s ease;
}
.atn-cv a:hover,
.atn-cv a:focus {
  color: var(--atn-rust);
  border-bottom-color: currentColor;
}
.atn-cv a:focus-visible {
  outline: 2px solid var(--atn-ochre);
  outline-offset: 3px;
}

/* Nature-themed cover */
.atn-cv .atn-hero {
  overflow: hidden;
  border-radius: 23px;
  border: 1px solid #ddcbb5;
  border-top: 7px solid var(--atn-rust);
  background: #f7efe3;
  box-shadow: 0 14px 36px rgba(62,45,32,.095);
}
.atn-cv .atn-hero-main {
  display: grid;
  grid-template-columns: minmax(0, 1.25fr) minmax(0, .83fr);
  align-items: center;
  gap: 27px;
  padding: 36px 35px 25px 44px;
}
.atn-cv .atn-eyebrow {
  display: flex;
  align-items: center;
  gap: 9px;
  color: var(--atn-olive);
  font-size: 10.5px;
  font-weight: 750;
  letter-spacing: .16em;
  text-transform: uppercase;
}
.atn-cv .atn-eyebrow svg {
  width: 21px;
  height: 21px;
  flex: 0 0 auto;
}
.atn-cv .atn-hero h1 {
  color: var(--atn-wine);
  font: 400 clamp(37px, 4.7vw, 53px)/1.1 Georgia, "Times New Roman", serif;
  letter-spacing: -.035em;
  margin: 24px 0 17px;
}
.atn-cv .atn-hero h1 span { color: var(--atn-rust); }
.atn-cv .atn-name-rule {
  display: block;
  width: 72px;
  height: 3px;
  background: var(--atn-ochre);
  border-radius: 3px;
  margin: 0 0 18px;
}
.atn-cv .atn-subtitle {
  max-width: 490px;
  margin-bottom: 12px;
  color: #4e493f;
  font-size: 16px;
  font-weight: 600;
  letter-spacing: -.01em;
}
.atn-cv .atn-affiliation {
  font-size: 13px;
  color: var(--atn-muted);
  margin-bottom: 0;
}
.atn-cv .atn-art {
  min-width: 0;
  overflow: hidden;
  border-radius: 115px 115px 17px 17px;
  background: linear-gradient(157deg, #e9dfc9, #d7ddc0 77%);
  border: 1px solid rgba(104,108,66,.2);
  box-shadow: inset 0 2px 15px rgba(115,100,66,.05);
  position: relative;
}
.atn-cv .atn-art svg {
  display: block;
  width: 100%;
  height: auto;
}
.atn-cv .atn-art-caption {
  position: absolute;
  bottom: 9px;
  left: 0;
  right: 0;
  color: #fff8ec;
  text-shadow: 0 1px 2px rgba(28,47,29,.6);
  font: 600 9px/1.4 -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  letter-spacing: .14em;
  text-align: center;
  text-transform: uppercase;
}

/* Contact links */
.atn-cv .atn-social {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 8px 9px;
  padding: 15px 37px 18px 44px;
  background: #fffaf2;
  border-top: 1px solid #e5d7c4;
}
.atn-cv .atn-social a {
  color: var(--atn-rust-dark);
  font-size: 12px;
  font-weight: 650;
  line-height: 1.5;
  background: #fffefa;
  border: 1px solid #dcc5ad;
  padding: 6px 12px;
  border-radius: 40px;
}
.atn-cv .atn-social a:hover {
  background: #f1e5d2;
  border-color: var(--atn-rust);
}

/* Navigation */
.atn-cv .atn-nav {
  display: flex;
  gap: 3px;
  flex-wrap: wrap;
  padding: 19px 2px 11px;
  margin: 0 0 16px;
  border-bottom: 1px solid var(--atn-stroke);
}
.atn-cv .atn-nav a {
  display: inline-block;
  padding: 5px 12px;
  border: 0;
  border-radius: 40px;
  color: var(--atn-muted);
  font-size: 12px;
  font-weight: 700;
}
.atn-cv .atn-nav a:hover {
  background: #f2e8da;
  color: var(--atn-rust-dark);
}

/* Profile */
.atn-cv .atn-content { padding: 0 17px; }
.atn-cv .atn-profile {
  display: grid;
  grid-template-columns: minmax(0, 1.5fr) minmax(210px, .75fr);
  gap: 26px;
  align-items: stretch;
  padding: 12px 0 23px;
}
.atn-cv .atn-profile-text {
  border-left: 3px solid var(--atn-ochre);
  padding: 8px 15px 7px 22px;
}
.atn-cv .atn-kicker {
  font-size: 10.5px;
  color: var(--atn-rust);
  font-weight: 800;
  text-transform: uppercase;
  letter-spacing: .15em;
  margin: 0 0 8px;
}
.atn-cv .atn-profile-text p:last-child { margin-bottom: 0; }
.atn-cv .atn-quickfacts {
  background: var(--atn-cream);
  border: 1px solid var(--atn-stroke);
  border-radius: 13px;
  padding: 16px 19px;
}
.atn-cv .atn-fact + .atn-fact {
  border-top: 1px solid #e8daca;
  padding-top: 10px;
  margin-top: 10px;
}
.atn-cv .atn-fact strong {
  color: var(--atn-wine);
  font-size: 13.8px;
  display: block;
  line-height: 1.45;
}
.atn-cv .atn-fact span {
  color: var(--atn-muted);
  font-size: 12px;
  display: block;
  line-height: 1.5;
}

/* Sections */
.atn-cv section.atn-section {
  margin: 20px 0 40px;
  scroll-margin-top: 24px;
}
.atn-cv .atn-heading {
  display: flex;
  gap: 15px;
  align-items: baseline;
  border-bottom: 1px solid var(--atn-stroke);
  padding-bottom: 11px;
  margin-bottom: 23px;
}
.atn-cv .atn-heading .atn-n {
  flex: 0 0 auto;
  color: var(--atn-ochre);
  font: 400 15px Georgia, serif;
}
.atn-cv .atn-heading h2 {
  font: 400 29px/1.22 Georgia, "Times New Roman", serif;
  letter-spacing: -.02em;
  color: var(--atn-wine);
  margin: 0;
}

/* Career and education */
.atn-cv .atn-card {
  border-left: 2px solid #d6b18b;
  padding: 1px 0 1px 22px;
  margin: 0 0 26px 5px;
  position: relative;
}
.atn-cv .atn-card::before {
  content: "";
  position: absolute;
  width: 9px;
  height: 9px;
  background: var(--atn-rust);
  border: 3px solid var(--atn-paper);
  border-radius: 50%;
  left: -5px;
  top: 7px;
  box-sizing: content-box;
}
.atn-cv .atn-card:last-child { margin-bottom: 0; }
.atn-cv .atn-card-head {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  flex-wrap: wrap;
  gap: 4px 16px;
}
.atn-cv .atn-card h3 {
  color: var(--atn-ink);
  font-size: 16.4px;
  line-height: 1.4;
  margin: 0 0 4px;
  font-weight: 750;
}
.atn-cv .atn-date {
  white-space: normal;
  color: var(--atn-rust);
  font-size: 12px;
  font-weight: 750;
  letter-spacing: .02em;
}
.atn-cv .atn-org {
  color: var(--atn-olive);
  font-weight: 650;
  margin-bottom: 2px;
}
.atn-cv .atn-note {
  color: var(--atn-muted);
  font-size: 13.5px;
  margin-bottom: 5px;
}
.atn-cv .atn-columns {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
}
.atn-cv .atn-minicard {
  background: var(--atn-cream);
  border: 1px solid var(--atn-stroke);
  border-radius: 12px;
  padding: 18px 21px;
}
.atn-cv .atn-minicard h3 {
  color: var(--atn-rust-dark);
  font: 400 20px Georgia, serif;
  margin: 0 0 8px;
}
.atn-cv .atn-minicard p {
  margin: 0;
  font-size: 13.5px;
}

/* Awards */
.atn-cv .atn-honour {
  display: grid;
  grid-template-columns: 60px minmax(0,1fr);
  gap: 16px;
  margin: 0 0 18px;
  align-items: baseline;
}
.atn-cv .atn-honour .atn-year {
  color: var(--atn-ochre);
  font: 400 18px Georgia, serif;
}
.atn-cv .atn-honour strong {
  display: block;
  line-height: 1.45;
}
.atn-cv .atn-honour p {
  font-size: 13.5px;
  color: var(--atn-muted);
  margin: 2px 0 0;
}

/* Lists */
.atn-cv .atn-list {
  list-style: none;
  margin: 0;
  padding: 0;
}
.atn-cv .atn-list li {
  position: relative;
  padding-left: 19px;
  margin: 0 0 11px;
}
.atn-cv .atn-list li::before {
  content: "";
  width: 6px;
  height: 6px;
  border-radius: 50%;
  position: absolute;
  left: 1px;
  top: .7em;
  background: var(--atn-ochre);
}

/* Teaching */
.atn-cv .atn-course {
  padding: 0 0 18px;
  margin-bottom: 17px;
  border-bottom: 1px dashed var(--atn-stroke);
}
.atn-cv .atn-course:last-child {
  padding-bottom: 0;
  margin-bottom: 0;
  border-bottom: 0;
}
.atn-cv .atn-course h3 {
  font-size: 15.5px;
  color: var(--atn-ink);
  margin: 0 0 4px;
  line-height: 1.5;
}
.atn-cv .atn-course p {
  margin: 0 0 3px;
  font-size: 13.5px;
  color: var(--atn-muted);
}
.atn-cv .atn-course .atn-course-title {
  color: var(--atn-olive);
  font-weight: 700;
  font-size: 14px;
}

/* Publications */
.atn-cv .atn-subhead {
  color: var(--atn-rust-dark);
  font: 400 23px/1.3 Georgia, serif;
  margin: 28px 0 14px;
}
.atn-cv .atn-introline {
  color: var(--atn-muted);
  font-size: 13.5px;
  margin: -7px 0 18px;
}
.atn-cv .atn-pubs {
  padding: 0;
  margin: 0;
  list-style: none;
}
.atn-cv .atn-pub {
  display: grid;
  grid-template-columns: 56px minmax(0,1fr);
  gap: 14px;
  border-top: 1px solid #eee4d8;
  padding: 17px 0;
}
.atn-cv .atn-pub:first-child {
  border-top: 0;
  padding-top: 4px;
}
.atn-cv .atn-pub-year {
  color: var(--atn-ochre);
  font: 400 18px Georgia, serif;
  padding-top: 2px;
}
.atn-cv .atn-pub-title {
  display: inline;
  font-size: 15.1px;
  font-weight: 740;
  line-height: 1.45;
}
.atn-cv .atn-pub p {
  margin: 5px 0 0;
  color: var(--atn-muted);
  font-size: 13.5px;
  line-height: 1.65;
  overflow-wrap: anywhere;
}
.atn-cv .atn-pub em { color: #55433b; }
.atn-cv .atn-status {
  display: inline-block;
  background: #f1e5d4;
  border: 1px solid #e7d0b7;
  color: #76503c;
  padding: 2px 7px;
  border-radius: 5px;
  font-size: 11px;
  line-height: 1.4;
  font-weight: 700;
  margin: 0 0 2px 7px;
  white-space: nowrap;
}

/* Footer */
.atn-cv .atn-footer {
  margin: 35px 17px 0;
  padding: 16px 0 0;
  border-top: 2px solid #b78355;
  color: var(--atn-muted);
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 8px 20px;
  font-size: 12px;
}

/* Mobile */
@media (max-width: 720px) {
  .atn-cv {
    font-size: 14.7px;
    width: min(100% - 20px, 1040px);
    margin: 14px auto 35px;
  }
  .atn-cv .atn-hero { border-radius: 16px; }
  .atn-cv .atn-hero-main {
    grid-template-columns: 1fr;
    gap: 18px;
    padding: 27px 23px 22px;
  }
  .atn-cv .atn-hero h1 {
    font-size: clamp(35px, 8.8vw, 49px);
    margin: 19px 0 15px;
  }
  .atn-cv .atn-subtitle { font-size: 14.5px; }
  .atn-cv .atn-art {
    width: min(100%, 340px);
    margin: 1px auto 0;
  }
  .atn-cv .atn-social { padding: 14px 21px 18px; }
  .atn-cv .atn-content { padding: 0 9px; }
  .atn-cv .atn-profile,
  .atn-cv .atn-columns {
    grid-template-columns: 1fr;
    gap: 17px;
  }
  .atn-cv .atn-heading h2 { font-size: 25px; }
  .atn-cv .atn-nav { gap: 2px; }
  .atn-cv .atn-nav a { padding: 5px 9px; }
  .atn-cv .atn-pub {
    grid-template-columns: 42px minmax(0,1fr);
    gap: 10px;
  }
  .atn-cv .atn-pub-year { font-size: 16px; }
  .atn-cv .atn-card { padding-left: 16px; }
}
@media (prefers-reduced-motion: reduce) {
  .atn-cv a { transition: none; }
}
@media print {
  .atn-cv {
    max-width: none;
    width: 100%;
    padding: 0;
    margin: 0;
    color: #222;
    background: white;
    font-size: 11pt;
  }
  .atn-cv .atn-hero {
    box-shadow: none;
    -webkit-print-color-adjust: exact;
    print-color-adjust: exact;
  }
  .atn-cv .atn-nav { display: none; }
  .atn-cv a { color: #683c2c; }
  .atn-cv section,
  .atn-cv .atn-card,
  .atn-cv .atn-pub { break-inside: avoid; }
}
</style>

<div class="atn-cv">

  <header class="atn-hero">
    <div class="atn-hero-main">
      <div class="atn-hero-copy">
        <div class="atn-eyebrow">
          <svg viewBox="0 0 24 24" aria-hidden="true" xmlns="http://www.w3.org/2000/svg">
            <path d="M5 20C7 12 10 7 19 4c-1 8-5 13-13 15" fill="none" stroke="#61704d" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
            <path d="M6 19c4-4 7-7 11-10" fill="none" stroke="#9d543c" stroke-width="1.4" stroke-linecap="round"/>
          </svg>
          Academic CV &amp; publications
        </div>
        <h1>Eleni-Elda<br><span>(Elina) Takola</span></h1>
        <span class="atn-name-rule" aria-hidden="true"></span>
        <p class="atn-subtitle">Ecologist &nbsp;&middot;&nbsp; Meta-analyst &nbsp;&middot;&nbsp; Research Group Leader</p>
        <p class="atn-affiliation">BIOECOS Group · Helmholtz Centre for Environmental Research – UFZ<br>Leipzig, Germany</p>
      </div>

      <div class="atn-art">
        <!-- Original illustration: lapwing, hare and autumn meadow -->
        <svg viewBox="0 0 450 370" role="img" aria-labelledby="atn-scene-title atn-scene-desc" xmlns="http://www.w3.org/2000/svg">
          <title id="atn-scene-title">Wildlife in an autumn meadow</title>
          <desc id="atn-scene-desc">A stylised northern lapwing and a hare, with leaves, grasses and a warm autumn sky.</desc>
          <circle cx="336" cy="98" r="59" fill="#dca361" opacity=".7"/>
          <path d="M0 246 C75 232 129 246 185 257 C260 272 329 233 450 233 L450 370 L0 370Z" fill="#b5c09a" opacity=".57"/>
          <path d="M0 285 C71 257 157 274 219 284 C313 299 359 270 450 277 L450 370 L0 370Z" fill="#8d9e78" opacity=".53"/>
          <path d="M13 211 C48 190 66 148 80 103 C84 89 92 73 106 58" fill="none" stroke="#75815b" stroke-width="4" stroke-linecap="round"/>
          <path d="M67 151 C43 146 35 127 37 108 C60 109 73 125 67 151Z" fill="#a96f46"/>
          <path d="M75 116 C94 117 109 100 110 82 C89 81 77 95 75 116Z" fill="#bd8954"/>
          <path d="M50 185 C26 185 18 166 21 149 C43 149 53 163 50 185Z" fill="#c39b66"/>
          <path d="M89 84 C66 80 63 61 72 47 C91 53 96 68 89 84Z" fill="#89996b"/>
          <path d="M27 220 C14 208 10 198 7 181" fill="none" stroke="#75815b" stroke-width="2"/>

          <!-- Lapwing -->
          <path d="M209 227 L202 310 M241 225 L240 307" stroke="#453b37" stroke-width="3.8" stroke-linecap="round"/>
          <path d="M202 310 l-17 4 m17-4 l13 6 m-13-6 l-6 8 M240 307 l-17 5 m17-5 l17 5 m-17-5 l-5 7" fill="none" stroke="#453b37" stroke-width="3" stroke-linecap="round"/>
          <path d="M155 192 C151 168 170 148 199 147 C215 147 232 152 244 166 C244 152 250 143 258 129 C264 116 260 102 268 92 C275 83 288 82 296 91 C301 97 302 104 299 112 C290 123 280 125 276 144 C270 161 278 171 275 188 C268 213 243 229 215 230 C189 231 167 217 155 192Z" fill="#494142"/>
          <path d="M288 90 C288 70 284 55 276 36 M291 90 C298 65 297 48 294 25 M293 91 C305 74 314 67 327 57" fill="none" stroke="#494142" stroke-width="4.2" stroke-linecap="round"/>
          <path d="M298 104 L329 110 L299 116Z" fill="#92573b"/>
          <circle cx="288" cy="99" r="2.6" fill="#f4e7cc"/>
          <path d="M158 177 C179 159 207 158 249 176 C241 199 222 217 200 220 C184 209 167 196 158 177Z" fill="#ad634c"/>
          <path d="M170 180 C196 172 215 176 242 188 C231 202 214 211 200 214 C184 205 173 192 170 180Z" fill="#d5b394"/>
          <path d="M177 170 C196 168 218 170 249 176 C240 187 224 193 209 194 C196 187 184 180 177 170Z" fill="#6d4b48"/>
          <path d="M158 189 L132 198 L157 200" fill="#494142"/>

          <!-- Hare -->
          <path d="M343 244 C335 224 328 199 330 169 C343 164 352 187 353 217 C359 195 370 170 380 171 C390 180 378 217 368 244Z" fill="#935e45"/>
          <path d="M339 177 C341 193 344 213 345 224 M379 180 C372 192 365 209 362 224" fill="none" stroke="#d7ab81" stroke-width="3.1" stroke-linecap="round"/>
          <path d="M334 241 C347 229 372 226 386 240 C394 251 395 260 395 270 C411 280 420 297 415 314 C408 337 381 337 354 336 C328 336 306 324 301 303 C295 281 309 256 329 246Z" fill="#9c6e51"/>
          <path d="M334 270 C341 251 360 243 374 249" fill="none" stroke="#bc8b68" stroke-width="4" stroke-linecap="round"/>
          <path d="M302 295 C284 290 284 309 302 313 C310 307 311 301 302 295Z" fill="#faf0d8"/>
          <ellipse cx="367" cy="247" rx="3.1" ry="3.6" fill="#372f2d"/>
          <path d="M391 261 l10 3" stroke="#563a34" stroke-width="2.4" stroke-linecap="round"/>
          <path d="M344 333 c14-13 33-10 46 0" fill="none" stroke="#7c5745" stroke-width="5" stroke-linecap="round"/>

          <!-- Meadow -->
          <path d="M0 322 Q68 309 143 323 T293 323 T450 320 L450 370 H0Z" fill="#687a59"/>
          <g fill="none" stroke="#526b4f" stroke-width="3" stroke-linecap="round">
            <path d="M23 341l-9-46 M23 341l21-36 M23 341l-16-19 M115 341l-14-43 M115 341l25-38 M154 341l-4-32 M284 341l19-48 M284 341l-10-36 M424 342l-16-44 M424 342l18-37"/>
          </g>
          <g fill="#bf8d55">
            <ellipse cx="14" cy="295" rx="4" ry="9" transform="rotate(-17 14 295)"/>
            <ellipse cx="102" cy="297" rx="4" ry="9" transform="rotate(-19 102 297)"/>
            <ellipse cx="302" cy="292" rx="4" ry="9" transform="rotate(15 302 292)"/>
            <ellipse cx="408" cy="297" rx="4" ry="9" transform="rotate(-16 408 297)"/>
          </g>
          <path d="M0 352 Q115 340 220 353 T450 345 L450 370 H0Z" fill="#526b4d" opacity=".76"/>
        </svg>
        <span class="atn-art-caption">Wildlife · Landscapes · Ecology</span>
      </div>
    </div>

    <div class="atn-social" aria-label="Academic and professional profiles">
      <a href="mailto:elina.takola@gmail.com">Email</a>
      <a href="https://orcid.org/0000-0003-1268-5513">ORCID</a>
      <a href="https://www.ufz.de/index.php?en=50117">UFZ profile</a>
      <a href="https://scholar.google.com/citations?user=kmt3hFoAAAAJ&amp;hl=en">Google Scholar</a>
      <a href="https://de.linkedin.com/in/dr-elina-takola">LinkedIn</a>
      <a href="https://github.com/ETakola">GitHub</a>
      <a href="https://www.researchgate.net/profile/Elina-Takola">ResearchGate</a>
    </div>
  </header>

  <nav class="atn-nav" aria-label="On this page">
    <a href="#profile">Profile</a>
    <a href="#career">Career</a>
    <a href="#education">Education</a>
    <a href="#honours">Honours</a>
    <a href="#teaching">Teaching</a>
    <a href="#service">Service</a>
    <a href="#publications">Publications</a>
  </nav>

  <div class="atn-content">

    <!-- PROFILE -->
    <div class="atn-profile" id="profile">
      <div class="atn-profile-text">
        <p class="atn-kicker">Research profile</p>
        <p>Greek ecologist and meta-analyst leading the <a href="https://www.ufz.de/index.php?en=37501">BIOECOS Group</a> at the Helmholtz Centre for Environmental Research – UFZ in Leipzig, Germany. My research focuses on evidence synthesis and relationships between organisms and their environments across multiple scales, with a strong commitment to international collaboration, scientific service and open science.</p>
      </div>
      <aside class="atn-quickfacts" aria-label="At a glance">
        <p class="atn-kicker">At a glance</p>
        <div class="atn-fact"><strong>BIOECOS Group Leader</strong><span>UFZ · Since September 2024</span></div>
        <div class="atn-fact"><strong>Individualised niches &amp; evidence synthesis</strong><span>Research interests</span></div>
        <div class="atn-fact"><strong>540 Google Scholar citations</strong><span>As of 29 August 2026</span></div>
      </aside>
    </div>

    <!-- ACADEMIC APPOINTMENTS -->
    <section class="atn-section" id="career">
      <div class="atn-heading"><span class="atn-n">01</span><h2>Academic appointments</h2></div>

      <div class="atn-card">
        <div class="atn-card-head"><h3>Research Group Leader · BIOECOS</h3><span class="atn-date">Sep 2024 – present</span></div>
        <p class="atn-org">Helmholtz Centre for Environmental Research – UFZ</p>
        <p class="atn-note"><a href="https://www.ufz.de/index.php?en=34212">Department of Computational Landscape Ecology</a> · <a href="https://www.ufz.de/index.php?en=37501">BIOECOS Group</a></p>
      </div>

      <div class="atn-card">
        <div class="atn-card-head"><h3>Postdoctoral Researcher</h3><span class="atn-date">Nov 2022 – Sep 2024</span></div>
        <p class="atn-org">Helmholtz Centre for Environmental Research – UFZ</p>
        <p class="atn-note">Department of Computational Landscape Ecology · Advisor: Dr Michael Beckmann</p>
      </div>
    </section>

    <!-- EDUCATION -->
    <section class="atn-section" id="education">
      <div class="atn-heading"><span class="atn-n">02</span><h2>Education</h2></div>

      <div class="atn-card">
        <div class="atn-card-head"><h3>PhD · Ecology</h3><span class="atn-date">2018 – 2022</span></div>
        <p class="atn-org">Friedrich Schiller University Jena · Germany</p>
        <p><em>“The behavioural ecology of individualized niches in the light of meta-analysis”</em> · Supervisor: Prof. Holger Schielzeth · <a href="https://www.researchgate.net/publication/361763446_PhD_Thesis_-_Scaling_down_the_ecological_niche_from_populations_to_individuals_an_evidence_synthesis_approach">Dissertation</a></p>
      </div>

      <div class="atn-card">
        <div class="atn-card-head"><h3>MSc · Forestry and Natural Environment</h3><span class="atn-date">2016 – 2018</span></div>
        <p class="atn-org">Aristotle University of Thessaloniki · Greece</p>
        <p><em>“Herpetofauna-habitat relationships in the suburban forest of Thessaloniki”</em> · Supervisor: Prof. Dimitrios Bakaloudis · <a href="https://ikee.lib.auth.gr/record/297309?ln=en">Thesis</a></p>
      </div>

      <div class="atn-card">
        <div class="atn-card-head"><h3>BSc · Forestry and Natural Environment</h3><span class="atn-date">2010 – 2016</span></div>
        <p class="atn-org">Aristotle University of Thessaloniki · Greece</p>
      </div>
    </section>

    <!-- HONOURS -->
    <section class="atn-section" id="honours">
      <div class="atn-heading"><span class="atn-n">03</span><h2>Honours &amp; awards</h2></div>
      <div class="atn-honour"><span class="atn-year">2021</span><div><strong>Poster Prize</strong><p>Annual Meeting of the German Ecological Society (GfÖ).</p></div></div>
      <div class="atn-honour"><span class="atn-year">2019</span><div><strong>Poster Prize</strong><p>Meeting of the German Zoological Society (DZG), Behavioural Biology Section.</p></div></div>
      <div class="atn-honour"><span class="atn-year">2017</span><div><strong>Travel Grant</strong><p>Technical University of Denmark and Aristotle University of Thessaloniki, for participation in the “Green Challenge” competition.</p></div></div>
      <div class="atn-honour"><span class="atn-year">2016</span><div><strong>Commendation of Excellence</strong><p>Aristotle University of Thessaloniki, for excellence in undergraduate studies.</p></div></div>
      <div class="atn-honour"><span class="atn-year">2010</span><div><strong>Award and Commendation of Excellence</strong><p>Aristotle University of Thessaloniki, for the highest grade in the entrance examinations for the School of Forestry and Natural Environment.</p></div></div>
    </section>

    <!-- INTERNATIONAL EXPERIENCE -->
    <section class="atn-section" id="international">
      <div class="atn-heading"><span class="atn-n">04</span><h2>International research experience</h2></div>
      <div class="atn-minicard">
        <div class="atn-card-head"><h3>Erasmus Placement · University of Glasgow</h3><span class="atn-date">Mar – Jun 2018</span></div>
        <p><a href="https://www.gla.ac.uk/research/az/boydorr/people/byorganisation/biodiversityanimalhealthandcomparativemedicine/">Institute of Biodiversity, Animal Health and Comparative Medicine</a>, Scotland · Advisor: Prof. Jason Matthiopoulos</p>
        <p>Project: Environmental niche modelling of the black grouse (<em>Lyrurus tetrix</em>).</p>
      </div>
    </section>

    <!-- TEACHING -->
    <section class="atn-section" id="teaching">
      <div class="atn-heading"><span class="atn-n">05</span><h2>Teaching experience</h2></div>

      <div class="atn-course">
        <div class="atn-card-head"><h3>Friedrich Schiller University Jena</h3><span class="atn-date">Apr – Jul 2020; Apr – Jul 2022</span></div>
        <p>Course Assistant · PI: Prof. Holger Schielzeth</p>
        <p class="atn-course-title">Einflussreiche Publikationen in der Ökologie / Classic Papers in Ecology (MEES021/E16)</p>
      </div>

      <div class="atn-course">
        <div class="atn-card-head"><h3>Friedrich Schiller University Jena</h3><span class="atn-date">Nov 2021 – Jan 2022; Nov 2022 – Jan 2023</span></div>
        <p>Course Assistant · PI: Prof. Stefan Halle</p>
        <p class="atn-course-title">Ecological Concepts 1: Current Fields of Ecological Research (E15)</p>
      </div>

      <div class="atn-course">
        <div class="atn-card-head"><h3>Max Planck Institute for Evolutionary Anthropology / Leipzig University</h3><span class="atn-date">29 Nov – 17 Dec 2021</span></div>
        <p>Practical Course Assistant · PI: Prof. Anja Widdig</p>
        <p class="atn-course-title">Module 11-BIO-0804: Primate Behavioral Ecology</p>
      </div>

      <div class="atn-course">
        <div class="atn-card-head"><h3>Friedrich Schiller University Jena</h3><span class="atn-date">Oct 2021; Oct 2022</span></div>
        <p>Course Assistant · PI: Prof. Holger Schielzeth · <a href="https://www.uni-jena.de/220913-lehrpreisschielzeth">Teaching award</a></p>
        <p class="atn-course-title">Praktikum Evolutionsbiologie (BB006)</p>
      </div>

      <div class="atn-course">
        <div class="atn-card-head"><h3>Friedrich Schiller University Jena · Graduate Academy</h3><span class="atn-date">23 Nov 2020</span></div>
        <p>Qualification Programme</p>
        <p class="atn-course-title">Meta-analysis course · <a href="https://qualifizierung.uni-jena.de/pages/coursedescription.jsf?courseId=34064190">Course information</a></p>
      </div>
    </section>

    <!-- PROFESSIONAL DEVELOPMENT -->
    <section class="atn-section" id="training">
      <div class="atn-heading"><span class="atn-n">06</span><h2>Professional development</h2></div>
      <ul class="atn-list">
        <li><strong>2024–2025</strong> · COMPASS Mentoring Programme.</li>
        <li><strong>December 2024</strong> · How to Teach in Higher Education – Teaching Skills for Scientists (Basics).</li>
        <li><strong>2023</strong> · Peer Coaching Group, “Success Strategies for Women in Academia”.</li>
        <li><strong>2023–2024</strong> · Creative Problem-Solving – A Brief Introduction to the Design Thinking Method.</li>
        <li><strong>2023–2024</strong> · Professional Recruitment (mandatory course for managers).</li>
        <li><strong>2019</strong> · Meta-analysis using R, led by Shinichi Nakagawa, Lund, Sweden.</li>
        <li><strong>2018</strong> · Meta-analysis workshop, led by Wolfgang Viechtbauer, Maastricht, the Netherlands.</li>
      </ul>
      <p class="atn-note">More than 20 additional seminars and workshops on technical and transferable skills; details available upon request.</p>
    </section>

    <!-- SCIENTIFIC SERVICE -->
    <section class="atn-section" id="service">
      <div class="atn-heading"><span class="atn-n">07</span><h2>Scientific service &amp; community</h2></div>
      <div class="atn-columns">
        <div>
          <h3 class="atn-subhead">Committees &amp; review</h3>
          <ul class="atn-list">
            <li>Member, IP1 Board / Steering Committee, Helmholtz Centre for Environmental Research – UFZ.</li>
            <li>Member, <a href="http://www.sortee.org/">SORTEE</a> Conference Committee (three years) and Advocacy Committee (two years).</li>
            <li>External expert reviewer, IPBES Second Global Assessment of Biodiversity and Ecosystem Services, First External Review (2026).</li>
            <li>Elected member, Council of PhD Representatives (Dr.FSU), Friedrich Schiller University Jena (2020–2021 and 2021–2022).</li>
            <li>Reviewer of Student Research Grant applications, Animal Behavior Society (2022).</li>
            <li>Peer reviewer for <em>Journal of Applied Ecology</em>, <em>Evolution</em> and <em>Journal of Animal Ecology</em>.</li>
          </ul>
        </div>
        <div>
          <h3 class="atn-subhead">Organisation &amp; affiliations</h3>
          <ul class="atn-list">
            <li>Organiser, Open CLE Forum, a fortnightly colloquium of UFZ’s Department of Computational Landscape Ecology (since 2023).</li>
            <li>Co-organiser of three SORTEE conferences (2021–2023).</li>
            <li>Organiser of synthesis workshops in Jena (June 2023) and Leipzig (August 2024).</li>
            <li>Member of BES, SORTEE, GfÖ, ESA and HELECOS.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- INVITED TALKS -->
    <section class="atn-section" id="talks">
      <div class="atn-heading"><span class="atn-n">08</span><h2>Invited talks</h2></div>
      <ul class="atn-list">
        <li><strong>“Hutchinson’s ecological niche for individuals”</strong> · N. Dingemanse’s Lab, Ludwig Maximilian University of Munich · 11 January 2022.</li>
        <li><strong>“NC³ – Individualized niches: theory and practice”</strong> · InChangE, NC³ and JICE Symposium, Bielefeld University · 5 April 2022.</li>
        <li>Multiple presentations at the regular seminar of the Animal Behaviour Group, Bielefeld University.</li>
      </ul>
    </section>

    <!-- PUBLICATIONS -->
    <section class="atn-section" id="publications">
      <div class="atn-heading"><span class="atn-n">09</span><h2>Publications &amp; research outputs</h2></div>
      <p class="atn-introline">Peer-reviewed articles, manuscripts, preprints, software and science communication. Titles link to the original publications or repositories where available.</p>

      <h3 class="atn-subhead">Peer-reviewed publications</h3>
      <ul class="atn-pubs">

        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://doi.org/10.3897/ibe.2.203247">The individualized niche in motion: Quantifying individual specialisation with movement data</a><p><strong>Takola, E.</strong> (2026). <em>Individual-Based Ecology</em>, 2, e203247.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://doi.org/10.1016/j.ecoinf.2026.103725">From LSA to LLM: Evolution and limitations of topic modelling methods for biodiversity conservation</a><p><strong>Takola, E.</strong> (2026). <em>Ecological Informatics</em>, 95, 103725.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://doi.org/10.24072/pcjournal.677">Global North–South science inequalities due to language and funding barriers</a><p>Turba, R., Thoré, E. S. J., Bertram, M. G., Bridg, H., Sabet, S. S., Gamboa, M., Ríos-Orjuela, J. C., <strong>Takola, E.</strong>, Capa Salinas, J., Sampaio Franco, A. C., &amp; Marín, C. (2026). <em>Peer Community Journal</em>, 6, e9.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://doi.org/10.1098/rspb.2024.1487">The promise of community-driven preprints in ecology and evolution</a><p>Noble, D. W., Xirocostas, Z. A., Wu, N. C., Martinig, A. R., Almeida, R. A., Bairos-Novak, K. R., … <strong>Takola, E.</strong>, … &amp; Lagisz, M. (2025). <em>Proceedings of the Royal Society</em>, 292(2039), 20241487.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://doi.org/10.1098/rspb.2024.1430">Priced out of belonging? Insufficient concessions on membership fees across international societies in ecology and evolution</a><p>Lagisz, M., Bairos-Novak, K. R., Martinig, A. R., Bertram, M., Mizuno, A., Sabet, S. S., … <strong>Takola, E.</strong>, … &amp; Nakagawa, S. (2025). <em>Proceedings of the Royal Society</em>, 292(2040), 20241430.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://doi.org/10.1098/rspb.2025.1394">From policy to practice: Progress towards data- and code-sharing in ecology and evolution</a><p>Ivimey-Cook, E. R., Sánchez-Tójar, A., Berberi, I., <strong>Takola, E.</strong>, … Moran, N. P. (2025). <em>Proceedings of the Royal Society B: Biological Sciences</em>, 292(2055), 20251394.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://doi.org/10.1186/s12915-024-02101-x">Same data, different analysts: variation in effect sizes due to analytical decisions in ecology and evolutionary biology</a><p>Gould, E., Fraser, H. S., Parker, T. H., Nakagawa, S., Griffith, S. C., Vesk, P. A., Fidler, F., … <strong>Takola, E.</strong>, … Zitomer, R. A. (2025). <em>BMC Biology</em>, 23, 35.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2023</span><div><a class="atn-pub-title" href="https://doi.org/10.1016/j.dib.2023.109696">An open-access global database of meta-analyses investigating yield and biodiversity responses to different management practices</a><p><strong>Takola, E.</strong>, Bonfanti, J., Seppelt, R., &amp; Beckmann, M. (2023). <em>Data in Brief</em>, 109696.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2022</span><div><a class="atn-pub-title" href="https://doi.org/10.1093/biosci/biac023">How individualized niches arise: Defining mechanisms of niche construction, niche choice and niche conformance</a><p>Trappes, R., Nematipour, B., Kaiser, M. I., Krohs, U., van Benthem, K. J., Ernst, U. R., Gadau, J., Korsten, P., Kurtz, J., Schielzeth, H., Schmoll, T., &amp; <strong>Takola, E.</strong> (2022). <em>BioScience</em>, biac023.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2022</span><div><a class="atn-pub-title" href="https://doi.org/10.1007/s10539-022-09849-y">Hutchinson’s ecological niche for individuals</a><p><strong>Takola, E.</strong>, &amp; Schielzeth, H. (2022). <em>Biology &amp; Philosophy</em>, 37(4), 25.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2021</span><div><a class="atn-pub-title" href="https://doi.org/10.1016/j.anbehav.2021.07.018">Novelty at second glance: a critical appraisal of the novel object paradigm based on meta-analysis</a><p><strong>Takola, E.</strong>, Krause, E., Müller, C., &amp; Schielzeth, H. (2021). <em>Animal Behaviour</em>, 180, 123–142.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2021</span><div><a class="atn-pub-title" href="https://doi.org/10.1111/oik.08201">Shifts between cooperation and antagonism driven by individual variation: a systematic synthesis review</a><p>Moran, N., Caspers, B., Chakarov, N., Ernst, U., Fricke, C., Kurtz, J., Lilie, N., … <strong>Takola, E.</strong>, … &amp; Wittmann, M. (2021). <em>Oikos</em>.</p></div></li>
      </ul>

      <h3 class="atn-subhead">Manuscripts &amp; preprints</h3>
      <ul class="atn-pubs">

        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://ecoevorxiv.org/repository/view/13681/">An individual-based model for white storks (<em>Ciconia ciconia</em>) in Germany during the breeding season</a><span class="atn-status">Submitted · Preprint</span><p>Ferdous, J., Peters, R., Berger, U., &amp; <strong>Takola, E.</strong> (2026). <em>EcoEvoRxiv</em>.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://doi.org/10.32942/X2D08C">Factors influencing the use of scientific evidence in conservation practice and policy: Insights from a systematic map</a><span class="atn-status">Preprint</span><p>Martin, P. A., Amirmohammedi, F., Barreto, C., Berger, I., <strong>Takola, E.</strong>, … Oliver, K. (2026). <em>EcoEvoRxiv</em>.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://ecoevorxiv.org/repository/view/9796/">Tracking the hidden niches: Movement-based insights into northern lapwing intraspecific variation and conservation</a><span class="atn-status">Submitted · Preprint</span><p>Esguerra, J., Grimm-Seyfarth, A., &amp; <strong>Takola, E.</strong> (2025). <em>EcoEvoRxiv</em>.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2024</span><div><span class="atn-pub-title">The effect of surrounding landscape on the effectiveness of yield treatments: a global data synthesis of field experiments</span><span class="atn-status">In preparation</span><p><strong>Takola, E.</strong>, Beckmann, M., Beillouin, D., Bishop, J., Burian, A., Jones, S., Spake, R., &amp; Uksa, M. (2024).</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2024</span><div><a class="atn-pub-title" href="https://ecoevorxiv.org/repository/view/8371/">A network meta-analysis of yield treatments</a><span class="atn-status">Submitted · Preprint</span><p>Anochirim, M., Stewart, G., Grainger, M., &amp; <strong>Takola, E.</strong> (2024). <em>EcoEvoRxiv</em>.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2024</span><div><a class="atn-pub-title" href="https://ecoevorxiv.org/repository/view/8378/">Does sustainable agriculture promote biodiversity and yield? A second-order meta-analysis</a><span class="atn-status">Submitted · Preprint</span><p><strong>Takola, E.</strong>, Beckmann, M., Bonfanti, J., Diel, J., Korrell, L., Reitz, T., &amp; Tamburini, G. (2024). <em>EcoEvoRxiv</em>.</p></div></li>
      </ul>

      <h3 class="atn-subhead">Software</h3>
      <ul class="atn-pubs">
        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://zenodo.org/records/14855698">decimatoR: an R package to convert heterogeneous coordinate formats into decimal degrees</a><p>Shcherbinina, E., Doktor, D., &amp; <strong>Takola, E.</strong> (2025). Version 1.0. <em>Zenodo</em>.</p></div></li>
      </ul>

      <h3 class="atn-subhead">Science communication &amp; open science</h3>
      <ul class="atn-pubs">
        <li class="atn-pub"><span class="atn-pub-year">2026</span><div><a class="atn-pub-title" href="https://doi.org/10.17605/OSF.IO/WX5KA">Schutz von Amphibien und Reptilien in Deutschland</a><p>Dittmann, J., &amp; <strong>Takola, E.</strong> (2026). Policy brief in German.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2025</span><div><a class="atn-pub-title" href="https://zenodo.org/records/16421733">Organising projects for reproducibility</a><p><strong>Takola, E.</strong> (2025). In N. Cooper &amp; P.-Y. Hsing (Eds.), <em>A Guide to Reproducible Code in Ecology and Evolution</em>. British Ecological Society.</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">2024</span><div><a class="atn-pub-title" href="https://www.sortee.org/blog/2024/04/12/2024_open_data_myths/">Debunking myths around open data</a><p><strong>Takola, E.</strong> (2024).</p></div></li>

        <li class="atn-pub"><span class="atn-pub-year">—</span><div><span class="atn-pub-title">Contribution to the Greek translation of the CRediT statement</span><p>Contribution to the Greek-language version of the contributor roles taxonomy.</p></div></li>
      </ul>
    </section>
  </div>

  <footer class="atn-footer">
    <span>© Eleni-Elda (Elina) Takola · Leipzig, Germany</span>
    <span><a href="https://orcid.org/0000-0003-1268-5513">ORCID: 0000-0003-1268-5513</a></span>
  </footer>
</div>
