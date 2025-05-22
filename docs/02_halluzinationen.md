# 🧠 Halluzinationen in KI-Modellen: Ein technisches und ethisches Problem

## 📚 Definition

**Halluzinationen** in großen Sprachmodellen (LLMs) wie GPT bezeichnen Ausgaben, die faktisch falsch, erfunden oder nicht durch das zugrundeliegende Trainingsmaterial gestützt sind. Obwohl sie oft plausibel und sprachlich korrekt klingen, entbehren sie jeder realen Grundlage.

---

## 🔬 Arten von Halluzinationen

### 1. 🔍 **Falsche Fakten**

Modelle behaupten, dass ein bestimmter Fehler in Version X eines Programms existiere – obwohl das nie der Fall war.

### 2. 🧩 **Erfundene Referenzen**

Links, Dokumentationshinweise, Quellcodezeilen oder Commit-Hashes, die nie existiert haben.

### 3. 🧪 **Unbelegte Ursachenvermutung**

Die KI "diagnostiziert" eine Ursache, die auf keiner nachvollziehbaren Analyse basiert.

### 4. 📎 **Synthetische Stacktraces**

Fehlermeldungen und Logs, die aus einer logischen Mischung von Mustern bestehen, aber niemals tatsächlich erzeugt wurden.

---

## ⚠️ Warum das gefährlich ist

* ❌ **Verwirrung** für Maintainer und Entwickler, die reale Probleme von KI-Fiktion unterscheiden müssen.
* 🧱 **Blockierung von Bugfix-Pipelines**, weil Ressourcen in die Analyse falscher Berichte fließen.
* 🔇 **Schwächung der Glaubwürdigkeit von KI-gestütztem Reporting**.

---

## 🛡️ Ursachen für Halluzinationen

* 📉 Fehlende Kontextkenntnis
* 🔄 Kein Zugriff auf den aktuellen Quellcode / Runtime-Daten
* 🗣️ Rein sprachstatistische Prognose ohne Rückkopplung durch "Wahrheitsprüfung"
* 🧠 Kein "Verständnis" im menschlichen Sinn – nur Wahrscheinlichkeitsketten

---

## ✅ Gegenmaßnahmen

| Maßnahme                | Beschreibung                                                         |
| ----------------------- | -------------------------------------------------------------------- |
| 🔐 Kontext-Pinning      | Eingabe von Codeauszügen oder genauen Logs als "verankerter Kontext" |
| 🧭 Validierungs-Prompts | Meta-Analyse der generierten Antwort vor Verwendung                  |
| ✍️ Manuelle Prüfung     | Der Mensch entscheidet, ob etwas plausibel und relevant ist          |
| 🧪 Testfall-Ergänzung   | Konkrete Beweise statt spekulativer Vermutungen                      |

---

## 🔚 Fazit

Halluzinationen gehören zu den größten Herausforderungen beim Einsatz von LLMs in technischen Kontexten. Wer mit KI arbeitet, trägt Verantwortung – nicht nur für den Nutzen, sondern auch für die Vermeidung von Schaden durch plausibel klingenden Unsinn.

> "Eine halluzinierende KI ist kein Werkzeug, sondern ein Risikofaktor – solange niemand kontrolliert, was sie sagt."
