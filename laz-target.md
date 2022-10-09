# Laz-target

{% hint style="info" %}
We will try to keep the documentation up to date with each update of each script.tion!
{% endhint %}

## exports

It is planned to give you the information through the following exports

{% tabs %}
{% tab title="addPed" %}
```lua
exports['Laz-target']:addPed('model', 'anim',coords)
# Example
exports['Laz-target']:addPed('a_f_y_bevhills_04', 'anim', vector4(100.35, -1077.02, 28.21, 239.06)
```
{% endtab %}

{% tab title="addObject" %}
```lua
exports['Laz-target']:addObject('model',coords)
# Example

exports['Laz-target']:addObject('model',coords)

```
{% endtab %}

{% tab title="AddTargetPeds" %}
```lua
exports[''Laz-target']:addTargetPeds(name , model, distance,  options, BlackList, WhiteList)
# example 
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
# example 
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

{% hint style="info" %}
these exports can be updated. it's still a beta.
{% endhint %}
