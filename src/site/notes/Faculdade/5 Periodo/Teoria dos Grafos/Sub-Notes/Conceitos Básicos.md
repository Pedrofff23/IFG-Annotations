---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos/","tags":["grafos"]}
---

### Tópicos
1. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Definições e Exemplos\|Definições e Exemplos]]
	1. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Arestas\|Arestas]]
	2. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Graus\|Graus]]
		1. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Definição de grau\|Definição de grau]]
		2. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Grau de Entrada ou Saída\|Grau de Entrada ou Saída]]
		3. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Soma dos graus\|Soma dos graus]]
	3. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Ordem, Tamanho e Rótulo\|Ordem, Tamanho e Rótulo]]
	4. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Direcionado ou Orientado\|Direcionado ou Orientado]]
2. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Teoremas\|Teoremas]]
	1. [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos#Teorema 1\|Teorema 1]]
---
- **Notações**:
	- *G*: Grafo com conjunto de vértices V(G) e conjunto de arestas E(G).
	- *n*: Número de vértices de G.
	- *m*: Número de arestas de G.

## Definições e Exemplos
### Arestas
- **Incidentes**: Os extremos de uma aresta são ditos incidentes com a aresta
- **Adjacentes**: Dois vértices que são incidentes a uma mesma aresta são ditos adjacentes.
<style> .container {font-family: sans-serif; text-align: center;} .button-wrapper button {z-index: 1;height: 40px; width: 100px; margin: 10px;padding: 5px;} .excalidraw .App-menu_top .buttonList { display: flex;} .excalidraw-wrapper { height: 800px; margin: 50px; position: relative;} :root[dir="ltr"] .excalidraw .layer-ui__wrapper .zen-mode-transition.App-menu_bottom--transition-left {transform: none;} </style><script src="https://cdn.jsdelivr.net/npm/react@17/umd/react.production.min.js"></script><script src="https://cdn.jsdelivr.net/npm/react-dom@17/umd/react-dom.production.min.js"></script><script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@excalidraw/excalidraw@0/dist/excalidraw.production.min.js"></script><div id="Drawing_2024-03-17_1752.11.excalidraw.md1"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.0.25","elements":[{"type":"ellipse","version":227,"versionNonce":769668834,"isDeleted":false,"id":"m__w-3O2se0RxAF6xNKwY","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-225.83984593288878,"y":-206.55612529896217,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":21.455796767742868,"height":18.186031696330048,"seed":1934291802,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false},{"type":"text","version":222,"versionNonce":1217175614,"isDeleted":false,"id":"wPFhmt8e","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-221.5240003139031,"y":-191.30186387976903,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":11.3599853515625,"height":25,"seed":704523354,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u","rawText":"u","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u","lineHeight":1.25,"baseline":18},{"type":"line","version":335,"versionNonce":1278937762,"isDeleted":false,"id":"WNfo4mPj7oBzBueDPxkis","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-203.7890922958844,"y":-196.92512739767741,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":65.96520665238668,"height":1.081396830366998,"seed":1300629062,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[65.96520665238668,-1.081396830366998]]},{"type":"ellipse","version":236,"versionNonce":1892280446,"isDeleted":false,"id":"UodOMKIPxDMYplg-L6V_Z","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-136.30993008098395,"y":-206.44141950490697,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":16.869790553725124,"height":15.355834991211324,"seed":665602374,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false},{"type":"text","version":237,"versionNonce":1199924834,"isDeleted":false,"id":"z2Ve39ME","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-132.20062212558938,"y":-193.03209880835624,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10.459991455078125,"height":25,"seed":2044071366,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"v","rawText":"v","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"v","lineHeight":1.25,"baseline":18},{"type":"text","version":223,"versionNonce":1790191806,"isDeleted":false,"id":"1gb5sA8i","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-178.26812709922334,"y":-230.01587040690748,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10.939987182617188,"height":25,"seed":337262534,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e","rawText":"e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e","lineHeight":1.25,"baseline":18},{"type":"text","version":213,"versionNonce":1754155554,"isDeleted":false,"id":"XakQxQmC","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-216.5149927300738,"y":-270.5338671433383,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":99.41990661621094,"height":25,"seed":1173685126,"groupIds":["AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"Incidentes","rawText":"Incidentes","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"Incidentes","lineHeight":1.25,"baseline":18},{"type":"text","version":272,"versionNonce":1709990142,"isDeleted":false,"id":"wqqgdaki","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-270.34246602337583,"y":-144.29286551155366,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":222.459716796875,"height":25,"seed":1009448646,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são incidentes a ","rawText":" e   são incidentes a ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são incidentes a ","lineHeight":1.25,"baseline":18},{"type":"text","version":382,"versionNonce":105166306,"isDeleted":false,"id":"ejGHugwA","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-281.34246602337583,"y":-144.29286551155366,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":242.7596435546875,"height":25,"seed":1377714074,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                  e","rawText":"u   v                  e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                  e","lineHeight":1.25,"baseline":18},{"id":"z08tEvt2","type":"text","x":-224.33764424603208,"y":-85.78836632744594,"width":117.81988525390625,"height":25,"angle":0,"strokeColor":"#2f9e44","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":1480202338,"version":226,"versionNonce":1978896702,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"Adjacentes ","rawText":"Adjacentes ","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"Adjacentes ","lineHeight":1.25},{"id":"oLidlY6Vd1eVHndOxSSCj","type":"ellipse","x":-210.33764424603208,"y":-11.788366327445942,"width":18.5,"height":17,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"seed":348109922,"version":373,"versionNonce":1102555554,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false},{"type":"ellipse","version":500,"versionNonce":371898750,"isDeleted":false,"id":"f1X5FWvk5hrRMXp7TT3yG","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-135.08764424603208,"y":4.711633672554058,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":862545790,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false},{"type":"ellipse","version":474,"versionNonce":1108747618,"isDeleted":false,"id":"EZID2798LPl6lebk8UFgq","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-139.58764424603208,"y":-44.78836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":1768518178,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false},{"id":"PNMX0VbipxCgLGH4BKhZO","type":"line","x":-195.83764424603208,"y":-10.288366327445942,"width":57.5,"height":24.5,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"seed":1239108222,"version":264,"versionNonce":768793022,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"points":[[0,0],[57.5,-24.5]],"lastCommittedPoint":null,"startBinding":null,"endBinding":null,"startArrowhead":null,"endArrowhead":null},{"type":"line","version":375,"versionNonce":1890527522,"isDeleted":false,"id":"m-2mjWmd0QFCYpKtEPvxk","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-190.3643547531148,"y":1.002768449059701,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":54.5,"height":12,"seed":744607074,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[54.5,12]]},{"id":"KCsn2p8b","type":"text","x":-174.33764424603208,"y":-53.78836632744594,"width":16.179977416992188,"height":25,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":524773630,"version":246,"versionNonce":336392702,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"e´","rawText":"e´","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"e´","lineHeight":1.25},{"id":"9AKS8btf","type":"text","x":-169.83764424603208,"y":7.211633672554058,"width":10.939987182617188,"height":25,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":147591102,"version":199,"versionNonce":888255714,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"e","rawText":"e","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"e","lineHeight":1.25},{"id":"HxK9kOVq","type":"text","x":-227.83764424603208,"y":-7.788366327445942,"width":11.3599853515625,"height":25,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":428905186,"version":267,"versionNonce":333054526,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"u","rawText":"u","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"u","lineHeight":1.25},{"id":"eaLXljUF","type":"text","x":-271.8376442460321,"y":46.71163367255406,"width":214.25973510742188,"height":25,"angle":0,"strokeColor":"#1e1e1e","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":1983866622,"version":374,"versionNonce":812435618,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"  e   são adjacentes","rawText":"  e   são adjacentes","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"  e   são adjacentes","lineHeight":1.25},{"id":"hd9ojiZj","type":"text","x":-271.3376442460321,"y":47.21163367255406,"width":57.11991882324219,"height":25,"angle":0,"strokeColor":"#2f9e44","backgroundColor":"transparent","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"seed":1582856674,"version":289,"versionNonce":1880820350,"isDeleted":false,"boundElements":null,"updated":1710791717407,"link":null,"locked":false,"text":"e   e´","rawText":"e   e´","fontSize":20,"fontFamily":1,"textAlign":"left","verticalAlign":"top","baseline":18,"containerId":null,"originalText":"e   e´","lineHeight":1.25},{"type":"text","version":312,"versionNonce":2060412002,"isDeleted":false,"id":"lGDBrsO1","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-267.71746602337583,"y":-119.28836632744594,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":211.81968688964844,"height":25,"seed":614997666,"groupIds":["jULvgpI_jw0I4GRtIO2Nb","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                ","rawText":"u   v                ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                ","lineHeight":1.25,"baseline":18},{"type":"text","version":428,"versionNonce":1737558718,"isDeleted":false,"id":"G7BTDzJF","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-259.0675026444696,"y":-120.28836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":214.25973510742188,"height":25,"seed":1045650494,"groupIds":["giOkxg_aoKh7L4yrSlfC3","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1710791717407,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são adjacentes ","rawText":" e   são adjacentes ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são adjacentes ","lineHeight":1.25,"baseline":18}],"appState":{"theme":"dark","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#2f9e44","currentItemBackgroundColor":"transparent","currentItemFillStyle":"solid","currentItemStrokeWidth":2,"currentItemStrokeStyle":"solid","currentItemRoughness":1,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","scrollX":462.8376442460321,"scrollY":356.53836632744594,"zoom":{"value":2},"currentItemRoundness":"round","gridSize":null,"gridColor":{"Bold":"#C9C9C9FF","Regular":"#EDEDEDFF"},"currentStrokeOptions":null,"previousGridSize":null,"frameRendering":{"enabled":true,"clip":true,"name":true,"outline":true}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Drawing_2024-03-17_1752.11.excalidraw.md1");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>

- **Loop** (LAÇO): uma aresta com extremos idênticos.
![](https://i.imgur.com/XMeXXkM.png)
- **Link** (enlace): aresta com extremos diferentes.
![](https://i.imgur.com/HnYrJJx.png)
- **Arestas Múltiplas**: mais de uma aresta com os mesmos extremos. 
![](https://i.imgur.com/8wKVP0F.png)

- **Arestas paralelas**: duas arestas com os mesmos extremos.
![](https://i.imgur.com/8t3gPix.png)

### Graus

#### Definição de grau
- **Definição:** O grau de um vértice v, denotado por d(v), é o número de arestas incidentes a esse vértice v .
	- Grafos com apenas um vértice são ditos *triviais*.
	- Um grafo é *simples* se não possuir laços e arestas múltiplas. 
	
![](https://i.imgur.com/PS0X9wE.png)

| vertices | Arestas |
| -------- | ------- |
| d(u)     | 1       |
| d(v)     | 4       |
| d(w)     | 2       |
| d(z)     | 0        |


- A **sequência de grau de um grafo** consiste em que os graus são escritos em ordem crescente.

$$
I
$$

![](https://i.imgur.com/sICkvTY.png)

$$
II
$$

![](https://i.imgur.com/l6Ic04A.png)

$$
III
$$

![](https://i.imgur.com/Useg3BA.png)

<ol type="A" style="list-style-type:upper-roman;">
<li>Sequência de grau do grafo (i):  (1, 1, 2, 2, 2)</li>
<li>Sequência de grau do grafo (ii): (1, 1, 2, 2, 2)</li>
<li>Sequência de grau do grafo (iii):  (1, 3, 6, 8)</li>
</ol>


#### Grau de Entrada ou Saída
- **Grau de entrada**: o vértice é denotado **d⁻(v)⁺**.
	- O vértice é chamado de **fonte** (é a origem de suas arestas incidentes).
- **Grau de saída**: o vértice é denotado **d⁺(v)**.
	- O vértice é chamado de **sumidouro**.
	
![](https://i.imgur.com/2iP2jWq.png)

#### Soma dos graus
- O grafo é chamado de dígrafo balanceado se:

$$
d⁻(v) = d⁺(v)
$$

- Exemplo:
![](https://i.imgur.com/JUvcAS8.png)

| d⁻(v)     | d⁺(v)     |
| --------- | --------- |
| d⁻(a) = 2 | d⁺(v) = 2 |
| d⁻(b) = 2 | d⁺(v) = 2 |
| d⁻(c) = 1 | d⁺(v) = 3 |
| d⁻(d) = 1 | d⁺(v) = 0 |
| total = 6 | total = 6 | 


### Ordem, Tamanho e Rótulo
- Um grafo é dito **rotulado** se existem atribuições associadas a suas arestas ou vértices
- Denomina-se **ordem** de G a cardinalidade do seu conjunto de vértices. |V|= n.
- Denomina-se **tamanho** de G a cardinalidade do seu conjunto de arestas. |E|= m.
![](https://i.imgur.com/0Hdmh4R.png)

Grafo (1) ordem  5       e tamanho     8   . 
Grafo (2) ordem    4     e tamanho     4    .

### Direcionado ou Orientado
**Definição**: Um grafo é dito direcionado ou orientado ou, simplesmente,  *dígrafo* quando o *sentido das ligações entre os vértices é importante*. Nesse caso, as **arestas** possuem um sentido marcado por uma seta e recebem o nome de **arcos**.

```mermaid
flowchart LR

a --> b
b --> a
a --> c
c--> d
d--->b
c-->e
e-->a

```

## Teoremas
### Teorema 1
- Em **qualquer grafo**, a soma dos graus de um grafo **G = (V; E)** é igual a duas vezes o número de arestas
$$ \sum d(v_i) = 2 |E| = 2m$$

- **Exemplo:** Um grafo tem exatamente 4 vértices,  cada um de grau 3. Quantas arestas este grafo tem?

$$
\begin{aligned}
 \sum d(v_i) &= 4 \cdot 3 = 12  && \text (1)  \\
    \sum d(v_i) &= 2 |E|\\
    12     &= 2|E|        \\
    |E|     &= \frac{12}{2} \\
    |E| &= 6 \text{ arestas}
\end{aligned}
$$

> [!important] Importante
> **Corolário 1:** O número de vértices de grau impar é par (trivial). 

### Grafos simples
- Um **grafo simples** com **N** nós pode ter:
$$
C(n,2) =  \frac{n\cdot(n-1)}{2}
$$
diferentes arestas e cada uma delas pode estar presente ou não
- E por meio dessa conta calculamos o **máximo de grafos simples** com N nós:

$$
2^{n \cdot(n-1)/2}
$$