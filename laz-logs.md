---
description: standalone system to create logs on our server
---

# Laz-logs

{% tabs %}
{% tab title="client" %}
```lua
TriggerServerEvent('Laz-Logs:LogFields',typewebhook, title, Description, color, footer, field, id)
```
{% endtab %}

{% tab title="Server" %}
```lua
TriggerEvent('Laz-Logs:LogFields',typewebhook, title, Description, color, footer, field, id)
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
## Desactive description

* ```lua
  TriggerServerEvent('Laz-Logs:LogFields',typewebhook, title, false, color, footer, field, id)
  ```
{% endhint %}

