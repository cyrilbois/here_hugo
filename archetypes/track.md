---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: Curated sounds 🧘‍♂️
tags: [music, track, curated]
---

{{<spotifyembed track id>}}