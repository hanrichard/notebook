### lambda event
```
event: input data or input parameters
based on event source
```

### lambda context
```
it's method and property
- context.functionVersion
- context.functionArn
- context.identity
```

### lambda common pattern

```
let userid = event.pathParameters.userid
```

### put 
```
let data = await dynamodb.put({
  TableName: tablename,
  Item: item
}).promose()
```

### get
```
let data = await dynamodb.get({
  TableName: tablename,
  key: {
    userid: userid
  }
}).promose()
```
### delete
```
let data = await dynamodb.delete({
  TableName: tablename,
  key: {
    userid: userid
  }
}).promose()

```

### JSON
```
let {a, b} = JSON.parse(event.body)

JSON.stringify({
  a: a,
  b: b
})
```
