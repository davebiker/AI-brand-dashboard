# Škoda X — AI Brand Visibility Dashboard

Real-time monitoring dashboard pro sledování viditelnosti značky Škoda v odpovědích AI platforem (Claude, GPT-4o, Gemini).

![Škoda CI](https://img.shields.io/badge/Škoda_CI-Emerald_%230E3A2F-0E3A2F) ![Electric Green](https://img.shields.io/badge/Electric_%2378FAAE-78FAAE)

## 🖥️ Zobrazení

| Režim | URL | Použití |
|-------|-----|---------|
| **Preview** | `index.html` | Desktop s přepínačem TV/panel |
| **TV fullscreen** | `index.html#tv` | Firemní LED TV (16:9) |
| **Vertikální panel** | `index.html#vertical` | LED panel 50×180cm |
| **Mobil** | `index.html` | Automaticky při šířce <768px |

## 🚀 Nasazení

Běží na GitHub Pages jako statický HTML — žádný build, žádné závislosti.

**Live URL:** [https://davebiker.github.io/AI-brand-dashboard/](https://davebiker.github.io/AI-brand-dashboard/)

## ⚙️ Konfigurace

Vše se edituje přímo v `index.html` v sekci `KONFIGURACE` na začátku scriptu:

### Přidat dotaz
```js
// Najdi příslušnou kategorii v QUERY_CATEGORIES a přidej řádek:
"Tvůj nový dotaz zde",
```

### Přidat kategorii
```js
{
  category: "Název nové kategorie",
  queries: [
    "Dotaz 1",
    "Dotaz 2",
  ],
},
```

### Přidat platformu
```js
// V poli PLATFORMS odkomentuj nebo přidej:
{ name: "Perplexity", color: "#B4A0FF" },
```

### Přidat konkurenta
```js
// V poli COMPETITORS přidej:
"BYD", "Dacia", "Volvo",
```

### Změnit rychlost aktualizace
```js
const UPDATE_INTERVAL = 4000; // ms — změň dle potřeby
```

## 📊 Aktuální stav

**Mockup verze** — data jsou simulovaná (random). Pro napojení na reálná API (Anthropic, OpenAI, Google) je potřeba backend.

## 🎨 Design

- Škoda CI: **Emerald Green** `#0E3A2F` + **Electric Green** `#78FAAE`
- Fonty: Outfit (UI) + JetBrains Mono (data)
- Dark theme optimalizované pro LED displeje

---

Škoda X — AI Brand Intelligence
