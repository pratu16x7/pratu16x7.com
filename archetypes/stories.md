---
title: "{{ replace .Name "-" " " | title }}"
subtitle: ""
date: {{ .Date }}
color: "{{ index (shuffle (slice "" "yellow" "brown" "sepia" "green")) 0 }}"
draft: true
---
