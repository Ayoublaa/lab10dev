````md id="lab10drawer"
# LAB 10 — Navigation Drawer et Fragments Android

![Android](https://img.shields.io/badge/Platform-Android-green)
![Java](https://img.shields.io/badge/Language-Java-orange)
![Fragments](https://img.shields.io/badge/UI-Fragments-blue)

## 📌 Description

Ce laboratoire présente la création d’une application Android avec :

- Navigation Drawer
- Fragments
- Menu latéral
- Transactions de fragments

Objectif :
apprendre la navigation modulaire sous Android avec Java.

---

# ⚙️ Prérequis

- Android Studio
- Java
- SDK Android
- Connaissances basiques Android

---

# 🎯 Objectifs

- créer un Navigation Drawer
- gérer plusieurs fragments
- changer les fragments dynamiquement
- utiliser un ListFragment

---

# 🚀 Étape 1 — Création du Projet

Créer un projet Android :

```text id="p7m3kd"
Empty Activity
Language: Java
Minimum SDK: API 21+
````
<img width="1620" height="879" alt="image" src="https://github.com/user-attachments/assets/af024949-6e2c-4c7a-89a2-9a61aca9623c" />

---

# 🎨 Étape 2 — Modifier le Menu

Fichier :

```text id="w9x2vu"
res/menu/activity_main_drawer.xml
```

Ajouter des items :

```xml id="m4q8tn"
<item
    android:id="@+id/nav_home"
    android:title="Home"/>
```

---

# 📱 Étape 3 — Création des Fragments

Créer :

* HomeFragment
* ProfileFragment
* SettingsFragment

Exemple :

```java id="g6r1lp"
public class HomeFragment extends Fragment {

}
```

---

# ⚡ Étape 4 — Ajouter le Conteneur

Dans :

```text id="a8v5qx"
activity_main.xml
```

Ajouter :

```xml id="z3t7wr"
<FrameLayout
    android:id="@+id/fragment_container"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>
```

---

# 🔥 Étape 5 — Afficher les Fragments

Exemple Java :

```java id="u2m9ks"
getSupportFragmentManager()
.beginTransaction()
.replace(R.id.fragment_container, new HomeFragment())
.commit();
```
<img width="276" height="573" alt="image" src="https://github.com/user-attachments/assets/3329dbaa-67e9-4100-8c5b-e22f6fd68a04" />

---

# 📋 Étape 6 — Ajouter un ListFragment

Créer une liste :

```java id="f5p1xb"
public class ListFrag extends ListFragment {

}
```
<img width="1747" height="853" alt="image" src="https://github.com/user-attachments/assets/29ac0aac-b626-4938-9055-71bd68703ed6" />


---

# ▶️ Étape 7 — Exécution

Lancer l’application :

```text id="q4v8ny"
Run > Start App
```

Résultat attendu :

* menu latéral fonctionnel
* fragments dynamiques
* navigation fluide

---
<img width="490" height="936" alt="image" src="https://github.com/user-attachments/assets/a55cb673-f710-4076-9029-bf0b12513f20" />

# ✅ Concepts Appris

* Navigation Drawer
* Fragment Transactions
* Android UI
* Modular Navigation
* ListFragment

---

# 📚 Technologies Utilisées

* Java
* Android Studio
* Android SDK
* Fragments API

---

# ⚠️ Bonnes Pratiques

* séparer chaque écran dans un fragment
* éviter le code dupliqué
* utiliser des noms clairs

---

# 👨‍💻 Auteur

Ayoub Laafar — EMSI Marrakech

```
```
