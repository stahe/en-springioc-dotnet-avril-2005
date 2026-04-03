# Spring IoC pour .NET

➡️ Cours associé : **[Spring IoC pour .NET](https://stahe.github.io/springioc-dotnet-avril-2005/)**

Ce document présente les principes de **l'inversion de contrôle (IoC – Inversion of Control)** et leur mise en œuvre dans l'écosystème **.NET** grâce au framework **Spring.NET**, adaptation du framework **Spring** initialement conçu pour Java. 

L'objectif est de montrer comment améliorer la conception d'applications en **découplant les composants** et en déléguant leur assemblage à un conteneur de configuration.

---

# Objectifs du document

Ce tutoriel a pour objectifs :

- découvrir les possibilités de **configuration et d’intégration du framework Spring** dans une application .NET  
- comprendre la notion d’**Inversion of Control (IoC)**  
- apprendre à utiliser l’**injection de dépendances (Dependency Injection)** pour découpler les composants  
- mettre en œuvre ces concepts dans des **exemples concrets en VB.NET** 

---

# Contexte

Les idées présentées dans ce document s’inspirent fortement du livre de **Rod Johnson** :

**J2EE Development without EJB (Wrox, 2004)**

Ce livre a posé les bases de la philosophie Spring : construire des applications plus simples, plus modulaires et plus testables en évitant les dépendances lourdes des frameworks traditionnels.

Un document similaire existe déjà pour **Spring / Java**.  
Le présent tutoriel reprend les mêmes concepts et les **adapte à la plate-forme .NET**. 

---

# Spring.NET

Au moment de la rédaction du document :

- **Spring.NET** est en version **0.6 RC3 (avril 2005)**  
- seules certaines fonctionnalités du Spring Java original sont portées  
- les fonctionnalités essentielles sont cependant disponibles :

- **Inversion of Control (IoC)**
- **Programmation orientée aspects (AOP)**

Ce tutoriel se concentre principalement sur **l’IoC**, qui constitue le cœur de la philosophie Spring. 

---

# Principe : Inversion of Control (IoC)

Dans une architecture classique, un objet :

- crée lui-même ses dépendances
- contrôle directement les objets dont il a besoin

Avec **IoC** :

- les dépendances sont **injectées par un conteneur**
- les composants deviennent **faiblement couplés**
- la configuration est **externalisée**

Cela permet :

- une **meilleure maintenabilité**
- une **plus grande testabilité**
- une **architecture plus flexible**

---

# Exemples pratiques

La partie pratique du document contient plusieurs exemples illustrant :

- la configuration de composants Spring.NET
- l’injection de dépendances
- la mise en place d’objets métier découplés

Les exemples sont écrits en **VB.NET**.

Les tests utilisent le framework **NUnit**, équivalent .NET du framework **JUnit** utilisé dans l’écosystème Java. 

---

# Prérequis

Pour suivre les exemples :

- environnement **.NET**
- **Spring.NET**
- **NUnit** pour l'exécution des tests unitaires

Les annexes du document expliquent :

- où télécharger ces outils
- comment les installer

---

# Philosophie Spring

L'intérêt principal de Spring ne réside pas uniquement dans ses mécanismes techniques, mais surtout dans sa **philosophie de conception** :

- séparation des responsabilités  
- faible couplage entre composants  
- configuration externe des dépendances  
- architecture orientée test

Ces principes permettent de concevoir des applications **plus simples, plus modulaires et plus robustes**.

