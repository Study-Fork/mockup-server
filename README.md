# Mock Server 

![mock-manual](https://github.com/joon610/readMEImg/blob/master/mock-server/mock-manual.gif)

## Translate
한국어 : <https://joon610.github.io/sideproject/MockUp-Server> <br> 
日本語 : <https://qiita.com/joon610/items/f5aae93815b536a3f56b>

## Usage
- [`Initialize Setting`](#initialize)   
- [`set Header and Cookies`](#headerSetting)    
- [`CRUD`](#crud)   

## <a id="initialize"></a> initialize Setting
<img src="https://joon610.github.io/assets/images/mockupServer/graph.png" alt="graph">

1. created directory.
2. make Json files, index.json(successe case),error.json(error case),header.json(api Header, set Cookie)
3. Mockup Server start! 


## <a id="headerSetting"></a> Set Header and Cookies  (header.Json)
```js
{  //example add header.json in your directory
    "header": {
        "Content-Type": "application/json; charset=utf-8"
    },
    "cookies": [
        {
            "name": "fff",
            "value": "cookieValue",
            "options": {
                "maxAge": 30000
            }
        },
        {
            ...
        }
    ]
}
```

## <a id="crud"></a>CRUD (Create, Read, Update ,Delete)
``` Json
// index.json
[
  {
        "id": "1",   // id is key
        "name": "Sara",
        "age": "13"
    },
    {
        "id": "2",
        "name": "teddy",
        "age": "14"
    }   
]
```

### Create (POST)    
<img src="https://joon610.github.io/assets/images/mockupServer/post.png" alt="post">


### Read (GET)
<img src="https://joon610.github.io/assets/images/mockupServer/get_all.png" alt="get_all">
<img src="https://joon610.github.io/assets/images/mockupServer/get_1.png" alt="get_1">

### Update
<img src="https://joon610.github.io/assets/images/mockupServer/put.png" alt="put">

### Delete
<img src="https://joon610.github.io/assets/images/mockupServer/delete.png" alt="delete">

### DownLoad
- Mac : 
  - <https://github.com/joon610/mockup-server/releases/download/v0.2.1/mockup-server-0.2.1.dmg>

- Windows :
  - <https://github.com/joon610/mockup-server/releases/download/v0.2.1/mockup-server.Setup.0.2.1.exe>

## TodoList 
- [X] allow cross origin option
- [X] add header and cookie  
- [ ] Dynamic key name 
- [ ] Each api description

## License
MIT License

## Project setupø
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn dev
```

### Compiles and minifies for production(electront)
```
build:electron
```

