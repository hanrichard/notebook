### header
```
x-auth-token
```


```
Content-Type
```

cors header
```
app.use((req, res, next) => {
  res.setHeader('Access-Control-Allow-Origin', '*')
  res.setHeader('Access-Control-Allow-Methods', 'GET, POST, PUT, PATCH, DELETE')
  res.setHeader('Access-Control-Allow-Headers', 'Content-Type') 
})
```


```
router.get('/me', auth, async (req, res) => {
  try {
  
  } catch(err) {
    console.error(error);
    return res.status(500).json({ msg: 'Server error' });
  }
})

router.get('/', async (req, res) => {
  try {
  
  } catch(err) {
    console.error(error);
    return res.status(500).json({ msg: 'Server error' });
  }
})
```


### header response


### body parser
```
const bodypaser = require('body-parser')
app.use(bodypaser.urlencoded({extended:false}))
```

### common path
```
app.use("/admin", adminRoutes)
```

### sendfile
```
res.statusCode(200).sendFile(path.join(__dirname, "view", "index.html"))
```

### static serve
```
app.use(express.static(path.join(__dirname, "public"))
```

This route path will match acd and abcd.
```
app.get('/ab?cd', function (req, res) {
  res.send('ab?cd')
})
This route path will match abcd, abbcd, abbbcd, and so on.

app.get('/ab+cd', function (req, res) {
  res.send('ab+cd')
})
This route path will match abcd, abxcd, abRANDOMcd, ab123cd, and so on.

app.get('/ab*cd', function (req, res) {
  res.send('ab*cd')
})
This route path will match /abe and /abcde.

app.get('/ab(cd)?e', function (req, res) {
  res.send('ab(cd)?e')
})
```

```
const router = express.Router();
const { getblalb } = require('../blblbl')

router.route('/').get(getblablaba).post(addblblbl)

router.route('/:id').delete(deleteblablaba)
```

