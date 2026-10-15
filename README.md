<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,60:6e40c9,100:a371f7&height=190&section=header&text=Erich%20Valarini&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Full%20Stack%20Developer&descAlignY=57&descSize=16" width="100%"/>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1000&color=A371F7&center=true&vCenter=true&width=520&lines=%24+node+server.js;GET+%2Fsobre+%E2%86%92+200+OK;Veni%2C+vidi%2C+vici." alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/runtime-node.js-a371f7?style=for-the-badge&logo=nodedotjs&logoColor=white&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/framework-express-ffffff?style=for-the-badge&logo=express&logoColor=white&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/status-online-a371f7?style=for-the-badge&labelColor=0d1117" />
  <img src="https://komarev.com/ghpvc/?username=Erich-z&style=for-the-badge&color=6e40c9&label=requests" />
</p>

<br/>

```js
// 📁 server.js
const express = require('express');
const app = express();

app.get('/sobre', (req, res) => {
  res.json({
    nome: 'Erich Valarini',
    cargo: 'Desenvolvedor Full Stack',
    formacao: 'Análise e Desenvolvimento de Sistemas',
    curte: ['código limpo', 'lógica bem estruturada', 'sistemas organizados'],
  });
});

app.get('/stack', (req, res) => {
  res.json({
    linguagens: ['JavaScript', 'TypeScript'],
    back: ['Node.js', 'Express'],
    front: ['React', 'HTML', 'CSS'],
    ferramentas: ['Git'],
  });
});

app.get('/evoluindo', (req, res) => {
  res.json([
    'JavaScript & TypeScript',
    'Node.js + Express',
    'APIs REST',
    'Boas práticas e arquitetura',
  ]);
});

app.use((req, res) => res.status(404).send('Veni, vidi, vici.'));

app.listen(3000);
```



```diff
+ $ node server.js
+ GET /sobre      200 OK
+ GET /stack      200 OK
+ GET /evoluindo  200 OK
```

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:a371f7,40:6e40c9,100:0d1117&height=100&section=footer" width="100%"/>
