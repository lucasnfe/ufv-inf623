---
layout: home
title: INF623 - Inteligência Artificial
nav_exclude: true
permalink: /:path/
seo:
  type: Course
  name: INF623 - Inteligência Artificial 
---

# INF623 - Inteligência Artificial

Esta disciplina apresenta as técnicas fundamentais para o projeto de sistemas computacionais inteligentes, incluindo resolução de problemas por meio busca, representação do conhecimento, raciocínio probabilístico e aprendizado de máquina. As técnicas discutidas neste curso aplicam-se a uma ampla variedade de problemas e servem de base para estudos posteriores em qualquer subárea da Inteligência Artificial.

## Avisos Recentes

{% assign announcements = site.announcements %}
{{ announcements.last }}

## Ensalamento

- Aulas: Terças e Quintas: 14:00-15:40h, CCE408
- Atendimendo: Terças e Quintas: 16:00-17:00h, CCE401B

## Professor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}
