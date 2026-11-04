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

.he-summary {
  border-left: 4px solid #667eea;
  background: #f3f4fc;
  padding: 0.8em 1.1em;
  margin: 1em 0 1.5em;
  border-radius: 0 6px 6px 0;
}
.he-summary ul { margin: 0.3em 0 0; }
.he-phases { display: flex; flex-wrap: wrap; gap: 0.4em; margin: 0.8em 0 1em; }
.he-phase { color: #fff; padding: 0.35em 0.8em; border-radius: 999px; font-size: 0.85em; white-space: nowrap; }
.he-p1 { background: #667eea; }
.he-p2 { background: #48bb78; }
.he-p3 { background: #f6ad55; }
.he-p4 { background: #ed64a6; }
.he-p5 { background: #9f7aea; }
.he-toc { font-size: 0.9em; margin-bottom: 1.5em; }
.he-toc a { margin-right: 1em; white-space: nowrap; }
</style>

<div class="lang-switcher">
  <button id="btn-en" class="lang-btn active" onclick="setLang('en')">🇬🇧 English</button>
  <button id="btn-fr" class="lang-btn" onclick="setLang('fr')">🇫🇷 Français</button>
</div>

<div id="content-en" class="lang-content" markdown="1">

This page is the participant guide for a human evaluation study of the conversational agent built during my PhD at LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, supervised by **Mathieu d'Aquin** (LORIA, CNRS) and **Gaël Guibon** (LIPN, Université Sorbonne Paris Nord). No AI background is needed.

<div class="he-summary" markdown="1">
**The experiment in short**

* You play **a candidate in a mock job interview**. The other side is **a recruiter agent** (a chatbot).
* You send **12 messages**. There are no right or wrong answers: **the agent is being evaluated, not you.**
* After each message, the agent proposes **two replies**. You pick the one that **shows more clearly the requested style**, and the conversation continues with it.
* Anonymous, voluntary, and you can stop at any time by closing the page.
</div>

<div class="he-toc">
<a href="#he-steps">How a turn works</a>
<a href="#he-criteria">What to judge</a>
<a href="#he-stuck">Stuck?</a>
<a href="#he-flag">Flag a problem</a>
<a href="#he-know">Good to know</a>
<a href="#he-contact">Take part</a>
</div>

## Before you start {#he-before}

1. Read the information screen and tick the consent box.
2. Optionally fill in a short **"About you"** form (age range, English level, interview experience...). You can skip it. The agent never sees it.
3. Click start and wait a moment while the interview is prepared.

Only **one person can take part at a time**. If the page says someone else is taking the experiment, come back in a few minutes.

## How a turn works {#he-steps}

1. **Write your message** and send it. Answer as in a real interview, in a few sentences.
2. **Wait** for the agent (a few seconds to a few minutes). Don't close the page; if you reload it, your conversation is kept.
3. **Read the requested style** shown above the two replies, e.g. *"The agent response is expected to be Positive, Non loaded, B1."*
4. **Read both replies.** Left or right is random.
5. **Click the reply that shows this style more clearly**, then **Confirm choice**.

The agent leads the interview through five phases, always shown at the top of the chat. You don't have to follow them, just answer naturally.

<div class="he-phases">
<span class="he-phase he-p1">1 Greetings</span>
<span class="he-phase he-p2">2 Background</span>
<span class="he-phase he-p3">3 Technical point</span>
<span class="he-phase he-p4">4 Short debate</span>
<span class="he-phase he-p5">5 Send-off</span>
</div>

## What to judge {#he-criteria}

The question is **not** "which reply is nicer or better written?" but **"which one shows the requested style more clearly?"** Each turn shows one to three of these characteristics. Only judge the ones displayed.

| Characteristic | Values | In plain words |
|---|---|---|
| **Language level** | A1-A2 / B1-B2 / C1-C2 | How sophisticated the English is. **A1-A2**: very simple words and short sentences. **B1-B2**: everyday language. **C1-C2**: rich vocabulary, complex sentences. |
| **Polarity** | Positive / Negative / Neutral | Attitude of the reply: encouraging, critical, or neither. |
| **Emotional load** | Loaded / Non loaded | **Loaded**: expresses or insists on feelings. **Non loaded**: calm and factual. |

Tips:

* Judge what is **requested**, not what you like. A pleasant reply can still miss the target.
* *Neutral* and *Non loaded* mean the **absence** of attitude or emotion: pick the plainer, more factual reply.
* For a basic level (A1-A2), the **simpler** English wins.

## Stuck? {#he-stuck}

* **Can't tell the replies apart** (equally good or equally bad): tick **"I can't decide"** and confirm. One reply is picked at random to continue, and a note tells you so. This is a valid answer.
* **Identical replies**: nothing to choose, a note says *"No choice to make"*.
* **Don't know what to write?** In the right panel, **Pick a persona** gives you a random character to play (adapt it freely). Before your first message, **"Need help to get started?"** offers opening lines. The agent never sees these aids.

## Flag a problem (optional) {#he-flag}

If the last agent message seems wrong, click **Flag Inconsistency** in the right panel. It doesn't interrupt the interview.

* **Phase-level**: the agent stays in the previous phase or jumps to one that doesn't fit.
* **Context-level**: it forgets or contradicts something said earlier.
* **Nonsensical**: the text doesn't make sense.
* **Other**: describe it in a few words.

## Good to know {#he-know}

* **Don't write personal data** (name, address, employer...). Invent details if you like.
* After **30 minutes without any action**, the conversation is closed.
* Waiting is normal: the agent builds two replies for every message.
* After the 12th choice, you can leave an optional comment, then close the page.
* **What is recorded**: your messages, choices, response times, flags, comment and optional "About you" answers. No name or email is asked.
* The purpose of the comparison is explained at the end of the experiment, so as not to influence your choices.

## Take part {#he-contact}

Want to take part, or have a question? [Get in touch](mailto:barbara.gendron@loria.fr).

</div>

<div id="content-fr" class="lang-content" markdown="1" style="display:none;">

Cette page est le guide du participant pour une étude d'évaluation humaine de l'agent conversationnel développé pendant ma thèse au LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, encadrée par **Mathieu d'Aquin** (LORIA, CNRS) et **Gaël Guibon** (LIPN, Université Sorbonne Paris Nord). Aucune connaissance en IA n'est nécessaire.

<div class="he-summary" markdown="1">
**L'expérience en bref**

* Vous jouez **un candidat lors d'un faux entretien d'embauche**. En face, **un agent recruteur** (un chatbot).
* Vous envoyez **12 messages**. Il n'y a ni bonne ni mauvaise réponse : **c'est l'agent qui est évalué, pas vous.**
* Après chaque message, l'agent propose **deux réponses**. Vous choisissez celle qui **montre le plus clairement le style demandé**, et la conversation continue avec elle.
* Anonyme, volontaire, et vous pouvez arrêter à tout moment en fermant la page.
</div>

<div class="he-toc">
<a href="#he-steps-fr">Déroulé d'un tour</a>
<a href="#he-criteria-fr">Quoi juger</a>
<a href="#he-stuck-fr">Bloqué ?</a>
<a href="#he-flag-fr">Signaler un problème</a>
<a href="#he-know-fr">À savoir</a>
<a href="#he-contact-fr">Participer</a>
</div>

## Avant de commencer {#he-before-fr}

1. Lisez l'écran d'information et cochez la case de consentement.
2. Remplissez si vous le souhaitez un court formulaire **« À propos de vous »** (tranche d'âge, niveau d'anglais, expérience des entretiens...). Il est facultatif, et l'agent ne le voit jamais.
3. Cliquez sur démarrer et patientez le temps que l'entretien soit préparé.

**Une seule personne à la fois** peut participer. Si la page indique qu'une autre personne passe l'expérience, revenez dans quelques minutes.

## Déroulé d'un tour {#he-steps-fr}

1. **Écrivez votre message** et envoyez-le. Répondez comme lors d'un vrai entretien, en quelques phrases.
2. **Patientez** (de quelques secondes à quelques minutes). Ne fermez pas la page ; si vous la rechargez, votre conversation est conservée.
3. **Lisez le style demandé**, affiché au-dessus des deux réponses, par exemple *« The agent response is expected to be Positive, Non loaded, B1. »*
4. **Lisez les deux réponses.** Gauche ou droite est aléatoire.
5. **Cliquez sur la réponse qui montre ce style le plus clairement**, puis sur **Confirm choice**.

L'agent mène l'entretien en cinq phases, toujours affichées en haut du chat. Inutile de les suivre : répondez naturellement.

<div class="he-phases">
<span class="he-phase he-p1">1 Accueil</span>
<span class="he-phase he-p2">2 Parcours</span>
<span class="he-phase he-p3">3 Point technique</span>
<span class="he-phase he-p4">4 Court débat</span>
<span class="he-phase he-p5">5 Conclusion</span>
</div>

## Quoi juger {#he-criteria-fr}

La question n'est **pas** « quelle réponse est la plus agréable ou la mieux écrite ? » mais **« laquelle montre le plus clairement le style demandé ? »** Chaque tour affiche une à trois de ces caractéristiques. Ne jugez que celles affichées.

| Caractéristique | Valeurs | En clair |
|---|---|---|
| **Niveau de langue** | A1-A2 / B1-B2 / C1-C2 | Sophistication de l'anglais. **A1-A2** : mots très simples, phrases courtes. **B1-B2** : langage courant. **C1-C2** : vocabulaire riche, phrases complexes. |
| **Polarité** | Positive / Negative / Neutral | Attitude de la réponse : encourageante, critique, ou ni l'un ni l'autre. |
| **Charge émotionnelle** | Loaded / Non loaded | **Loaded** : exprime ou insiste sur des émotions. **Non loaded** : calme et factuelle. |

Conseils :

* Jugez ce qui est **demandé**, pas ce que vous préférez. Une réponse agréable peut passer à côté de la cible.
* *Neutral* et *Non loaded* signifient l'**absence** d'attitude ou d'émotion : choisissez la réponse la plus sobre et factuelle.
* Pour un niveau de base (A1-A2), l'anglais le **plus simple** l'emporte.

## Bloqué ? {#he-stuck-fr}

* **Impossible de départager** (aussi bonnes ou aussi mauvaises) : cochez **« I can't decide »** et confirmez. Une réponse est tirée au hasard pour continuer, et une note vous le signale. C'est une réponse valide.
* **Réponses identiques** : rien à choisir, une note indique *« No choice to make »*.
* **Pas d'inspiration ?** Dans le panneau de droite, **Pick a persona** vous donne un personnage tiré au hasard (adaptez-le librement). Avant votre premier message, **« Need help to get started? »** propose des phrases d'ouverture. L'agent ne voit jamais ces aides.

## Signaler un problème (facultatif) {#he-flag-fr}

Si le dernier message de l'agent vous semble anormal, cliquez sur **Flag Inconsistency** dans le panneau de droite. Cela n'interrompt pas l'entretien.

* **Phase-level** : l'agent reste dans la phase précédente ou saute vers une phase inadaptée.
* **Context-level** : il oublie ou contredit un élément dit plus tôt.
* **Nonsensical** : le texte n'a pas de sens.
* **Other** : décrivez-le en quelques mots.

## À savoir {#he-know-fr}

* **N'écrivez aucune donnée personnelle** (nom, adresse, employeur...). Inventez des détails si vous voulez.
* Après **30 minutes sans action**, la conversation est fermée.
* L'attente est normale : l'agent construit deux réponses pour chaque message.
* Après le 12e choix, vous pouvez laisser un commentaire facultatif, puis fermer la page.
* **Ce qui est enregistré** : vos messages, choix, temps de réponse, signalements, commentaire et réponses facultatives « À propos de vous ». Ni nom ni email ne sont demandés.
* L'objectif de la comparaison est expliqué à la fin de l'expérience, pour ne pas influencer vos choix.

## Participer {#he-contact-fr}

Envie de participer, ou une question ? [Contactez-moi](mailto:barbara.gendron@loria.fr).

</div>

<script>
function setLang(lang) {
  document.getElementById('content-en').style.display = (lang === 'en') ? 'block' : 'none';
  document.getElementById('content-fr').style.display = (lang === 'fr') ? 'block' : 'none';
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  document.getElementById('btn-fr').classList.toggle('active', lang === 'fr');
}
</script>
