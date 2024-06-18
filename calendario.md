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
    <td>Caps. 1 e 2</td>
    <td></td>
  </tr>
  <tr>
    <td>07/03</td>
    <td>2. Busca no espaço de estados I<br><a href="{{ 'assets/slides/A02-busca-estados1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 3.1-3.4.3</td>
    <td></td>
  </tr>

  <!-- Semana 2 -->
  <tr>
    <td rowspan="2">2</td>
    <td>12/03</td>
    <td>3. Busca no espaço de estados II<br><a href="{{ 'assets/slides/A03-busca-estados2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 3.5-3.5.4</td>
    <td rowspan="5"><a href="{{ site.url }}/assignments/tp1-busca">TP1: Busca no espaço de estados</a></td>
  </tr>
  <tr>
    <td>14/03</td>
    <td>4. Busca local e otimização I<br><a href="{{ 'assets/slides/A04-busca-local1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 4.1-4.1.3</td>
  </tr>

  <!-- Semana 3 -->
  <tr>
    <td rowspan="2">3</td>
    <td>19/03</td>
    <td>5. Busca local e otimização II<br><a href="{{ 'assets/slides/A05-busca-local2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 4.1.4</td>
  </tr>
  <tr>
    <td>21/03</td>
    <td>6. Busca competitiva I<br><a href="{{ 'assets/slides/A06-busca-adversarial1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 5.1-5.3</td>
  </tr>

  <!-- Semana 5 -->
  <tr>
    <td rowspan="2">4</td>
    <td>26/03</td>
    <td>7. Busca competitiva II<br><a href="{{ 'assets/slides/A07-busca-adversarial2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 5.5</td>
  </tr>
  <tr>
    <td>28/03</td>
    <td><b>Feriado (Semana Santa)</b></td>
    <td></td>
    <td></td>
  </tr>

  <!-- Semana 6 -->
  <tr>
    <td rowspan="2">5</td>
    <td>02/04</td>
    <td>8. Busca competitiva III<br><a href="{{ 'assets/slides/A08-busca-adversarial3.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 5.4</td>
    <td></td>
  </tr>
  <tr>
    <td>04/04</td>
    <td>9. Satisfação de restrição I<br><a href="{{ 'assets/slides/A09-csp1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 6.1</td>
    <td></td>
  </tr>

  <!-- Semana 7 -->
  <tr>
    <td rowspan="2">6</td>
    <td>09/04</td>
    <td>10. Satisfação de restrição II<br><a href="{{ 'assets/slides/A10-csp2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 6.2-6.3</td>
    <td rowspan="6"><a href="{{ site.url }}/assignments/tp2-busca-local">TP2: Busca local</a></td>
  </tr>
  <tr>
    <td>11/04</td>
    <td><b>Prova 1</b></td>
    <td><a href="{{ 'assets/homework/lista1.pdf' | relative_url }}">[Lista 1]</a></td>
  </tr>

  <!-- Semana 8 -->
  <tr>
    <td rowspan="2">7</td>
    <td>16/04</td>
    <td>11. Representação do conhecimento I<br><a href="{{ 'assets/slides/A11-conhecimento1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 7.1-7.4</td>
  </tr>
  <tr>
    <td>18/04</td>
    <td>12. Representação do conhecimento II<br>
      <a href="{{ 'assets/slides/A12-conhecimento2.pdf' | relative_url }}">[slides]</a>
      <a href="{{ 'assets/code/A12-conhecimento.zip' | relative_url }}">[código]</a>
    </td>
    <td>Cap. 7.7</td>
  </tr>  

  <!-- Semana 9 -->
  <tr>
    <td rowspan="2">8</td>
    <td>23/04</td>
    <td>13. Representação do conhecimento III<br><a href="{{ 'assets/slides/A13-conhecimento3.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap 7.5</td>
  </tr>
  <tr>
    <td>25/04</td>
    <td>14. Raciocínio probabilístico I<br><a href="{{ 'assets/slides/A14-incerteza1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap 12.1-12.5</td>  
  </tr>  

  <!-- Semana 10 -->
  <tr>
    <td rowspan="2">9</td>
    <td>30/04</td>
    <td>15. Raciocínio probabilístico II<br><a href="{{ 'assets/slides/A15-incerteza2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 13.1-13.4</td>
    <td rowspan="2"><a href="{{ site.url }}/assignments/r1-problema">R1: Identificação de problema</a></td>
  </tr>
  <tr>
    <td>02/05</td>
    <td>16. Raciocínio probabilístico III<br><a href="{{ 'assets/slides/A16-incerteza3.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 14.1-14.5</td>
  </tr>  

  <!-- Semana 11 -->
  <tr>
    <td rowspan="2">10</td>
    <td>07/05</td>
    <td>17. Raciocínio probabilístico IV<br><a href="{{ 'assets/slides/A17-incerteza4.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 17.3-17.4</td>
    <td rowspan="10"><a href="{{ site.url }}/assignments/r2-revisao">R2: Revisão da literatura</a></td>
  </tr>
  <tr>
    <td>09/05</td>
    <td>18. Processos de decisão de Markov I<br><a href="{{ 'assets/slides/A18-mdp1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 17.3-17.4</td>
  </tr>  

  <!-- Semana 12 -->
  <tr>
    <td rowspan="2">11</td>
    <td>14/05</td>
    <td>19. Processos de decisão de Markov II<br><a href="{{ 'assets/slides/A19-mdp2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 22.1-22.4</td>
  </tr>
  <tr>
    <td>16/05</td>
    <td>20. Processos de decisão de Markov III<br><a href="{{ 'assets/slides/A20-mdp3.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 22.5-22.7</td>
  </tr>  

  <!-- Semana 13 -->
  <tr>
    <td rowspan="2">12</td>
    <td>21/05</td>
    <td><b>Prova 2</b></td>
    <td><a href="{{ 'assets/homework/lista2.pdf' | relative_url }}">[Lista 2]</a></td>
  </tr>
  <tr>
    <td>23/05</td>
    <td>21. Aprendizado por reforço I<br><a href="{{ 'assets/slides/A21-rl1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 19.1-19.4</td> 
  </tr>  

  <!-- Semana 14 -->
  <tr>
    <td rowspan="2">13</td>
    <td>28/05</td>
    <td>22. Aprendizado por reforço II<br><a href="{{ 'assets/slides/A22-rl2.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 19.1-19.6</td>
  </tr>
  <tr>
    <td>30/05</td>
    <td><b>Feriado (Corpus Christi)</b></td>
    <td></td>
  </tr>  

  <!-- Semana 15 -->
  <tr>
    <td rowspan="2">14</td>
    <td>04/06</td>
    <td>23. Aprendizado por reforço III<br><a href="{{ 'assets/slides/A23-rl3.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 19.7.1 - 19.7.4</td>
  </tr>
  <tr>
    <td>06/06</td>
    <td>24. Aprendizado supervisionado I<br><a href="{{ 'assets/slides/A24-ml1.pdf' | relative_url }}">[slides]</a></td>
    <td>Cap. 19.7.5 - 19.7.6</td>
  </tr>  

  <!-- Semana 16 -->
  <tr>
    <td rowspan="2">15</td>
    <td>11/06</td>
    <td>25. Aprendizado supervisionado II<br><a href="{{ 'assets/slides/A25-ml2.pdf' | relative_url }}">[slides]</a><a href="{{ 'https://colab.research.google.com/drive/1EDFQ4FTYVTx2XW4iz6FHcO_GCYy2aoUg?usp=sharing' | relative_url }}">[colab]</a></td>
    <td>Cal. 19.8</td>
    <td rowspan="4"><a href="{{ site.url }}/assignments/tp3-aprendizado-reforco">TP3: Aprendizado por reforço</a></td>
  </tr>
  <tr>
    <td>13/06</td>
    <td>26. Aprendizado supervisionado III<br><a href="{{ 'assets/slides/A26-ml3.pdf' | relative_url }}">[slides]</a><a href="{{ 'https://colab.research.google.com/drive/1Osf18leU7bW0lCDUfyPTqy3Xr_68iviV?usp=sharing' | relative_url }}">[colab 1]</a><a href="{{ 'https://colab.research.google.com/drive/1hC680xDkpO34eXwkhC9xtumpvRozKiiz?usp=sharing' | relative_url }}">[colab 2]</a></td>
    <td>Cap.  21.1-21.2</td>
  </tr>  

  <!-- Semana 17 -->
  <tr>
    <td rowspan="2">16</td>
    <td>18/06</td>
    <td>27. Aprendizado supervisionado IV</td>
    <td>Cap. 21.3, 21.6</td>
  </tr>
  <tr>
    <td>20/06</td>
    <td>28. Aprendizado supervisionado V</td>
    <td>Cap. 21.7</td>
  </tr>  

  <!-- Semana 18 -->
  <tr>
    <td rowspan="2">17</td>
    <td>25/06</td>
    <td>29. Aprendizado supervisionado VI</td>
    <td>Cap. 21.9</td>
    <td rowspan="2">R3: Proposta de metodologia</td>
  </tr>
  <tr>
    <td>27/06</td>
    <td><b>Apresentação dos Trabalhos</b></td>
    <td></td>
  </tr>  

</table>
