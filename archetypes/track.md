---
title: "Track: {{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: Curated sounds 🧘‍♂️
tags: [music, track, curated]
images: ['https://images-here-hugo.vercel.app/api/og-image?title={{ urlquery (replace .Name "-" " " | title) }}']
---

{{<spotify track id>}}
