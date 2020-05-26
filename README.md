# Things

### select points from GeoJson
```
jq -r '.features[] | select(.geometry.type == "Point") | "\(.properties.Name), \(.geometry.coordinates[0]), \(.geometry.coordinates[1])"' geo.json

Some place, 35.2972888972788, 30.8024146526215
...

```
