Bootstrap v4 has seperated the grid system as independent file - ```bootstrap-grid.css```
But the default grid file doesn't include the flex system
We need to create flex grid by ourselves

## How
1. Download bootstrap and npm install its dependencies
2. create a file and put the following code

```scss
@import 'bootstrap-grid.scss';
@import 'utilities/_flex.scss';

```
3. revise ```package.json``` by adding our created file for latter compiling
```json
scripts: {
   'npm run sass': ...  //add our created scss file
   'npm run clean-css': ... //add ourt created css file
}
```

4. run ```npm run sass``` and ```npm run clean-css```
