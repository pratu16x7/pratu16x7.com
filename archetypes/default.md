---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
color: "{{ index (shuffle (slice "" "yellow" "brown" "sepia" "green")) 0 }}"
draft: true
---
