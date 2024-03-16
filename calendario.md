---
layout: page
title: Calendário
description: Listing of course modules and topics.
---

# Calendário

Calendário da disciplina com base na [[RESOLUÇÃO CEPE Nº 10/2023]](https://res.ufv.br/wp-content/uploads/2023/11/Resolucao-Cepe-no-10-2023.pdf):

<!-- {% for module in site.modules %}
{{ module }}
{% endfor %} -->

<table>
  <tr>
    <th>Semana</th>
    <th>Data</th>
    <th>Aula</th>
    <th>Leituras<br><a href="https://aima.cs.berkeley.edu/">(AIMA, 4th ed.)</a></th>
    <th>Projetos</th>
  </tr>

  <!-- Semana 1 -->
  <tr>
    <td rowspan="2">1</td>
    <td>05/03</td>
    <td>1. Introdução<br><a href="{{ 'assets/slides/A01-introducao.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 1, 2</td>
    <td></td>
  </tr>
  <tr>
    <td>07/03</td>
    <td>2. Busca no espaço de estados I<br><a href="{{ 'assets/slides/A02-buscaI.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 3.1-3.4</td>
    <td></td>
  </tr>

  <!-- Semana 2 -->
  <tr>
    <td rowspan="2">2</td>
    <td>12/03</td>
    <td>3. Busca no espaço de estados II<br><a href="{{ 'assets/slides/A03-buscaII.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 3.5-3.6</td>
    <td rowspan="4"><a href="{{ site.url }}/assignments/tp1-busca">TP1: Busca no espaço de estados</a></td>
  </tr>
  <tr>
    <td>14/03</td>
    <td>4. Busca local e otimização I: subida de encosta, têmpera simulada e busca em feixe</td>
    <td>Cap. 4.1</td>
  </tr>

  <!-- Semana 3 -->
  <tr>
    <td rowspan="2">3</td>
    <td>19/03</td>
    <td>5. Busca local e otimização II</td>
    <td>Cap. 4.2</td>
  </tr>
  <tr>
    <td>21/03</td>
    <td>6. Busca competitiva I: minimax, poda alpha-beta e funções de utilidade</td>
    <td>Cap. 5.1-5.3</td>
  </tr>

  <!-- Semana 5 -->
  <tr>
    <td rowspan="2">4</td>
    <td>26/03</td>
    <td>7. Busca competitiva II: busca em árvore monte carlo</td>
    <td>Cap. 5.4</td>
    <td rowspan="6">TP2: Busca local</td>
  </tr>
  <tr>
    <td>28/03</td>
    <td>8. Busca competitiva III: jogos estocásticos e parcialmente observáveis</td>
    <td>Cap. 5.5-5.6</td>
  </tr>

  <!-- Semana 6 -->
  <tr>
    <td rowspan="2">5</td>
    <td>02/04</td>
    <td>9. Satisfação de Restrição I</td>
    <td>Cap. 6.1-6.2</td>
  </tr>
  <tr>
    <td>04/04</td>
    <td>10. Satisfação de Restrição II</td>
    <td>Cap. 6.3-6.5</td>
  </tr>

  <!-- Semana 7 -->
  <tr>
    <td rowspan="2">6</td>
    <td>09/04</td>
    <td><b>Prova 1</b></td>
    <td></td>
  </tr>
  <tr>
    <td>11/04</td>
    <td>11. Agentes lógicos I: lógica proposicional</td>
    <td>Cap. 7.1-7.4</td>
  </tr>

  <!-- Semana 8 -->
  <tr>
    <td rowspan="2">7</td>
    <td>16/04</td>
    <td>12. Agentes lógicos II: inferência lógica, prova de teorema, satisfatibilidade booleana</td>
    <td>Cap. 7.5-7.7, 8.1-8.2</td>
    <td rowspan="2">R1: Identificação de problema</td>
  </tr>
  <tr>
    <td>18/04</td>
    <td>13. Agentes lógicos III: lógica de primeira ordem</td>
    <td>Cap 8.3-8.4</td>
  </tr>  

  <!-- Semana 9 -->
  <tr>
    <td rowspan="2">8</td>
    <td>23/04</td>
    <td>14. Raciocínio Probabilístico I: intro. à probabilidade</td>
    <td>Cap 12.1-12.5</td>
    <td rowspan="6">R2: Revisão da literatura</td>
  </tr>
  <tr>
    <td>25/04</td>
    <td>15. Raciocínio Probabilístico II: redes bayesianas</td>
    <td>Cap. 13.1-13.4</td>
  </tr>  

  <!-- Semana 10 -->
  <tr>
    <td rowspan="2">9</td>
    <td>30/04</td>
    <td>16. Raciocínio Probabilístico III: modelos de Markov</td>
    <td>Cap. 14.1-14.5</td>
  </tr>
  <tr>
    <td>02/05</td>
    <td>17. Processos de decisão de Markov II</td>
    <td>Cap. 17.3-17.4</td>
  </tr>  

  <!-- Semana 11 -->
  <tr>
    <td rowspan="2">10</td>
    <td>07/05</td>
    <td>18. Processos de decisão de Markov II</td>
    <td>Cap. 17.3-17.4</td>
  </tr>
  <tr>
    <td>09/05</td>
     <td>19. Aprendizado por Reforço I</td>
    <td>Cap. 22.1-22.4</td>
  </tr>  

  <!-- Semana 12 -->
  <tr>
    <td rowspan="2">11</td>
    <td>14/05</td>
    <td>20. Aprendizado por Reforço II</td>
    <td>Cap. 22.5-22.7</td>
    <td rowspan="5">TP3: Aprendizado por reforço</td>
  </tr>
  <tr>
    <td>16/05</td>
    <td><b>Prova 2</b></td>
    <td></td>
  </tr>  

  <!-- Semana 13 -->
  <tr>
    <td rowspan="2">12</td>
    <td>21/05</td>
    <td>21. Aprendizado de Máquina I: introdução e árvores de decisão</td>
    <td>Cap. 19.1-19.4</td>
  </tr>
  <tr>
    <td>23/05</td>
    <td>22. Aprendizado de Máquina II: regressão linear e logística</td>
    <td>Cap. 19.1-19.6</td>
  </tr>  

  <!-- Semana 14 -->
  <tr>
    <td rowspan="2">13</td>
    <td>28/05</td>
    <td>23. Aprendizado de Máquina III: kNN</td>
    <td>Cap. 19.7.1 - 19.7.4</td>
  </tr>
  <tr>
    <td>30/05</td>
    <td><b>Feriado (Corpus Christi)</b></td>
    <td></td>
    <td rowspan="4">TP4: Aprendizado de máquina</td>
  </tr>  

  <!-- Semana 15 -->
  <tr>
    <td rowspan="2">14</td>
    <td>04/06</td>
    <td>24. Aprendizado de Máquina IV: máquinas de vetores de suporte</td>
    <td>Cap. 19.7.5 - 19.7.6</td>
  </tr>
  <tr>
    <td>06/06</td>
    <td>25. Aprendizado de Máquina V: emsemble learning</td>
    <td>Cal. 19.8</td>
  </tr>  

  <!-- Semana 16 -->
  <tr>
    <td rowspan="2">15</td>
    <td>11/06</td>
    <td>26. Aprendizado de Máquina VI: Deep Learning I</td>
    <td>Cap.  21.1-21.2</td>
  </tr>
  <tr>
    <td>13/06</td>
    <td>27. Aprendizado de Máquina VII: Deep Learning II</td>
    <td>Cap. 21.3, 21.6</td>
    <td rowspan="2">R3: Metodologia de pesquisa</td>
  </tr>  

  <!-- Semana 17 -->
  <tr>
    <td rowspan="2">16</td>
    <td>18/06</td>
    <td>28. Aprendizado de Máquina VIII: Aprendizado não-supervisionado</td>
    <td>Cap. 21.7</td>
  </tr>
  <tr>
    <td>20/06</td>
    <td><b>Prova 3</b></td>
    <td></td>
    <td rowspan="3">R4: Introdução do projeto</td>
  </tr>  

  <!-- Semana 18 -->
  <tr>
    <td rowspan="2">17</td>
    <td>25/06</td>
    <td>29. Conclusão</td>
    <td></td>
  </tr>
  <tr>
    <td>27/06</td>
    <td><b>Apresentação dos Trabalhos</b></td>
    <td></td>
  </tr>  

</table>
