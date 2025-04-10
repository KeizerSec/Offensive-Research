# Low-Level Notes – Payloads, Syscalls & Hooking

🛑 **Avertissement :** Ce document est strictement éducatif. Il vise à partager des notions explorées dans un cadre d'apprentissage de la cybersécurité offensive, dans un environnement personnel. Aucune de ces pratiques ne doit être utilisée en dehors d'un cadre légal, éthique et autorisé.

## 🧠 Objectif

Partager quelques réflexions, expériences et rappels personnels sur :
- L’injection mémoire
- Le bypass antivirus (AV/EDR)
- Le hooking d’API
- La création de payloads simples via `syscall`
- Le fonctionnement interne des moteurs de jeu

## 🔹 Syscall & AV Bypass

- J’ai appris à générer des payloads en utilisant `syscall()` pour éviter les signatures des antivirus classiques (ex: Windows Defender à l'époque).
- L’objectif était de comprendre comment un antivirus repère un shellcode en mémoire.
- J’utilisais des outils type C/Assembly pour interagir directement avec les API Windows sans utiliser les fonctions classiques (CreateProcess, etc.).

## 🔹 DLL Injection & Hooking

- Injection de DLL testées dans des moteurs de jeu.
- Hook de fonctions graphiques ou système (ex: `GetAsyncKeyState`, `ReadProcessMemory`), pour détourner des appels ou insérer du code.
- Compréhension des points d’injection (IAT, EAT, inline patching).

## 🔹 Exploration mémoire

- Manipulation de la mémoire en environnement sandbox
- Observation de structures de données, de buffers, et modification en live
- Utilisation de `cheat engine` à titre personnel pour comprendre comment fonctionnent les modifications runtime

## 🔹 Philosophie

Ce n’est pas une pratique orientée “cheat”, mais une volonté de comprendre **les mécaniques internes** d’un système, d’un moteur de jeu ou d’un programme natif.

Je ne prétends pas tout maîtriser, mais je souhaite montrer :
- ma capacité à comprendre des sujets complexes,
- ma curiosité profonde,
- et mon éthique dans la manière de traiter ce savoir.
