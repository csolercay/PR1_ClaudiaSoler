# PR1_ClaudiaSoler
# FlashBreath

**FlashBreath** és una aplicació Android desenvolupada amb **Capacitor** i **p5.js** que proposa un exercici de respiració guiada mitjançant una visualització generativa. L’app combina animació, interacció i funcionalitats natives per ajudar a millorar la consciència respiratòria.

---

## Objectiu de l’aplicació

FlashBreath està dirigida principalment a:

- Persones amb **ansietat** que necessiten una eina senzilla per regular la respiració.
- Usuaris que volen **aprendre a controlar el ritme respiratori**.
- Pràctiques de **relaxació, meditació o ioga**.
- Persones que busquen pauses conscients durant el dia.

La visualització abstracta del cercle ajuda a **sincronitzar la respiració**: creix durant la inhalació i decreix durant l’exhalació, creant un ritme visual fàcil de seguir.

---

## Tecnologies utilitzades

- Capacitor (Android)
- Android Studio
- JavaScript
- p5.js (canvas i animació generativa)
- HTML / CSS
- LocalStorage (persistència de dades)
- APIs natives d’Android (flash / vibració)

---

## Funcionalitats principals

- Canvas amb animació generativa sincronitzada amb el temps.
- Control de respiració mitjançant els botons **Iniciar** i **Detener**.
- Panell de configuració desplegable:
  - Durada del cicle respiratori.
  - Color del cercle.
  - Activació del flash durant la inhalació.
- Persistència de dades mitjançant `localStorage`.
- Interfície adaptada a dispositius mòbils.
- Integració amb funcionalitats natives del dispositiu.

---

## Explicació del codi

- **index.html**  
  Defineix l’estructura principal de la interfície: capçalera, canvas central, botons de control i panell de configuració. També carrega les llibreries i scripts en l’ordre correcte.

- **style.css**  
  Controla la disposició visual de l’app: distribució vertical, centrament del canvas, botons a la part inferior ocupant l’amplada del dispositiu, disseny responsive i estil fosc coherent amb l’objectiu de relaxació.

- **app.js**  
  Gestiona la lògica de la interfície d’usuari: esdeveniments dels botons, obertura i tancament del panell de configuració, guardat de preferències a `localStorage` i comunicació amb el sketch de p5.js.

- **p5-sketch.js**  
  Conté la lògica de l’animació generativa. Calcula el temps del cicle respiratori, genera el creixement i decreixement del cercle amb funcions d’easing i sincronitza la visualització amb l’estat de respiració.

---

> ❗ No s’inclouen `node_modules` ni `www`, tal com indiquen les bones pràctiques i els requisits del lliurament.

---

## 🚀 Instal·lació i execució (avaluació)

### Requisits previs

- Node.js (versió LTS)
- npm
- Android Studio
- Android SDK i Emulator configurat

### Passos d’instal·lació

```bash
npm install
npm run build
npx cap sync android
npx cap open android
```

---

###Llicència
Aquest projecte es distribueix sota la llicència MIT.

---

### Claudia
Projecte acadèmic desenvolupat per a una assignatura universitària: Desenvolupamernt d'Aplicacions Interactives
Any: 2025-2026


