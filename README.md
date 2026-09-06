<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8E2DE2,100:4A00E0&height=220&section=header&text=ADITYA%20SHELKE&fontSize=68&fontColor=ffffff&animation=fadeIn&fontAlignY=34&desc=AI%20%26%20Systems%20Engineer%20%C2%B7%20Rust%20%26%20Python%20%C2%B7%20Local-first%20software&descSize=17&descAlignY=53" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=23&duration=3200&pause=900&color=8E2DE2&center=true&vCenter=true&width=780&lines=Building+OpenVoice+%E2%80%94+local-first+dictation+for+Windows;9+Rust+crates+%C2%B7+243+tests+%C2%B7+zero+network+calls;Technical+Support+Engineer+Intern+%40+Karix+Mobile;I+turn+support+tickets+into+shipped+products" alt="Building OpenVoice — local-first dictation for Windows. 9 Rust crates, 243 tests, zero network calls. Technical Support Engineer Intern at Karix Mobile. I turn support tickets into shipped products." />

<br/>

<a href="https://aditya-shelke-portfolio.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-8E2DE2?style=for-the-badge&logo=vercel&logoColor=white&labelColor=000000" alt="Portfolio"/></a>
&nbsp;
<a href="https://linkedin.com/in/adityashelke04"><img src="https://img.shields.io/badge/LINKEDIN-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=000000" alt="LinkedIn"/></a>
&nbsp;
<a href="mailto:adityashelke04@gmail.com"><img src="https://img.shields.io/badge/EMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=000000" alt="Email"/></a>
&nbsp;
<a href="https://youtube.com/@adityashelke06"><img src="https://img.shields.io/badge/YOUTUBE-FF0000?style=for-the-badge&logo=youtube&logoColor=white&labelColor=000000" alt="YouTube"/></a>

</div>

---

## 👨‍💻 Who I Am

```typescript
const aditya = {
    role:        "Technical Support Engineer Intern @ Karix Mobile",
    shipping:    "OpenVoice — local-first dictation for Windows",
    dayJob:      ["Meta webhook logs", "SMPP error codes",
                  "DLT registration", "delivery-report SQL"],
    writesIn:    ["Rust", "Python", "TypeScript"],
    education:   "Final Year — Information Science & Engineering",
    location:    "Bengaluru, India 🇮🇳",
    lookingFor:  "AI / Systems Engineering roles",
    philosophy:  "If users keep hitting the same wall, build the ladder",
};
```

I spend my days on the support desk of a CPaaS platform, watching the same failures
arrive over and over. Most of what I build starts there — a problem I had to solve by
hand enough times that automating it stopped being optional.

---

## 🎙️ OpenVoice &nbsp;·&nbsp; <sub>flagship</sub>

> **The one I want you to look at.** Local-first push-to-talk dictation for Windows.
> Hold a key, speak, release — correctly formatted text appears at your cursor, in any
> app. No cloud, no account, no telemetry.

<div align="center">

<a href="https://openvoice-dictation.vercel.app">
<img src="https://raw.githubusercontent.com/adityashelke04/OpenVoice/main/docs/images/hub-home.png" width="88%" alt="OpenVoice home screen showing words dictated, speaking speed charted against a typing baseline, time saved, a daily streak, and recent dictations"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/v0.8.0-alpha-FF9F0A?style=for-the-badge&labelColor=000000" alt="v0.8.0 alpha"/>
<img src="https://img.shields.io/badge/RUST%20TESTS-243-44D62C?style=for-the-badge&logo=rust&logoColor=white&labelColor=000000" alt="243 Rust tests"/>
<img src="https://img.shields.io/badge/DECODE-~500ms-8E2DE2?style=for-the-badge&labelColor=000000" alt="Median decode about 500 milliseconds"/>
<img src="https://img.shields.io/badge/IDLE%20RAM-~60MB-8E2DE2?style=for-the-badge&labelColor=000000" alt="About 60 megabytes idle RAM"/>
<img src="https://img.shields.io/badge/NETWORK%20CALLS-0-44D62C?style=for-the-badge&labelColor=000000" alt="Zero network calls"/>

</div>

**Whisper transcribes beautifully and formats nothing.** Ask it to transcribe someone
writing code and you get `use effect` for `useEffect`, `cube control` for `kubectl`, and
the literal words "open parenthesis". Those aren't model bugs — they're accurate
transcriptions of what you actually said. Fixing them is a text-processing problem, and
text processing is deterministic, testable, and improvable one rule at a time.

So OpenVoice treats the speech model as a swappable commodity and puts all its effort
into what happens next:

```
you say:   "um so we need to call use effect here comma then return null"
you get:   "So we need to call useEffect here, then return null"

you say:   "cube control get pods"          (a terminal has focus)
you get:   "kubectl get pods"               — no capital, no period. it runs.
```

Both are asserted as tests in the formatter crate, not illustrations. It knows which app
has focus and applies the rules that app deserves. The no-network claim is enforced in
CI by an allow-list check, not just promised in a README.

<div align="center">

