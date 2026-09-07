---
version: alpha
name: "Donotr469 Genius Bar Guide"
description: "Apple-cinematic design system : noir cinématique, un seul accent bleu interactif, typographie SF serrée, surfaces glass discrètes."
colors:
  primary: "#000000"
  secondary: "#F5F5F7"
  tertiary: "#0071E3"
  neutral: "#1D1D1F"
  success: "#30D158"
  warning: "#FF9F0A"
typography:
  h1:
    fontFamily: SF Pro Display
    fontSize: 2.125rem
    fontWeight: 600
    lineHeight: "1.1"
    letterSpacing: "-0.02em"
  h2:
    fontFamily: SF Pro Display
    fontSize: 1.5rem
    fontWeight: 600
    lineHeight: "1.14"
    letterSpacing: "-0.011em"
  body:
    fontFamily: SF Pro Text
    fontSize: 0.9375rem
    fontWeight: 400
    lineHeight: "1.47"
    letterSpacing: "-0.012em"
  caption:
    fontFamily: SF Pro Text
    fontSize: 0.875rem
    fontWeight: 400
    lineHeight: "1.29"
    letterSpacing: "-0.014em"
rounded:
  sm: 8px
  md: 14px
  lg: 20px
  pill: 980px
spacing:
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
components:
  card:
    backgroundColor: "rgba(255,255,255,0.055)"
    textColor: "#F5F5F7"
    rounded: "{rounded.lg}"
    padding: 32px
  cta-primary:
    backgroundColor: "{colors.tertiary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.sm}"
    padding: 12px
  pill-label:
    backgroundColor: "rgba(255,255,255,0.10)"
    textColor: "rgba(245,245,247,0.72)"
    rounded: "{rounded.pill}"
    padding: 8px
  verdict-green:
    backgroundColor: "rgba(48,209,88,0.10)"
    textColor: "#F5F5F7"
    rounded: "{rounded.md}"
    padding: 16px
---

## Overview

Système « Apple cinématique » adapté aux outils Genius Bar : fond noir profond, sections en surfaces glass discrètes, UN seul accent interactif (Apple Blue #0071E3) réservé aux éléments cliquables. Les couleurs vert/violet/orange sont strictement sémantiques (verdicts éligible/partiel, catégories de puces) — jamais décoratives.

## Colors

- **Primary (#000000) :** noir pur pour l'immersion, fond par défaut du site.
- **Secondary (#F5F5F7) :** le gris Apple — texte principal sur noir, fond en mode light.
- **Tertiary (#0071E3) :** Apple Blue — réservé aux interactions (boutons, sélection quiz, focus).
- **Semantic :** green (#30D158) = verdict favorable ; orange (#FF9F0A) = attention ; purple (#BF5AF2) = catégorie puces Pro.

## Typography

SF Pro (fallback system-ui). Display 600 pour les titres avec tracking -0.02em et lh 1.07-1.14 ; corps 400 en lh 1.47 avec tracking -0.012em universel (philosophie Apple du tracking négatif à toutes tailles).

## Components

`card` = surface glass unique (blur 20px, saturate 180%) ; élévation par surface, pas par ombres multiples. `cta-primary` = le seul bouton à fort contraste. Focus ring 2px #0071E3 sur tous les éléments interactifs (WCAG 2.4.7).

## Do's and Don'ts

- Ne jamais introduire d'autre accent interactif que le bleu Apple.
- Pas de bordures voyantes : les frontières sont des surfaces (`hair-soft`).
- Rayons : 8px (contrôles), 14-20px (cartes), 980px (pills) — pas au-delà.
- Tracking négatif à toutes les tailles ; jamais de lh < 1.07 en display ni > 1.6 en corps.
