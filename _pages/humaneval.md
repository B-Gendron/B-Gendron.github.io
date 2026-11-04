---
layout: single
title: "Human Evaluation"
permalink: /humaneval/
author_profile: true
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
.he-footnote { font-size: 0.8em; color: #777; margin: 0.3em 0 1em; }
.he-hint { font-size: 0.8em; font-style: italic; color: #777; margin: 0.5em 0 0; }
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

## Before you start {#he-before}

Read the information screen and tick the consent box. A short "About you" form comes next (age range, English level, interview experience...). You can skip it, and the agent never sees your answers. Then click start and give the page a moment to prepare the interview.

Only one person can take part at a time. If the page tells you someone else is already on it, come back in a few minutes.

## How a turn works {#he-steps}

1. Write your message and send it. Answer the way you would in a real interview, in a few sentences.
2. Wait for the agent, which can take anywhere from a few seconds to a few minutes. If you reload the page, your conversation is kept.
3. Above the two replies, a sentence tells you which style they should have, for example *"The agent response is expected to be Positive, Non loaded, B1."*
4. Read both replies. Which one is on the left or the right is random.
5. Click the one that shows this style more clearly, then click **Confirm choice**. The conversation goes on with the reply you picked.

The agent leads the interview through five phases, and the current one is always displayed at the top of the chat. You don't need to follow them, just answer naturally.

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

When you really can't tell the two replies apart, tick **I can't decide** and confirm. One of them is then picked at random to continue the conversation, and a short note tells you so. It counts as a valid answer. If the two replies are identical, there is nothing to choose and a note says so.

If you don't know what to write, the right panel has a **Pick a persona** button that gives you a random character to play. Adapt it as much as you like. Before your first message, a **Need help to get started?** link also offers a few opening lines. The agent never sees any of this.

## Flagging a problem {#he-flag}

If the last message from the agent looks off, click **Flag Inconsistency** in the right panel. It doesn't interrupt the interview. You can say that the agent is stuck in the previous phase or jumped to a phase that doesn't fit (phase-level), that it forgot or contradicted something said earlier (context-level), that the text makes no sense, or describe something else in a few words.

## Good to know {#he-know}

Please don't write personal data such as your name, address or employer. Invent details if you want to.

The agent builds two replies for every message, so waiting is normal. Try not to leave the page idle for too long: after 30 minutes without any action, the conversation is closed.

After the 12th choice, you can leave a comment if you wish, and then close the page. We record your messages, your choices, how long you take, the problems you flag, your comment and the optional "About you" answers. We don't ask for any name or email address. What the comparison is about is explained at the end of the experiment, so that it doesn't influence your choices.

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

## Avant de commencer {#he-before-fr}

Lisez l'écran d'information et cochez la case de consentement. Un court formulaire « About you » suit (tranche d'âge, niveau d'anglais, expérience des entretiens...). Vous pouvez le passer, et l'agent ne voit jamais vos réponses. Cliquez ensuite sur démarrer et laissez à la page un instant pour préparer l'entretien.

Une seule personne à la fois peut participer. Si la page indique que quelqu'un d'autre est en cours d'expérience, revenez dans quelques minutes.

## Déroulé d'un tour {#he-steps-fr}

1. Écrivez votre message et envoyez-le. Répondez comme dans un vrai entretien, en quelques phrases.
2. Patientez le temps que l'agent réponde, de quelques secondes à quelques minutes. Si vous rechargez la page, votre conversation est conservée.
3. Au-dessus des deux réponses, une phrase indique le style qu'elles doivent avoir, par exemple *« The agent response is expected to be Positive, Non loaded, B1. »*
4. Lisez les deux réponses. Leur position à gauche ou à droite est aléatoire.
5. Cliquez sur celle qui montre ce style le plus clairement, puis sur **Confirm choice**. La conversation continue avec la réponse choisie.

L'agent mène l'entretien en cinq phases, et la phase en cours est toujours affichée en haut du chat. Inutile de les suivre, répondez naturellement.

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

Si vous n'arrivez vraiment pas à départager les deux réponses, cochez **I can't decide** et confirmez. L'une d'elles est alors tirée au hasard pour continuer la conversation, et une courte note vous le signale. C'est une réponse valide. Si les deux réponses sont identiques, il n'y a rien à choisir et une note vous l'indique.

Si vous ne savez pas quoi écrire, le panneau de droite propose un bouton **Pick a persona** qui vous donne un personnage tiré au hasard à incarner. Adaptez-le comme vous voulez. Avant votre premier message, un lien **Need help to get started?** propose aussi quelques phrases d'ouverture. L'agent ne voit rien de tout cela.

## Signaler un problème {#he-flag-fr}

Si le dernier message de l'agent vous paraît anormal, cliquez sur **Flag Inconsistency** dans le panneau de droite. Cela n'interrompt pas l'entretien. Vous pouvez indiquer que l'agent reste bloqué dans la phase précédente ou saute vers une phase inadaptée (phase-level), qu'il oublie ou contredit quelque chose dit plus tôt (context-level), que le texte n'a pas de sens, ou décrire autre chose en quelques mots.

## À savoir {#he-know-fr}

Merci de ne pas écrire de données personnelles comme votre nom, votre adresse ou votre employeur. Inventez des détails si vous le souhaitez.

L'agent construit deux réponses pour chaque message, donc l'attente est normale. Évitez simplement de laisser la page inactive trop longtemps : après 30 minutes sans action, la conversation est fermée.

Après le 12e choix, vous pouvez laisser un commentaire si vous le souhaitez, puis fermer la page. Nous enregistrons vos messages, vos choix, votre temps de réponse, les problèmes signalés, votre commentaire et les réponses facultatives à « About you ». Aucun nom ni adresse email n'est demandé. L'objet de la comparaison est expliqué à la fin de l'expérience, pour ne pas influencer vos choix.

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
