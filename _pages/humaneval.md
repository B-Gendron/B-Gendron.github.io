---
layout: single
title: "Human Evaluation"
permalink: /humaneval/
author_profile: true
---

<div class="lang-switcher">
  <button id="btn-en" class="lang-btn active" onclick="setLang('en')">🇬🇧 English</button>
  <button id="btn-fr" class="lang-btn" onclick="setLang('fr')">🇫🇷 Français</button>
</div>

<div id="content-en" class="lang-content" markdown="1">

  This page hosts a human evaluation study for the conversational agent I built during my PhD at LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, supervised by **Mathieu d'Aquin** (LORIA, CNRS) and **Gaël Guibon** (LIPN, Université Sorbonne Paris Nord).

The idea: guide the model with a conversation strategy defined from formal concepts and rules, giving a set of explicit constraints laid on top of a language model to make its behaviour more predictable and relevant to the use-case. The prototype simulates a job interview across five stages:

<style>
.phase {
  padding: 0.8em 1em;
  margin: 0.6em 0;
  border-radius: 6px;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.phase1 { background-color: #667eea; }
.phase2 { background-color: #48bb78; }
.phase3 { background-color: #f6ad55; }
.phase4 { background-color: #ed64a6; }
.phase5 { background-color: #9f7aea; }
.phase-turns { font-style: italic; font-size: 0.85em; opacity: 0.9; white-space: nowrap; margin-left: 1em; }
</style>

<div class="phase phase1"><strong>Phase 1 — Greetings and small talk</strong><span class="phase-turns">2 turns</span></div>

<div class="phase phase2"><strong>Phase 2 — Background and experience</strong><span class="phase-turns">3 turns</span></div>

<div class="phase phase3"><strong>Phase 3 — Technical discussion</strong><span class="phase-turns">3 turns</span></div>

<div class="phase phase4"><strong>Phase 4 — Short debate</strong><span class="phase-turns">2 turns</span></div>

<div class="phase phase5"><strong>Phase 5 — Summary and send-off</strong><span class="phase-turns">2 turns</span></div>

At each stage, the model is expected to respect constraints on language level, polarity, emotional tone, and fit with the current stage.

<h2>Taking part</h2>

For each context, you'll see two possible responses and pick the one that fits best. You can also flag inconsistencies — the agent stuck in the wrong stage, contradicting itself, or forgetting something said earlier. No AI background needed, just read the guide first:

* [Annotator guide — English (PDF)](/files/annotator-guide-en.pdf)

Questions, or want to take part? [Get in touch](mailto:barbara.gendron@loria.fr).

</div>

<div id="content-fr" class="lang-content" markdown="1" style="display:none;">

  Cette page présente une étude d'évaluation humaine pour l'agent conversationnel développé pendant ma thèse au LORIA, *Controlled Conversational Models through Conversation-Dedicated Ontology*, encadrée par **Mathieu d'Aquin** (LORIA, CNRS) et **Gaël Guibon** (LIPN, Université Sorbonne Paris Nord).

L'idée : guider le modèle par une stratégie conversationnelle définie à partir de concepts et de règles formalisés, apportant un ensemble de contraintes explicites posées sur un modèle de langage afin de rendre son comportement plus prévisible et plus pertinent pour le cas d'usage. Le prototype simule un entretien d'embauche en cinq étapes :

<div class="phase phase1"><strong>Phase 1 — Accueil et discussion informelle</strong><span class="phase-turns">2 tours</span></div>

<div class="phase phase2"><strong>Phase 2 — Parcours et expérience</strong><span class="phase-turns">3 tours</span></div>

<div class="phase phase3"><strong>Phase 3 — Discussion technique</strong><span class="phase-turns">3 tours</span></div>

<div class="phase phase4"><strong>Phase 4 — Court débat</strong><span class="phase-turns">2 tours</span></div>

<div class="phase phase5"><strong>Phase 5 — Conclusion et prise de congé</strong><span class="phase-turns">2 tours</span></div>

À chaque étape, le modèle doit respecter des contraintes de niveau de langue, de polarité, de charge émotionnelle et de cohérence avec l'étape en cours.

<h2>Participer</h2>

Pour chaque contexte, vous verrez deux réponses possibles et choisirez celle qui correspond le mieux. Vous pouvez aussi signaler des incohérences — l'agent resté bloqué dans une étape précédente, qui se contredit, ou qui oublie une information donnée plus tôt. Aucune expertise en IA n'est nécessaire, il suffit de lire le guide de l'annotateur :

* [Guide de l'annotateur — Français (PDF)](/files/annotator-guide-fr.pdf)

Des questions, envie de participer ? [Contactez-moi](mailto:barbara.gendron@loria.fr).

</div>

<script>
function setLang(lang) {
  document.getElementById('content-en').style.display = (lang === 'en') ? 'block' : 'none';
  document.getElementById('content-fr').style.display = (lang === 'fr') ? 'block' : 'none';
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  document.getElementById('btn-fr').classList.toggle('active', lang === 'fr');
}
</script>

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
</style>