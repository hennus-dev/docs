# Laz-target



{% hint style="info" %}
Intentaremos mantener la documentación al día con cada actualización de los scripts.
{% endhint %}

## Exportaciones

Está previsto que la información se facilite a través de las siguientes exportaciones

{% tabs %}
{% tab title="addPed" %}
```lua
exports['Laz-target']:addPed('model', 'anim',coords)
# ejemplo
exports['Laz-target']:addPed('a_f_y_bevhills_04', 'anim', vector4(100.35, -1077.02, 28.21, 239.06)
```
{% endtab %}

{% tab title="addObject" %}
```lua
exports['Laz-target']:addObject('model',coords)
# ejemplo

exports['Laz-target']:addObject('model',coords)

```
{% endtab %}

{% tab title="AddTargetPeds" %}
```lua
exports[''Laz-target']:addTargetPeds(name , model, distance,  options, BlackList, WhiteList)
# ejemplo
  exports['Laz-target']:AddTargetPeds('Laz-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'Laz-carinsurance:open',
                key = 'Laz-carinsurance:open',
                label = 'Open'
            }
        },
        false,
        {    coords = {
                pos = vector3(100.35, -1077.02, 29.21),
                radius = 2.0
            }
        }
    )
```
{% endtab %}

{% tab title="AddTargetObjects" %}
```lua
exports[''Laz-target']:AddTargetObjects(name , model, distance,  options, BlackList, WhiteList)
# ejemplo
  exports['Laz-target']:AddTargetObjects('Laz-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'Laz-carinsurance:open',
                key = 'Laz-carinsurance:open',
                label = 'Open'
            }
        },
        false,
        {    coords = {
                pos = vector3(100.35, -1077.02, 29.21),
                radius = 2.0
            }
        }
    )
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
Se pueden actualizar las exportaciones. Todavía es una beta.
{% endhint %}
