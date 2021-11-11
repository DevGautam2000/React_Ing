# Usage

inside a react project

### to generate all files (.js and .css)

into the root of the react project

```bash
    ing gen -a <replace-with-component-name>

    e.g,
    ing gen -a mycomponent
```

this generates Mycomponent.js into src/components
and mycomponent.css into src/css

### to generate all files (.js and .module.css)

```bash
    ing gen -a <replace-with-component-name> -m

    e.g,
    ing gen -a mycomponent -m
```

this generates Mycomponent.js into src/components
and mycomponent.module.css into src/css

## both commands above will create a Mycomponent.js file with this boiler plate

### with -m flag for css module files

```javascript
import React from "react";
import style from "../css/mycomponent.module.css";

function Mycomponent() {
  return <div className={style.mycomponent}></div>;
}

export default Mycomponent;
```

### without -m flag

```javascript
import React from "react";
import "../css/mycomponent.css";

function Mycomponent() {
  return <div className="mycomponent__main"></div>;
}

export default Mycomponent;
```

## to omit the boiler plate from being generated

### add -o flag at end

```bash
    ing gen -a <component-name> -o        //for normal css files

     e.g., ing gen -a component -o
```

```bash
    ing -a <component-name> -m -o     //for css module files

    e.g., ing gen -a component -m -o
```

## to generate a component file only (.js)

```bash
    ing gen -c <component-name>

    e.g., ing gen -c component
```

## to generate a style sheet only (.css)

### for css module file

```bash
    ing gen -s <name> -m

    e.g., ing gen -s home -m
```

### for normal css file

```bash
    ing gen -s <name>

     e.g., ing gen -s home
```

## to generate a screen only (.js in src/screens)

```bash
    ing gen -scr <screen-name>

    e.g., ing gen -scr home
```

## to generate a custom file in a custom directory (into src/)

```bash
    ing gen <path-to-dir> <file-name-with-extension>

    e.g., ing gen one/two/three numbers.js
```

## Authors

- [@devgautam2000](https://www.github.com/devgautam2000)

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Support

For support, email devgautam1231@icloud.com or create an issue.
