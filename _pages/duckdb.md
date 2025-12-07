---
title: Expériences avec R/DuckDB
layout: single
permalink: /duckdb/
classes: wide
---

Lors de mon passage à la Dares (2023-2025), j'ai travaillé sur les données du SI Agora sur la formation professionnelle en France. 
Ce sont des données volumineuses, qui dépassent la mémoire vive d'un poste de travail standard.
(~ 100-800 millions de lignes pour certaines tables).

Pour pouvoir analyser ces données sur un ordinateur portable, il faut parfois ruser. 
Sur cette page, je rassemble quelques travaux de comparaison entre solutions techniques. 
Ceci permet d'apporter des éléments de justification pour des recommandations d'usage de R/DuckDB (sous Windows).

(Work in progress)

[ParquetCompression.html]({% link /duckdb_html/ParquetCompression.html %})

Est-ce que DuckDB optimise automatiquement ? 

- éviter un calcul quand la colonne n'est pas sélectionnée : [oui]({% link /duckdb_html/20240610_BenchmarkMutateSelect.html %})







