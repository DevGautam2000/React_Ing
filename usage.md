# Usage

inside a react project

### to generate components (.js and .css)

into the root of the react project

```bash
    ing g -c <replace-with-component-name>

    e.g,
    ing g -c mycomponent
```

this generates Mycomponent.js into src/components
and mycomponent.css into src/css

### to generate components (.js and .module.css)

```bash
    ing g -c <replace-with-component-name> -m

    e.g,
    ing g -c mycomponent -m
```

this generates Mycomponent.js into src/components
and mycomponent.module.css into src/css

## both commands above will create a Mycomponent.js file with this boiler plate

### with -m flag for css module files

```javascript
import React from "react";
import style from "../css/mycomponent.module.css";

function Mycomponent() {
  return <div className={style.mycomponent}>mycomponent works!</div>;
}

export default Mycomponent;
```

### without -m flag

```javascript
import React from "react";
import "../css/mycomponent.css";

function Mycomponent() {
  return <div className="mycomponent__main">mycomponent works!</div>;
}

export default Mycomponent;
```

## to omit the boiler plate from being generated

### add -o flag at end

```bash
    ing g -c <component-name> -o        //for normal css files

     e.g., ing g -c component -o
```

```bash
    ing -c <component-name> -m -o     //for css module files

    e.g., ing g -c component -m -o
```

## to generate a style sheet only (.css)

### for css module file

```bash
    ing g -s <name> -m

    e.g., ing g -s home -m
```

### for normal css file

```bash
    ing g -s <name>

     e.g., ing g -s home
```

## to generate a screen with boiler plate(.js in src/screens)

```bash
    ing g -sc <screen-name>

    e.g., ing g -sc home
```

##### for generating screens/pages use -sc or -p flag follwed by name

## to generate a custom file in a custom directory (into src/)

```bash
    ing g <path-to-dir> <file-name-with-extension>

    e.g., ing g one/two/three numbers.js
```

## 🔗 Links

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://inginer.me/)

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gautam-chandra-saha-896735205/)

[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/gautam1200)

## Authors

- [@devgautam2000](https://www.github.com/devgautam2000)

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Support

For support, email devgautam1231@icloud.com or create an issue.
