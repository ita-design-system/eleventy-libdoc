---
title: Sandbox from srcdoc
description: Include a sandbox without a file, input code directly into your page
layout: simple_page.liquid
eleventyNavigation:
    key: Sandbox from srcdoc
    parent: Samples
tags: first
---
```liquid
{% raw %}{% sandbox %}
<!-- your HTML -->
{% endsandbox %}{% endraw %}
```

# Example 1

{% sandbox %}
<h1>Hello</h1>
<script>
    document.querySelector('h1').innerHTML += ' World!';
</script>
{% endsandbox %}

# Example 2

{% sandbox 'Custom title' %}
<nav c-scrollsyncbar="">
    <a href="#">c-scrollsyncbar.js</a>
</nav>

<p>Défiler vers le bas pour observer l'effet, vers le haut pour inverser immédiatement le mouvement.</p>

<p>ScrollSyncBar est une barre d'affichage et de masquage synchronisée avec le défilement de la fenêtre.</p>

<p>ScrollSyncBar permet d'afficher et de masquer progressivement la navigation ou tout autre élément en synchronisation avec le défilement de la fenêtre.</p>

<nav id="commands">
    <menu>
        <li><button onclick="cScrollSyncBar.update()">cScrollSyncBar.update()</button> <br>Initialise en créant les instances des éléménts à activer</li>
        <li><button onclick="cScrollSyncBar.update({scrollSteps:500})">cScrollSyncBar.update({scrollSteps:500})</button> <br>Plus le paramètre scrollSteps est élevé, plus la course du défilement nécessaire est longue (200 par défaut)</li>
        <li><button onclick="cScrollSyncBar.update({scrollSteps:50})">cScrollSyncBar.update({scrollSteps:50})</button> <br>Plus le paramètre scrollSteps est petit, plus la course du défilement nécessaire est courte (200 par défaut)</li>
        <li><button onclick="cScrollSyncBar.pause()">cScrollSyncBar.pause()</button> <br>Stoppe et laisse l'élément en l'état</li>
        <li><button onclick="cScrollSyncBar.stop()">cScrollSyncBar.stop()</button> <br>Stoppe et rétablit l'état d'origne de l'élément</li>
        <li><button onclick="cScrollSyncBar.start()">cScrollSyncBar.start()</button> <br>Démarre la synchronisation</li>
    </menu>
</nav>

<nav c-scrollsyncbar="bar">
    <a href="#">Retour vers le haut</a>
</nav>

<!-- DEMO ONLY -->
<link rel="stylesheet" href="https://ita-design-system.github.io/starter-template/ui/css/briks_css_variables.css">
<style>
    * {
        box-sizing: border-box;
    }
    body {
        min-height: 500vh;
        padding: var(--ita-spacing-14) var(--ita-spacing-8);
        color: var(--ita-color-primary-800);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        background-color: ghostwhite;
    }
    #commands {
        margin-top: 10em;
        margin-bottom: 10em;
        position: sticky;
        top: 5em;
    }
    #commands menu {
        display: flex;
        flex-direction: column;
        gap: 1em;
    }
    [c-scrollsyncbar=""] {
        position: fixed;
        top: 0%;
        left: 0;
        width: 100%;
        padding: 1em;
        background-color: var(--ita-color-primary-500);
    }
    [c-scrollsyncbar="bar"] {
        position: fixed;
        top: 100%;
        left: 0;
        width: 100%;
        padding: 2em;
        background-color: var(--ita-color-support-success-100);
    }
    [c-scrollsyncbar=""] a {
        color: var(--ita-color-neutral-100);
    }
    [c-scrollsyncbar="bar"] a {
        color: var(--ita-color-support-success-700);
    }
</style>
<script src="https://ita-design-system.github.io/c-scrollsyncbar.js/ui/js/c-scrollsyncbar.js"></script>
{% endsandbox %}