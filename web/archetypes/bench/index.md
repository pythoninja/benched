{{- $rawName := split .Name "_" -}}
{{- $providerName := index $rawName 0 -}}
{{- $hostName := index $rawName 1 -}}
{{- $benchNumber := index $rawName 2 -}}
{{- $downloadFileName := printf "%s-bench-%s.txt" $hostName $benchNumber -}}

---
title: "{{ $providerName | title }} ({{ $hostName }}) Benchmark #{{ $benchNumber }}"
date: {{ .Date }}
lastmod: {{ .Date }}
tags:
    - yabs
    - {{ $providerName }}
    - {{ $hostName }}

draft: true
---

## Yabs Output

```text
yabs output
```

Download metrics as text: [yabs.txt](./yabs.txt)

Download as text: [{{ $downloadFileName }}](https://dl.benched.cc/yabs-archive/{{ $providerName }}/{{ $downloadFileName }})
