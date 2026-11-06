---
layout: single
title: "Human Evaluation"
permalink: /humaneval/
author_profile: false
---

<style>
.lang-switcher { margin-bottom: 1.5em; }
.lang-btn {
  cursor: pointer;
  padding: 0.4em 0.9em;
  margin-right: 0.5em;
  border: 1px solid #ccc;
  border-radius: 4px;
  background: #f5f5f5;
  font-size: 0.95em;
}
.lang-btn.active { background: #333; color: #fff; border-color: #333; }

.he-phases { display: flex; flex-wrap: wrap; gap: 0.4em; margin: 0.8em 0 1em; }
.he-phase {
  color: #fff; padding: 0.35em 0.8em; border-radius: 999px; border: 2px solid transparent;
  font-size: 0.85em; white-space: nowrap; cursor: pointer; font-family: inherit;
}
.he-phase:hover { filter: brightness(1.08); }
.he-phase[aria-expanded="true"] { border-color: #333; }
.he-p1 { background: #667eea; }
.he-p2 { background: #48bb78; }
.he-p3 { background: #f6ad55; }
.he-p4 { background: #ed64a6; }
.he-p5 { background: #9f7aea; }
.he-phase-block { margin: 0.8em 0 1em; }
.he-phase-block .he-phases { margin-bottom: 0; }
.page__content .he-footnote { font-size: 0.75em; line-height: 1.4; color: #777; margin: 0.3em 0 1em; }
.page__content .he-hint { font-size: 0.75em; font-style: italic; color: #777; margin: 0.5em 0 0; }
.he-panel { margin: 0.7em 0 0; padding: 0.6em 1em; border-left: 4px solid #ccc; background: #fafafa; border-radius: 0 6px 6px 0; }
.he-panel[hidden] { display: none; }
.he-panel p { margin: 0 0 0.4em; }
.he-panel p:last-child { margin-bottom: 0; }
.he-panel ul { margin: 0 0 0.4em; padding-left: 1.2em; }
.he-panel li { margin-bottom: 0.2em; }
.he-panel-p1 { border-left-color: #667eea; }
.he-panel-p2 { border-left-color: #48bb78; }
.he-panel-p3 { border-left-color: #f6ad55; }
.he-panel-p4 { border-left-color: #ed64a6; }
.he-panel-p5 { border-left-color: #9f7aea; }
.he-toc { font-size: 0.9em; margin-bottom: 1.5em; }
.he-toc a { margin-right: 1em; white-space: nowrap; }

/* Page width: full-width guide, no sidebar */
#main .page { float: none; width: 100%; margin: 0; padding: 0; }

/* Screenshots */
.page__content figure.he-fig { display: block; margin: 0; min-width: 0; }
.page__content .he-fig img { display: block; width: 100%; height: auto; margin: 0; border: 1px solid #e3e6ea; border-radius: 8px; box-shadow: 0 1px 4px rgba(0, 0, 0, 0.06); }
.page__content .he-fig figcaption { display: block; margin: 0.55em 0 0; padding: 0; font-family: inherit; font-size: 0.75em; line-height: 1.4; color: #666; }
.page__content > .lang-content > .he-fig { margin: 1.4em 0 0.5em; }
.he-row { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1.25em; margin: 1.2em 0 1.6em; }
.page__content .he-row .he-fig img { aspect-ratio: 1.38; object-fit: cover; }
.he-split { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 2em; align-items: start; margin: 1.2em 0 1.6em; }
.he-split-slimfig { grid-template-columns: minmax(0, 2.4fr) minmax(0, 1fr); }
.he-split-widefig { grid-template-columns: minmax(0, 1fr) minmax(0, 1.75fr); }
.he-split-midfig { grid-template-columns: minmax(0, 1.4fr) minmax(0, 1fr); }
.he-split-commentfig { grid-template-columns: minmax(0, 1.75fr) minmax(0, 1fr); }
.he-split > div > :first-child { margin-top: 0; }
.he-split > div > :last-child { margin-bottom: 0; }
.page__content .he-split > div > .he-fig { margin-top: 1em; max-width: 600px; }
.he-persona { display: flex; gap: 0.75em; align-items: stretch; }
.he-persona > img { flex: 1.1 1 0; min-width: 0; }
.he-persona-stack { flex: 1 1 0; min-width: 0; display: flex; flex-direction: column; justify-content: space-between; gap: 0.75em; }
.page__content img.he-crop-top { aspect-ratio: 1232 / 1402; object-fit: cover; object-position: bottom; }
.page__content img.he-crop-bottom { aspect-ratio: 1152 / 1290; object-fit: cover; object-position: top; }
.he-badged { position: relative; }
.he-badge {
  position: absolute; transform: translate(-50%, -50%); display: flex; align-items: center; justify-content: center;
  width: 1.7em; height: 1.7em; border-radius: 50%; background: #333; color: #fff; font-size: 0.75em; font-weight: 700;
  box-shadow: 0 0 0 2px #fff;
}
@media (max-width: 760px) {
  .he-row, .he-split, .he-split-slimfig, .he-split-widefig, .he-split-midfig, .he-split-commentfig { grid-template-columns: minmax(0, 1fr); }
}
</style>

<div class="lang-switcher">
  <button id="btn-en" class="lang-btn active" onclick="setLang('en')">🇬🇧 English</button>
  <button id="btn-fr" class="lang-btn" onclick="setLang('fr')">🇫🇷 Français</button>
</div>

<div id="content-en" class="lang-content" markdown="1">

Chatbots can be told how to talk: in simple or sophisticated English, in an upbeat or a critical tone, calmly or with some emotion. What we don't really know is whether they do it. This study looks at exactly that. You chat with a recruiter agent in a mock job interview, and each time it answers, you tell us which of two possible replies better shows the style the agent was asked to have.

You send 12 messages in total. You are not being tested here, the agent is, so there are no right or wrong answers. Everything is anonymous and voluntary, and you can stop at any time by closing the page.

<div class="he-toc">
<a href="#he-before">Before you start</a>
<a href="#he-steps">How a turn works</a>
<a href="#he-criteria">What to look for</a>
<a href="#he-stuck">If you're stuck</a>
<a href="#he-flag">Flagging a problem</a>
<a href="#he-know">Good to know</a>
<a href="#he-contact">Take part</a>
<a href="#he-about">About the research</a>
</div>

<figure class="he-fig">
<img src="/images/he-ensemble.png" alt="The experiment screen, with the chat on the left and the progress and memo panel on the right" width="3248" height="1548" loading="lazy">
<figcaption>The screen during a turn. On the left, the chat, with the current phase on top and the two replies to compare. On the right, your progress and a memo you can check at any time.</figcaption>
</figure>

## Before you start {#he-before}

<div class="he-split he-split-slimfig" markdown="1">
<div markdown="1">

Read the information screen. A short "About you" form comes next (age range, English level, interview experience...). You can skip it, and the agent never sees your answers. Then tick the consent box, click **Start the interview** and give the page a moment to prepare the interview.

Only one person can take part at a time. If the page tells you someone else is already on it, come back in a few minutes.

</div>
<figure class="he-fig">
<img src="/images/he-questionnaire.png" alt="The optional About you form, followed by the consent box and the Start the interview button" width="1232" height="1534" loading="lazy" class="he-crop-top">
<figcaption>Fill in only what you wish, tick the consent box, then click <strong>Start the interview</strong>.</figcaption>
</figure>
</div>

## How a turn works {#he-steps}

<div class="he-split" markdown="1">
<div markdown="1">

1. Write your message and send it. Answer the way you would in a real interview, in a few sentences.
2. Wait for the agent, which can take anywhere from a few seconds to a few minutes. If you reload the page, your conversation is kept.
3. Above the two replies, a sentence tells you which style they should have, for example *"The agent response is expected to be Positive, Non loaded, B1."*
4. Read both replies. Which one is on the left or the right is random.
5. Click the one that shows this style more clearly, then click **Confirm choice**. The conversation goes on with the reply you picked.

</div>
<figure class="he-fig">
<div class="he-badged">
<img src="/images/he-choice.png" alt="A turn: the requested style above two replies, with the Confirm choice button below" width="2126" height="1544" loading="lazy">
<span class="he-badge" style="left:13.5%;top:29.6%">3</span>
<span class="he-badge" style="left:52.3%;top:50.3%">4</span>
<span class="he-badge" style="left:34%;top:73.3%">5</span>
</div>
<figcaption>Steps 3 to 5 on screen: the requested style, the two replies, and the button to confirm.</figcaption>
</figure>
</div>

The agent leads the interview through five phases, and the current one is always displayed at the top of the chat. You don't need to follow them, just answer naturally.

<div class="he-row">
<figure class="he-fig">
<img src="/images/he-phase-change.png" alt="Chat in phase 2, in green, while the message is being processed" width="2120" height="1556" loading="lazy">
<figcaption>Phase 2: the banner names the current phase and the colours follow it. Here, your message is being processed (step 2).</figcaption>
</figure>
<figure class="he-fig">
<img src="/images/he-fairly-technical.png" alt="Chat in phase 3, in orange" width="2122" height="1546" loading="lazy">
<figcaption>Later, in phase 3: the banner and the colours have changed. There is nothing for you to do.</figcaption>
</figure>
</div>

<div class="he-phase-block">
<div class="he-phases">
<button type="button" class="he-phase he-p1" aria-expanded="false" aria-controls="he-en-ph1">1 Greetings</button>
<button type="button" class="he-phase he-p2" aria-expanded="false" aria-controls="he-en-ph2">2 Background</button>
<button type="button" class="he-phase he-p3" aria-expanded="false" aria-controls="he-en-ph3">3 Technical point</button>
<button type="button" class="he-phase he-p4" aria-expanded="false" aria-controls="he-en-ph4">4 Short debate</button>
<button type="button" class="he-phase he-p5" aria-expanded="false" aria-controls="he-en-ph5">5 Send-off</button>
</div>
<p class="he-hint">Click a phase for more details.</p>
<div class="he-panel he-panel-p1" id="he-en-ph1" hidden>
<p>The agent welcomes you and makes some small talk to put you at ease. Answer as you would at the start of a real interview.</p>
<p>Typical messages:</p>
<ul>
<li><em>"Hi, thanks for having me!"</em></li>
<li><em>"I'm doing well, a bit nervous but happy to be here."</em></li>
<li><em>"Am I at the right place for the interview?"</em></li>
</ul>
</div>
<div class="he-panel he-panel-p2" id="he-en-ph2" hidden>
<p>The agent asks about your studies and your professional experience. You can talk about real or made-up ones.</p>
<p>Typical message: <em>"I did a master's in marketing, then I spent two years in a small agency running social media campaigns."</em></p>
</div>
<div class="he-panel he-panel-p3" id="he-en-ph3" hidden>
<p>The agent asks a question about your skills and how you would handle a work situation. A few sentences are enough.</p>
<p>Typical messages:</p>
<ul>
<li><em>"I usually start by listing priorities with the team, then I plan the work week by week and check progress regularly."</em></li>
<li><em>"In my last project, I trained a classifier on imbalanced data and used cross-validation to avoid overfitting."</em></li>
</ul>
</div>
<div class="he-panel he-panel-p4" id="he-en-ph4" hidden>
<p>The agent defends a point of view and you are free to agree, disagree or nuance. It doesn't matter whether what you say matches what you actually think.</p>
<p>Typical message: <em>"I see your point, but I think working in the office helps newcomers learn faster."</em></p>
</div>
<div class="he-panel he-panel-p5" id="he-en-ph5" hidden>
<p>The agent sums up the interview and wraps up the conversation. A polite closing message is all it takes.</p>
<p>Typical message: <em>"Thank you for your time, I enjoyed our discussion and I hope to hear from you soon."</em></p>
</div>
</div>

## What to look for {#he-criteria}

Each turn asks for one to three of the characteristics below, and you only judge the ones displayed. The question to keep in mind is which reply shows the requested style more clearly, whatever you would personally prefer. A friendly, well-written reply can still miss the target.

| Characteristic | Possible values | Description |
|---|---|---|
| Language level | A1, A2, B1, B2, C1, C2 | How sophisticated the English is, from basic (A1) to proficient (C2).<sup><a href="#he-cefr-en">1</a></sup><br>A1: familiar everyday expressions and very basic phrases.<br>A2: simple sentences about everyday topics such as family, shopping or work.<br>B1: clear standard language on familiar matters, able to describe experiences and give brief reasons and opinions.<br>B2: clear, detailed text on a wide range of subjects, including abstract and technical ones, with viewpoints explained.<br>C1: fluent, flexible and well-structured language on complex subjects, with implicit meaning.<br>C2: virtually everything expressed with ease, very fluently and precisely, with fine shades of meaning. |
| Polarity | Positive, Negative, Neutral | The overall sentiment of the text, as in sentiment analysis: does the message sound positive, negative, or neither? |
| Emotional load | Loaded, Non loaded | Whether the text shows noticeable emotion (Loaded) or none (Non loaded). |

<p class="he-footnote" id="he-cefr-en"><sup>1</sup> Level descriptions summarised from the <a href="https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions">Common European Framework of Reference for Languages (CEFR)</a>, Council of Europe.</p>

*Neutral* and *Non loaded* describe the absence of sentiment or emotion, so the flatter, more factual reply is the one to pick.

## If you're stuck {#he-stuck}

### During the conversation

**Hard to get started?** In this experiment, you are the one who opens the conversation. If needed, click **Need help to get started?** to get a few opening lines. Select the one you like, edit it if you wish and send the message. Using one of the suggested lines has no influence on how the experiment goes.

<div class="he-row">
<figure class="he-fig">
<img src="/images/he-starters1.png" alt="Empty chat with the Need help to get started? link" width="2134" height="1570" loading="lazy">
<figcaption>When the chat opens, click <strong>Need help to get started?</strong>, just under the instructions.</figcaption>
</figure>
<figure class="he-fig">
<img src="/images/he-starters2.png" alt="List of six suggested opening lines" width="2136" height="1546" loading="lazy">
<figcaption>Click a line: it goes into the message box, and you can edit it before sending.</figcaption>
</figure>
</div>

<div class="he-split he-split-widefig" markdown="1">
<div markdown="1">

**Out of inspiration?** If you don't know what to write during the conversation, the right panel has a **Pick a persona** button that gives you a random character to play, with a desired job and a study and work background. If you don't like the persona you got, click the same button again to get another one. You are free to follow the mentioned characteristics or not, this option is only there in case you need inspiration. It has no influence on how the experiment goes.

</div>
<figure class="he-fig">
<div class="he-persona">
<img src="/images/he-persona-click.png" alt="The right panel with the Pick a persona button" width="1126" height="1554" loading="lazy">
<div class="he-persona-stack">
<img src="/images/he-persona1.png" alt="A persona card for Fatou, applying as an accountant" width="838" height="658" loading="lazy">
<img src="/images/he-persona2.png" alt="A persona card for Paul, applying as a communication officer" width="816" height="558" loading="lazy">
</div>
</div>
<figcaption>On the left, the right panel with the <strong>Pick a persona</strong> button. On the right, two personas you might get: the button then becomes <strong>Pick another persona</strong>.</figcaption>
</figure>
</div>

### When evaluating

<div class="he-split" markdown="1">
<div markdown="1">

If you can't tell the two replies apart with regard to the mentioned characteristics, tick **I can't decide** and confirm. One of the replies will then be picked at random so the conversation can continue. If the two replies are exactly identical, the system detects it automatically and you have nothing to choose. Just answer the agent to carry on with the conversation.

</div>
<figure class="he-fig">
<img src="/images/he-cant-decide.png" alt="A note above the agent's message saying that a reply was picked at random" width="1586" height="626" loading="lazy">
<figcaption>After <strong>I can't decide</strong>, a note above the message tells you that the reply was picked at random.</figcaption>
</figure>
</div>

## Flagging a problem {#he-flag}

<div class="he-split he-split-midfig" markdown="1">
<div markdown="1">

If the last message from the agent looks off, click **Flag Inconsistency** in the right panel. It doesn't interrupt the interview. You can say that the agent is stuck in the previous phase or jumped to a phase that doesn't fit (phase-level), that it forgot or contradicted something said earlier (context-level), that the text makes no sense, or describe something else in a few words.

<figure class="he-fig">
<img src="/images/he-flag-inconsistency.png" alt="The Flag Inconsistency button and the list of common inconsistencies" width="1052" height="698" loading="lazy">
<figcaption>The button is in the right panel, along with a reminder of the most common problems.</figcaption>
</figure>

</div>
<figure class="he-fig">
<img src="/images/he-report-inconsistency.png" alt="The form to report an inconsistency, with four types to choose from" width="1152" height="1714" loading="lazy" class="he-crop-bottom">
<figcaption>The form that opens: pick a type, or <strong>Other</strong> to describe the problem in your own words.</figcaption>
</figure>
</div>

## Good to know {#he-know}

Please don't write personal data such as your name, address or employer. Invent details if you want to.

The agent builds two replies for every message, so waiting is normal. Try not to leave the page idle for too long: after 30 minutes without any action, the conversation is closed.

<div class="he-split he-split-commentfig" markdown="1">
<div markdown="1">

After the 12th choice, you can leave a comment if you wish, and then close the page. We record your messages, your choices, how long you take, the problems you flag, your comment and the optional "About you" answers. We don't ask for any name or email address. What the comparison is about is explained at the end of the experiment, so that it doesn't influence your choices.

</div>
<figure class="he-fig">
<img src="/images/he-leave-comment.png" alt="The end-of-interview window with an optional feedback field" width="1894" height="1312" loading="lazy">
<figcaption>The last screen: the comment is optional.</figcaption>
</figure>
</div>

## Take part {#he-contact}

If you'd like to take part, or if you have a question, [get in touch](mailto:barbara.gendron@loria.fr).

## About the research {#he-about}

This study is part of my PhD at LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, supervised by Mathieu d'Aquin (LORIA, CNRS) and Gaël Guibon (LIPN, Université Sorbonne Paris Nord). The thesis explores how to guide a language model with a conversation strategy built from formal concepts and rules, so that its behaviour becomes more predictable and better suited to its use case. The job interview is the prototype setting for that work.

</div>

<div id="content-fr" class="lang-content" markdown="1" style="display:none;">

On peut demander à un chatbot de parler d'une certaine manière : dans un anglais simple ou soutenu, sur un ton enthousiaste ou critique, calmement ou avec de l'émotion. Ce qu'on sait moins, c'est s'il le fait vraiment. C'est ce que cette étude cherche à savoir. Vous discutez avec un agent recruteur lors d'un faux entretien d'embauche, et à chaque réponse, vous nous dites laquelle de deux réponses possibles montre le mieux le style que l'agent devait avoir.

Vous envoyez 12 messages au total. Ce n'est pas vous qui êtes évalué mais l'agent, donc il n'y a ni bonne ni mauvaise réponse. Tout est anonyme et volontaire, et vous pouvez arrêter à tout moment en fermant la page.

<div class="he-toc">
<a href="#he-before-fr">Avant de commencer</a>
<a href="#he-steps-fr">Déroulé d'un tour</a>
<a href="#he-criteria-fr">Quoi observer</a>
<a href="#he-stuck-fr">En cas de blocage</a>
<a href="#he-flag-fr">Signaler un problème</a>
<a href="#he-know-fr">À savoir</a>
<a href="#he-contact-fr">Participer</a>
<a href="#he-about-fr">À propos de la recherche</a>
</div>

<figure class="he-fig">
<img src="/images/he-ensemble.png" alt="L'écran de l'expérience, avec le chat à gauche et le panneau de progression et de mémo à droite" width="3248" height="1548" loading="lazy">
<figcaption>L'écran pendant un tour. À gauche, le chat, avec la phase en cours en haut et les deux réponses à comparer. À droite, votre progression et un mémo à consulter à tout moment.</figcaption>
</figure>

## Avant de commencer {#he-before-fr}

<div class="he-split he-split-slimfig" markdown="1">
<div markdown="1">

Lisez l'écran d'information. Un court formulaire « About you » suit (tranche d'âge, niveau d'anglais, expérience des entretiens...). Vous pouvez le passer, et l'agent ne voit jamais vos réponses. Cochez ensuite la case de consentement, cliquez sur **Start the interview** et laissez à la page un instant pour préparer l'entretien.

Une seule personne à la fois peut participer. Si la page indique que quelqu'un d'autre est en cours d'expérience, revenez dans quelques minutes.

</div>
<figure class="he-fig">
<img src="/images/he-questionnaire.png" alt="Le formulaire facultatif About you, suivi de la case de consentement et du bouton Start the interview" width="1232" height="1534" loading="lazy" class="he-crop-top">
<figcaption>Remplissez uniquement ce que vous souhaitez, cochez la case de consentement, puis cliquez sur <strong>Start the interview</strong>.</figcaption>
</figure>
</div>

## Déroulé d'un tour {#he-steps-fr}

<div class="he-split" markdown="1">
<div markdown="1">

1. Écrivez votre message et envoyez-le. Répondez comme dans un vrai entretien, en quelques phrases.
2. Patientez le temps que l'agent réponde, de quelques secondes à quelques minutes. Si vous rechargez la page, votre conversation est conservée.
3. Au-dessus des deux réponses, une phrase indique le style qu'elles doivent avoir, par exemple *« The agent response is expected to be Positive, Non loaded, B1. »*
4. Lisez les deux réponses. Leur position à gauche ou à droite est aléatoire.
5. Cliquez sur celle qui montre ce style le plus clairement, puis sur **Confirm choice**. La conversation continue avec la réponse choisie.

</div>
<figure class="he-fig">
<div class="he-badged">
<img src="/images/he-choice.png" alt="Un tour : le style demandé au-dessus de deux réponses, avec le bouton Confirm choice en dessous" width="2126" height="1544" loading="lazy">
<span class="he-badge" style="left:13.5%;top:29.6%">3</span>
<span class="he-badge" style="left:52.3%;top:50.3%">4</span>
<span class="he-badge" style="left:34%;top:73.3%">5</span>
</div>
<figcaption>Les étapes 3 à 5 à l'écran : le style demandé, les deux réponses et le bouton pour confirmer.</figcaption>
</figure>
</div>

L'agent mène l'entretien en cinq phases, et la phase en cours est toujours affichée en haut du chat. Inutile de les suivre, répondez naturellement.

<div class="he-row">
<figure class="he-fig">
<img src="/images/he-phase-change.png" alt="Le chat en phase 2, en vert, pendant le traitement du message" width="2120" height="1556" loading="lazy">
<figcaption>Phase 2 : le bandeau indique la phase en cours et les couleurs suivent. Ici, votre message est en cours de traitement (étape 2).</figcaption>
</figure>
<figure class="he-fig">
<img src="/images/he-fairly-technical.png" alt="Le chat en phase 3, en orange" width="2122" height="1546" loading="lazy">
<figcaption>Plus tard, en phase 3 : le bandeau et les couleurs ont changé. Vous n'avez rien à faire.</figcaption>
</figure>
</div>

<div class="he-phase-block">
<div class="he-phases">
<button type="button" class="he-phase he-p1" aria-expanded="false" aria-controls="he-fr-ph1">1 Accueil</button>
<button type="button" class="he-phase he-p2" aria-expanded="false" aria-controls="he-fr-ph2">2 Parcours</button>
<button type="button" class="he-phase he-p3" aria-expanded="false" aria-controls="he-fr-ph3">3 Point technique</button>
<button type="button" class="he-phase he-p4" aria-expanded="false" aria-controls="he-fr-ph4">4 Court débat</button>
<button type="button" class="he-phase he-p5" aria-expanded="false" aria-controls="he-fr-ph5">5 Conclusion</button>
</div>
<p class="he-hint">Cliquez sur une phase pour plus de détails.</p>
<div class="he-panel he-panel-p1" id="he-fr-ph1" hidden>
<p>L'agent vous accueille et fait un peu de conversation pour vous mettre à l'aise. Répondez comme au début d'un vrai entretien.</p>
<p>Messages typiques (à écrire en anglais) :</p>
<ul>
<li><em>"Hi, thanks for having me!"</em></li>
<li><em>"I'm doing well, a bit nervous but happy to be here."</em></li>
<li><em>"Am I at the right place for the interview?"</em></li>
</ul>
</div>
<div class="he-panel he-panel-p2" id="he-fr-ph2" hidden>
<p>L'agent vous interroge sur vos études et votre expérience professionnelle. Vous pouvez parler de parcours réels ou inventés.</p>
<p>Message typique (en anglais) : <em>"I did a master's in marketing, then I spent two years in a small agency running social media campaigns."</em></p>
</div>
<div class="he-panel he-panel-p3" id="he-fr-ph3" hidden>
<p>L'agent pose une question sur vos compétences et sur la façon dont vous géreriez une situation de travail. Quelques phrases suffisent.</p>
<p>Messages typiques (à écrire en anglais) :</p>
<ul>
<li><em>"I usually start by listing priorities with the team, then I plan the work week by week and check progress regularly."</em></li>
<li><em>"In my last project, I trained a classifier on imbalanced data and used cross-validation to avoid overfitting."</em></li>
</ul>
</div>
<div class="he-panel he-panel-p4" id="he-fr-ph4" hidden>
<p>L'agent défend un point de vue et vous pouvez être d'accord, en désaccord ou nuancer. Peu importe que vos propos correspondent ou non à ce que vous pensez vraiment.</p>
<p>Message typique (en anglais) : <em>"I see your point, but I think working in the office helps newcomers learn faster."</em></p>
</div>
<div class="he-panel he-panel-p5" id="he-fr-ph5" hidden>
<p>L'agent résume l'entretien et conclut la conversation. Un message de clôture poli suffit.</p>
<p>Message typique (en anglais) : <em>"Thank you for your time, I enjoyed our discussion and I hope to hear from you soon."</em></p>
</div>
</div>

## Quoi observer {#he-criteria-fr}

Chaque tour demande une à trois des caractéristiques ci-dessous, et vous ne jugez que celles affichées. La question à garder en tête est de savoir quelle réponse montre le plus clairement le style demandé, quelle que soit votre préférence personnelle. Une réponse aimable et bien écrite peut très bien passer à côté de la cible.

| Caractéristique | Valeurs possibles | Description |
|---|---|---|
| Niveau de langue | A1, A2, B1, B2, C1, C2 | La sophistication de l'anglais, de basique (A1) à avancé (C2).<sup><a href="#he-cefr-fr">1</a></sup><br>A1 : expressions quotidiennes familières et phrases très basiques.<br>A2 : phrases simples sur des sujets du quotidien comme la famille, les achats ou le travail.<br>B1 : langage standard clair sur des sujets familiers, capable de décrire des expériences et de donner brièvement des raisons et des opinions.<br>B2 : texte clair et détaillé sur une grande variété de sujets, y compris abstraits et techniques, avec des points de vue expliqués.<br>C1 : langage fluide, souple et bien structuré sur des sujets complexes, avec du sens implicite.<br>C2 : tout ou presque exprimé avec aisance, très couramment et précisément, avec des nuances fines. |
| Polarité | Positive, Negative, Neutral | Le sentiment global du texte, comme en analyse de sentiments : le message paraît-il positif, négatif, ou ni l'un ni l'autre ? |
| Charge émotionnelle | Loaded, Non loaded | Indique si le texte montre une émotion perceptible (Loaded) ou aucune (Non loaded). |

<p class="he-footnote" id="he-cefr-fr"><sup>1</sup> Descriptions des niveaux résumées à partir du <a href="https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions">Cadre européen commun de référence pour les langues (CECR)</a>, Conseil de l'Europe (site en anglais).</p>

*Neutral* et *Non loaded* décrivent l'absence de sentiment ou d'émotion : il faut donc choisir la réponse la plus sobre et la plus factuelle.

## En cas de blocage {#he-stuck-fr}

### Au cours de la conversation

**Difficile de démarrer ?** Dans cette expérience, c'est vous qui entamez la conversation. Si besoin, cliquez sur **Need help to get started?** pour que l'on vous propose quelques phrases d'ouverture. Sélectionnez celle qui vous convient, modifiez-la si vous le souhaitez et envoyez le message. L'utilisation d'une des phrases proposées n'aura aucune influence sur le déroulé de l'expérience.

<div class="he-row">
<figure class="he-fig">
<img src="/images/he-starters1.png" alt="Le chat vide avec le lien Need help to get started?" width="2134" height="1570" loading="lazy">
<figcaption>À l'ouverture du chat, cliquez sur <strong>Need help to get started?</strong>, juste sous les consignes.</figcaption>
</figure>
<figure class="he-fig">
<img src="/images/he-starters2.png" alt="La liste de six phrases d'ouverture proposées" width="2136" height="1546" loading="lazy">
<figcaption>Cliquez sur une phrase : elle va dans la zone de message, et vous pouvez la modifier avant de l'envoyer.</figcaption>
</figure>
</div>

<div class="he-split he-split-widefig" markdown="1">
<div markdown="1">

**En panne d'inspiration ?** Si vous ne savez pas quoi écrire au cours de la conversation, le panneau de droite propose un bouton **Pick a persona** qui vous donne un personnage tiré au hasard à incarner, avec un métier souhaité, un parcours d'études et un parcours professionnel. Si le personnage tiré aléatoirement ne vous convient pas, vous pouvez en avoir un autre en cliquant à nouveau sur le même bouton. Vous pouvez tout à fait décider de suivre ou non les caractéristiques mentionnées, cette option est simplement là si vous avez besoin d'inspiration. Cela n'aura aucune influence sur le déroulé de l'expérience.

</div>
<figure class="he-fig">
<div class="he-persona">
<img src="/images/he-persona-click.png" alt="Le panneau de droite avec le bouton Pick a persona" width="1126" height="1554" loading="lazy">
<div class="he-persona-stack">
<img src="/images/he-persona1.png" alt="La fiche de Fatou, candidate à un poste de comptable" width="838" height="658" loading="lazy">
<img src="/images/he-persona2.png" alt="La fiche de Paul, candidat à un poste de chargé de communication" width="816" height="558" loading="lazy">
</div>
</div>
<figcaption>À gauche, le panneau de droite avec le bouton <strong>Pick a persona</strong>. À droite, deux personnages que vous pourriez obtenir : le bouton devient alors <strong>Pick another persona</strong>.</figcaption>
</figure>
</div>

### Au moment de l'évaluation

<div class="he-split" markdown="1">
<div markdown="1">

Si vous n'arrivez pas à départager les deux réponses par rapport au respect des caractéristiques mentionnées, cochez **I can't decide** et confirmez. Une réponse sera alors tirée au hasard pour permettre de continuer la conversation. Dans le cas où les deux réponses sont parfaitement identiques, le système le détectera automatiquement. Dans ce cas vous n'aurez rien à choisir. Répondez simplement à l'agent pour poursuivre la conversation.

</div>
<figure class="he-fig">
<img src="/images/he-cant-decide.png" alt="Une note au-dessus du message de l'agent indiquant qu'une réponse a été tirée au hasard" width="1586" height="626" loading="lazy">
<figcaption>Après <strong>I can't decide</strong>, une note au-dessus du message vous indique que la réponse a été tirée au hasard.</figcaption>
</figure>
</div>

## Signaler un problème {#he-flag-fr}

<div class="he-split he-split-midfig" markdown="1">
<div markdown="1">

Si le dernier message de l'agent vous paraît anormal, cliquez sur **Flag Inconsistency** dans le panneau de droite. Cela n'interrompt pas l'entretien. Vous pouvez indiquer que l'agent reste bloqué dans la phase précédente ou saute vers une phase inadaptée (phase-level), qu'il oublie ou contredit quelque chose dit plus tôt (context-level), que le texte n'a pas de sens, ou décrire autre chose en quelques mots.

<figure class="he-fig">
<img src="/images/he-flag-inconsistency.png" alt="Le bouton Flag Inconsistency et la liste des incohérences courantes" width="1052" height="698" loading="lazy">
<figcaption>Le bouton se trouve dans le panneau de droite, avec un rappel des problèmes les plus courants.</figcaption>
</figure>

</div>
<figure class="he-fig">
<img src="/images/he-report-inconsistency.png" alt="Le formulaire de signalement, avec quatre types au choix" width="1152" height="1714" loading="lazy" class="he-crop-bottom">
<figcaption>Le formulaire qui s'ouvre : choisissez un type, ou <strong>Other</strong> pour décrire le problème avec vos mots.</figcaption>
</figure>
</div>

## À savoir {#he-know-fr}

Merci de ne pas écrire de données personnelles comme votre nom, votre adresse ou votre employeur. Inventez des détails si vous le souhaitez.

L'agent construit deux réponses pour chaque message, donc l'attente est normale. Évitez simplement de laisser la page inactive trop longtemps : après 30 minutes sans action, la conversation est fermée.

<div class="he-split he-split-commentfig" markdown="1">
<div markdown="1">

Après le 12e choix, vous pouvez laisser un commentaire si vous le souhaitez, puis fermer la page. Nous enregistrons vos messages, vos choix, votre temps de réponse, les problèmes signalés, votre commentaire et les réponses facultatives à « About you ». Aucun nom ni adresse email n'est demandé. L'objet de la comparaison est expliqué à la fin de l'expérience, pour ne pas influencer vos choix.

</div>
<figure class="he-fig">
<img src="/images/he-leave-comment.png" alt="La fenêtre de fin d'entretien avec un champ de commentaire facultatif" width="1894" height="1312" loading="lazy">
<figcaption>Le dernier écran : le commentaire est facultatif.</figcaption>
</figure>
</div>

## Participer {#he-contact-fr}

Si vous souhaitez participer, ou si vous avez une question, [contactez-moi](mailto:barbara.gendron@loria.fr).

## À propos de la recherche {#he-about-fr}

Cette étude s'inscrit dans ma thèse au LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, encadrée par Mathieu d'Aquin (LORIA, CNRS) et Gaël Guibon (LIPN, Université Sorbonne Paris Nord). La thèse explore comment guider un modèle de langage avec une stratégie conversationnelle construite à partir de concepts et de règles formalisés, afin que son comportement soit plus prévisible et mieux adapté à son cas d'usage. L'entretien d'embauche est le cadre du prototype développé dans ce travail.

</div>

<script>
document.addEventListener('click', function (e) {
  var btn = e.target.closest('.he-phase');
  if (!btn) return;
  var block = btn.closest('.he-phase-block');
  var open = btn.getAttribute('aria-expanded') === 'true';
  block.querySelectorAll('.he-phase').forEach(function (b) {
    b.setAttribute('aria-expanded', 'false');
    document.getElementById(b.getAttribute('aria-controls')).hidden = true;
  });
  if (!open) {
    btn.setAttribute('aria-expanded', 'true');
    document.getElementById(btn.getAttribute('aria-controls')).hidden = false;
  }
});

function setLang(lang) {
  document.getElementById('content-en').style.display = (lang === 'en') ? 'block' : 'none';
  document.getElementById('content-fr').style.display = (lang === 'fr') ? 'block' : 'none';
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  document.getElementById('btn-fr').classList.toggle('active', lang === 'fr');
}
</script>
