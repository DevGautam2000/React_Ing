# React-Ing

A cli for react projects to generate folder structures

- [Installation](https://github.com/DevGautam2000/React_Ing/blob/master/installation.md)
- [Usage](https://github.com/DevGautam2000/React_Ing/blob/master/usage.md)

## Examples

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
  return <div className={style.mycomponent}>
  
  mycomponent works!
  </div>;
}

export default Mycomponent;
```

### without -m flag

```javascript
import React from "react";
import "../css/mycomponent.css";

function Mycomponent() {
  return <div className="mycomponent__main">
  
  mycomponent works!
  </div>;
}

export default Mycomponent;
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

#### Note

- The code is open source so do not hesitate to make it better
- Thank you and keep coding!