**[⬇ Download for Windows](https://github.com/adityashelke04/OpenVoice/releases/download/download/OpenVoice-x64-setup.exe)** &nbsp;·&nbsp;
**[Website](https://openvoice-dictation.vercel.app)** &nbsp;·&nbsp;
**[Docs](https://openvoice-dictation.vercel.app/docs)** &nbsp;·&nbsp;
**[Source](https://github.com/adityashelke04/OpenVoice)**

<sub>Alpha, and honest about it: nothing is code-signed yet, so Windows will warn you
about an unknown publisher, and the bundled speech engine is CPU-only.</sub>

</div>

---

## 🧪 The Lab

<sub>Everything else I'm building, ordered by what I'd point a stranger at first.</sub>

<table>
<tr>
<td width="50%" valign="top">

### 🩺 WhatsApp Error → Client Reply
`INTERNAL · APPROVED`

Paste a Meta delivery-failure code, get the root cause, a resolution runbook, and a
client-ready email — in about thirty seconds instead of twenty minutes. 62 curated codes,
role-based access, a full audit trail, and a template fallback so it still works when the
model doesn't.

`FastAPI` `Gemini` `SQLite` `JWT`

</td>
<td width="50%" valign="top">

### 🛡️ Kavach
`HACKATHON BUILD`

Installable web app that tells you whether a message you just received is a scam —
running the model **on your own phone**, offline, with nothing sent anywhere unless you
ask for it. Built for the iQOO Hackathon 2026.

[`Repo →`](https://github.com/adityashelke04/Kavach-iqoo_hackathon) &nbsp; `React 19` `WebLLM` `PWA`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📊 XSlicer
`SHIPPED`

Splits oversized spreadsheets into attachment-sized parts entirely inside the browser
tab — no upload, no server, zero network calls enforced by CSP. Boring problem,
satisfying fix.

`JavaScript` `Web Workers` `fflate`

</td>
<td width="50%" valign="top">

### 🚀 Launchpad
`IN DEVELOPMENT`

Job-hunt command center — track applications, parse listings, and stay sane during the
grind.

`Vercel` `Supabase` `Gemini`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🌍 PrivLens
`IN DEVELOPMENT`

Global privacy enforcement tracker — GDPR fines, rulings, and regulatory decisions
gathered into one lens.

`Web` `Data`

</td>
<td width="50%" valign="top">

### 💼 Infinity Coins
`IN DEVELOPMENT`

Insurance advisory platform — policy discovery, comparison, and advisor workflows in one
place.

`Web`

</td>
</tr>
</table>

---

## 🛠️ Arsenal

<div align="center">

<img src="https://skillicons.dev/icons?i=rust,python,ts,js,java,cpp,tauri,fastapi,react,nextjs,tailwind,pytorch,sklearn,sqlite,mysql,aws,gcp,vercel,supabase,postman,git,github,vscode&perline=8" alt="Rust, Python, TypeScript, JavaScript, Java, C++, Tauri, FastAPI, React, Next.js, Tailwind, PyTorch, scikit-learn, SQLite, MySQL, AWS, GCP, Vercel, Supabase, Postman, Git, GitHub, VS Code"/>

<br/><br/>

<img src="https://img.shields.io/badge/Gemini%20API-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white&labelColor=000000" alt="Gemini API"/>
<img src="https://img.shields.io/badge/WhatsApp%20Business%20API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white&labelColor=000000" alt="WhatsApp Business API"/>
<img src="https://img.shields.io/badge/On--Device%20Inference-FF6B6B?style=for-the-badge&logo=openai&logoColor=white&labelColor=000000" alt="On-device inference"/>
<img src="https://img.shields.io/badge/Whisper%20%2F%20ASR-4A00E0?style=for-the-badge&logo=openai&logoColor=white&labelColor=000000" alt="Whisper and ASR"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white&labelColor=000000" alt="Pandas"/>

</div>

---

## 📈 Stats

<div align="center">

<img src="https://github-readme-stats-sigma-five.vercel.app/api?username=adityashelke04&show_icons=true&theme=radical&hide_border=true&bg_color=0d1117&title_color=8E2DE2&icon_color=4A00E0&include_all_commits=true&count_private=true" width="49%" alt="GitHub stats"/>
<img src="https://streak-stats.demolab.com/?user=adityashelke04&theme=radical&hide_border=true&background=0d1117&ring=8E2DE2&fire=4A00E0&currStreakLabel=8E2DE2" width="49%" alt="GitHub streak"/>

<br/>

<img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=adityashelke04&theme=radical&hide_border=true&bg_color=0d1117&title_color=8E2DE2&layout=compact&langs_count=8" width="42%" alt="Most used languages"/>

<br/><br/>

<img src="https://github.com/Platane/snk/raw/output/github-contribution-grid-snake-dark.svg" width="95%" alt="Contribution graph being eaten by a snake"/>

</div>

---

## 🎮 Beyond The Terminal

<div align="center">

**4000+ hours** in competitive FPS — shot-calling, reading a fight, and losing enough
to learn something

Reading about local-first software, ASR pipelines, and how to make slow things fast

*If users keep hitting the same wall, build the ladder*

</div>

<br/>

<div align="center">

<img src="https://komarev.com/ghpvc/?username=adityashelke04&color=8E2DE2&style=for-the-badge&label=PROFILE+VISITS" alt="Profile visit counter"/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4A00E0,100:8E2DE2&height=120&section=footer" width="100%"/>

</div>
