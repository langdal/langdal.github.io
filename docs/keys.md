---
title: Keys
layout: default
---

# Public keys

{% for key in site.data.keys %}

### {{ key.name }}
{% if key.gpg.enabled %}
- Public GPG key [[{{key.gpg.idlong}}]]({{key.gpg.link}}) {{key.gpg.fingerprint}}
{% endif %}
{% if key.ssh.enabled %}
- Public SSH key

```
{{key.ssh.pubkey}}

```
{% endif %}

{% endfor %}

[back](./)
