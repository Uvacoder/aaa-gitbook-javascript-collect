# Parcel

|  |  |
| :--- | :--- |
| [https://parceljs.org/](https://parceljs.org/) | 3/2 |

```text
npm init
```

{% code title="install parcel" %}
```bash
##yarn
yarn global add parcel-bundler
##local
yarn install parcen-bundler --save-dev

##npm
npm i -g parcel-bundler
##local
npm i parcel-bundler --D
```
{% endcode %}

{% code title="using parcel" %}
```bash
npm start     ##start = variable name in package.json under script:
npm run build ##build = var name 
```
{% endcode %}

{% code title="package.json" %}
```bash
{
  "scripts": {
    "start": "parcel index.html",
    "build": "parcel build index.html"
  }
}
```
{% endcode %}

### Debugging

delete `cache` and `dist` folders and rerun `npm start`

