# Awesome Javascript Anti Debugging [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Curated list of Javascript Anti Debugging techniques 

When it comes to Web Security there is a wide range of different aspects to it. 
The most discussed aspect is the different types of security breaches, such as XSS, CSRF and more.

Javascript Anti Debugging on the other hand is an aspect that is not disscued enough, but might have a large potential impact when it comes to attacking and defending in the web security world. 

*Please read the [contribution guidelines](CONTRIBUTING.md) before contributing.*

By [Gal Weizman](https://weizman.github.io/website/)

## Contents

- [Intro](#intro)
  - [What Is Browser Anti Debugging?](#what-is-browser-anti-debugging)
- ["New Gen" Techniques](#new-gen-technique)
  - [SourceMappingURL](#sourcemappingurl)
- ["Old Gen" Techniques](#old-gen-technique)
  - [TimeDiff](#time-diff)
  - [ChromeGetter](#chrome-getter)
  - [CodeIntegrity](#code-integrity)
  - [FlowIntegrity](#flow-integrity)
  - [HooksDetection](#hooks-detection)
  - [RestrictionalEnviroments](#restrictional-enviroments)
  - [SizeChanges](#size-changes)
  - [debugger;](#debugger)

<a name="intro"></a>
### Intro

<a name="what-is-browser-anti-debugging"></a>
#### What Is Browser Anti Debugging?

Anti Debugging techniques allow attackers to tell whether their malicious code is being inspected or not when is executed within the browser.
The idea is to use the tools given by the browser (which is simply javascript in most cases) to understand whether the website's source code is being inspected and/or debugged in any way, and to take different actions based on the result. 

Usually, these techniques are used by attackers to hide their malicious activity and protect their code from being uncovered. 
Meaning, attackers can protect their code using anti debugging techniques, that when find that the code is being inspected stop the attack instead of completing it.

<a name="new-gen-technique"></a>
### ["New Gen" Techniques](./NewGenTechniques)

<a name="sourcemappingurl"></a>
#### [SourceMappingURL](./NewGenTechniques/SourceMappingURL)

<a name="old-gen-technique"></a>
### ["Old Gen" Techniques](./OldGenTechniques)

<a name="time-diff"></a>
#### [TimeDiff](./OldGenTechniques/TimeDiff)

<a name="chrome-getter"></a>
#### [ChromeGetter](./OldGenTechniques/ChromeGetter)

<a name="code-integrity"></a>
#### [CodeIntegrity](./OldGenTechniques/CodeIntegrity)

<a name="flow-integrity"></a>
#### [FlowIntegrity](./OldGenTechniques/FlowIntegrity)

<a name="hooks-detection"></a>
#### [HooksDetection](./OldGenTechniques/HooksDetection)

<a name="restrictional-enviroments"></a>
#### [RestrictionalEnviroments](./OldGenTechniques/RestrictionalEnviroments)

<a name="size-changes"></a>
#### [SizeChanges](./OldGenTechniques/SizeChanges)

<a name="debugger"></a>
#### [debugger;](./OldGenTechniques/debugger;)



