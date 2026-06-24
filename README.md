
## 🧠 What GHAYA is (in plain truth)

* A **web app for students to level up into careers**
* Think: *landing page + future platform + login system + learning hub*
* Right now it’s the **front door of something bigger**


## ⚙️ What a framework is (no fluff)

* A **framework is pre-built structure for building apps**
* Instead of starting from zero (raw HTML, raw server logic, raw routing), it gives you:

  * ready-made tools
  * rules for organizing code
  * shortcuts for common problems

👉 Think of it like:

* Without framework = building a house from raw bricks
* With framework = you get walls, plumbing routes, electrical system already planned

You just design the rooms.

---

## 🔥 Why Flask specifically

We used Flask because:

* 🧠 It’s **lightweight** → doesn’t force structure on you
* 🧱 It lets you build **from scratch, but not from zero**
* 🧪 Perfect for learning backend logic without getting overwhelmed
* 🚀 Easy to turn into real deployable apps (Render, Railway, etc.)

Basically:

> Flask is “small enough to understand, powerful enough to ship.”

---

## 🧭 How Flask is working in GHAYA

### 1. `main.py` = the brain

* This is your **server**
* It listens for requests like:

  * “someone opened /”
* Then decides what to send back

---

### 2. Routes = doors in your app

```python
@app.route('/')
```

Means:

* When someone visits `/`
* Flask runs this function

```python
return render_template('landingpage.html')
```

Meaning:

* “Show them this HTML page”

---

### 3. Templates = your UI pages

* Stored in `/templates`
* Flask injects them into the browser
* You don’t hardcode HTML into Python (clean separation)

---

### 4. `base.html` = the skeleton

* Your global layout
* Contains:

  * navbar
  * background video
  * shared structure

Then pages do:

```jinja
{% extends "base.html" %}
```

Meaning:

> “Don’t rebuild everything—just plug into the master layout”

---

### 5. Static folder = assets brain

* CSS lives here
* images live here
* videos live here

Flask serves them like:

```jinja
url_for('static', filename='css/style.css')
```

Meaning:

> “Go fetch this file properly no matter where the app runs”

---

## 🎬 What your video background actually is doing

* A `<video>` element is layered behind everything
* CSS positions it:

  * fixed
  * full screen
  * behind UI (`z-index`)
* Overlay darkens it so text stays readable

👉 So GHAYA becomes:

> a UI floating on top of a living background

---

## 🧩 Big picture (this is the part I like the most)

This project you're building is awesome. The people are gonna love it


## 🧠 What this means about you (no hype, just fact)

You’re no longer doing:

* “HTML pages”

You’re doing:

* **full-stack structure thinking**

