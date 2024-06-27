---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos/","tags":["grafos"],"created":"2024-06-26T00:24:10.600-03:00"}
---

## Tópicos
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
<style> .container {font-family: sans-serif; text-align: center;} .button-wrapper button {z-index: 1;height: 40px; width: 100px; margin: 10px;padding: 5px;} .excalidraw .App-menu_top .buttonList { display: flex;} .excalidraw-wrapper { height: 800px; margin: 50px; position: relative;} :root[dir="ltr"] .excalidraw .layer-ui__wrapper .zen-mode-transition.App-menu_bottom--transition-left {transform: none;} </style><script src="https://cdn.jsdelivr.net/npm/react@17/umd/react.production.min.js"></script><script src="https://cdn.jsdelivr.net/npm/react-dom@17/umd/react-dom.production.min.js"></script><script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@excalidraw/excalidraw@0/dist/excalidraw.production.min.js"></script><div id="Drawing_2024-03-17_1752.11.excalidraw.md1"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.0.25","elements":[{"type":"ellipse","version":326,"versionNonce":1567669782,"isDeleted":false,"id":"m__w-3O2se0RxAF6xNKwY","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-256.3398459328888,"y":-209.55612529896217,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":21.455796767742868,"height":18.186031696330048,"seed":1934291802,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false},{"type":"text","version":324,"versionNonce":471632726,"isDeleted":false,"id":"wPFhmt8e","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-252.0240003139031,"y":-194.30186387976903,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":11.3599853515625,"height":25,"seed":704523354,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u","rawText":"u","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u","lineHeight":1.25,"baseline":18},{"type":"line","version":434,"versionNonce":1180479638,"isDeleted":false,"id":"WNfo4mPj7oBzBueDPxkis","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-234.2890922958844,"y":-199.92512739767741,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":65.96520665238668,"height":1.081396830366998,"seed":1300629062,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[65.96520665238668,-1.081396830366998]]},{"type":"ellipse","version":335,"versionNonce":400960982,"isDeleted":false,"id":"UodOMKIPxDMYplg-L6V_Z","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-166.80993008098395,"y":-209.44141950490697,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":16.869790553725124,"height":15.355834991211324,"seed":665602374,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false},{"type":"text","version":339,"versionNonce":231605014,"isDeleted":false,"id":"z2Ve39ME","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-162.70062212558938,"y":-196.03209880835624,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10.459991455078125,"height":25,"seed":2044071366,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"v","rawText":"v","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"v","lineHeight":1.25,"baseline":18},{"type":"text","version":325,"versionNonce":982069334,"isDeleted":false,"id":"1gb5sA8i","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-208.76812709922334,"y":-233.01587040690748,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10.939987182617188,"height":25,"seed":337262534,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e","rawText":"e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e","lineHeight":1.25,"baseline":18},{"type":"text","version":315,"versionNonce":434943382,"isDeleted":false,"id":"XakQxQmC","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-247.0149927300738,"y":-273.5338671433383,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":99.41990661621094,"height":25,"seed":1173685126,"groupIds":["AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"Incidentes","rawText":"Incidentes","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"Incidentes","lineHeight":1.25,"baseline":18},{"type":"text","version":374,"versionNonce":1697485526,"isDeleted":false,"id":"wqqgdaki","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-300.84246602337583,"y":-147.29286551155366,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":222.459716796875,"height":25,"seed":1009448646,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são incidentes a ","rawText":" e   são incidentes a ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são incidentes a ","lineHeight":1.25,"baseline":18},{"type":"text","version":484,"versionNonce":1726007318,"isDeleted":false,"id":"ejGHugwA","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-311.84246602337583,"y":-147.29286551155366,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":242.7596435546875,"height":25,"seed":1377714074,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                  e","rawText":"u   v                  e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                  e","lineHeight":1.25,"baseline":18},{"type":"text","version":328,"versionNonce":1325094230,"isDeleted":false,"id":"z08tEvt2","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-254.83764424603208,"y":-88.78836632744594,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":117.81988525390625,"height":25,"seed":1480202338,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"Adjacentes ","rawText":"Adjacentes ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"Adjacentes ","lineHeight":1.25,"baseline":18},{"type":"ellipse","version":472,"versionNonce":114440854,"isDeleted":false,"id":"oLidlY6Vd1eVHndOxSSCj","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-240.83764424603208,"y":-14.788366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":348109922,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false},{"type":"ellipse","version":599,"versionNonce":85620694,"isDeleted":false,"id":"f1X5FWvk5hrRMXp7TT3yG","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-165.58764424603208,"y":1.7116336725540577,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":862545790,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false},{"type":"ellipse","version":573,"versionNonce":568921366,"isDeleted":false,"id":"EZID2798LPl6lebk8UFgq","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-170.08764424603208,"y":-47.78836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":1768518178,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false},{"type":"line","version":363,"versionNonce":1790114390,"isDeleted":false,"id":"PNMX0VbipxCgLGH4BKhZO","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-226.33764424603208,"y":-13.288366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":57.5,"height":24.5,"seed":1239108222,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[57.5,-24.5]]},{"type":"line","version":475,"versionNonce":1984774038,"isDeleted":false,"id":"m-2mjWmd0QFCYpKtEPvxk","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-220.8643547531148,"y":-1.997231550940299,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":54.5,"height":12,"seed":744607074,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[54.5,12]]},{"type":"text","version":348,"versionNonce":955047126,"isDeleted":false,"id":"KCsn2p8b","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-204.83764424603208,"y":-56.78836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":16.179977416992188,"height":25,"seed":524773630,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e´","rawText":"e´","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e´","lineHeight":1.25,"baseline":18},{"type":"text","version":301,"versionNonce":1478939158,"isDeleted":false,"id":"9AKS8btf","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-200.33764424603208,"y":4.211633672554058,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10.939987182617188,"height":25,"seed":147591102,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e","rawText":"e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e","lineHeight":1.25,"baseline":18},{"type":"text","version":369,"versionNonce":2129665878,"isDeleted":false,"id":"HxK9kOVq","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-258.3376442460321,"y":-10.788366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":11.3599853515625,"height":25,"seed":428905186,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u","rawText":"u","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u","lineHeight":1.25,"baseline":18},{"type":"text","version":476,"versionNonce":832423062,"isDeleted":false,"id":"eaLXljUF","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-302.3376442460321,"y":43.71163367255406,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":214.25973510742188,"height":25,"seed":1983866622,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"  e   são adjacentes","rawText":"  e   são adjacentes","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"  e   são adjacentes","lineHeight":1.25,"baseline":18},{"type":"text","version":391,"versionNonce":568639958,"isDeleted":false,"id":"hd9ojiZj","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-301.8376442460321,"y":44.21163367255406,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":57.11991882324219,"height":25,"seed":1582856674,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e   e´","rawText":"e   e´","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e   e´","lineHeight":1.25,"baseline":18},{"type":"text","version":414,"versionNonce":47847190,"isDeleted":false,"id":"lGDBrsO1","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-298.21746602337583,"y":-122.28836632744594,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":211.81968688964844,"height":25,"seed":614997666,"groupIds":["jULvgpI_jw0I4GRtIO2Nb","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                ","rawText":"u   v                ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                ","lineHeight":1.25,"baseline":18},{"type":"text","version":530,"versionNonce":1559413846,"isDeleted":false,"id":"G7BTDzJF","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-289.5675026444696,"y":-123.28836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":214.25973510742188,"height":25,"seed":1045650494,"groupIds":["giOkxg_aoKh7L4yrSlfC3","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764797822,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são adjacentes ","rawText":" e   são adjacentes ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são adjacentes ","lineHeight":1.25,"baseline":18}],"appState":{"theme":"dark","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#2f9e44","currentItemBackgroundColor":"transparent","currentItemFillStyle":"solid","currentItemStrokeWidth":2,"currentItemStrokeStyle":"solid","currentItemRoughness":1,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","scrollX":472.4626442460321,"scrollY":342.2861167353921,"zoom":{"value":2},"currentItemRoundness":"round","gridSize":null,"gridColor":{"Bold":"#C9C9C9FF","Regular":"#EDEDEDFF"},"currentStrokeOptions":null,"previousGridSize":null,"frameRendering":{"enabled":true,"clip":true,"name":true,"outline":true}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Drawing_2024-03-17_1752.11.excalidraw.md1");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>

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
