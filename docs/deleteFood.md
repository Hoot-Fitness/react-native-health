# deleteFood

Delete a food entry from HealthKit.

`deleteFood` accepts a record's UUID string and a callback:

Example input object:

```javascript
let id = "ba13089a-a311-4ffe-9352-f5c568936f16"
```

Example usage:

```javascript
AppleHealthKit.deleteFood(
  id,
  (err: Object, result: number) => {
    if (err) {
      return
    }
    // food successfully deleted
    console.log(result)
  },
)
```

Example output (1 if deleted):

```json
1
```

