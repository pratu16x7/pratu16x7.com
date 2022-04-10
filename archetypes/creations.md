---
title: "{{ replace .Name "-" " " | title }}"
description: ""
date: {{ .Date }}
color: "{{ index (shuffle (slice "" "yellow" "brown" "sepia" "green")) 0 }}"
draft: false
---
