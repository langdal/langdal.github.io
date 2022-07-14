---
title: Keys
layout: default
---

# Public keys

{% for key in site.data.keys %}

### {{ key.name }}

- Public GPG key [[{{key.gpg.idlong}}]]({{key.gpg.link}})
- Public SSH key

```
{{key.ssh.pubkey}}

```

{% endfor %}

[back](./)
