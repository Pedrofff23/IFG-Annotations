---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Conceitos Básicos/","tags":["grafos"],"created":"2024-03-17T17:45:56.868-03:00"}
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
<style> .container {font-family: sans-serif; text-align: center;} .button-wrapper button {z-index: 1;height: 40px; width: 100px; margin: 10px;padding: 5px;} .excalidraw .App-menu_top .buttonList { display: flex;} .excalidraw-wrapper { height: 800px; margin: 50px; position: relative;} :root[dir="ltr"] .excalidraw .layer-ui__wrapper .zen-mode-transition.App-menu_bottom--transition-left {transform: none;} </style><script src="https://cdn.jsdelivr.net/npm/react@17/umd/react.production.min.js"></script><script src="https://cdn.jsdelivr.net/npm/react-dom@17/umd/react-dom.production.min.js"></script><script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@excalidraw/excalidraw@0/dist/excalidraw.production.min.js"></script><div id="Drawing_2024-03-17_1752.11.excalidraw.md1"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.0.25","elements":[{"type":"ellipse","version":308,"versionNonce":1706030730,"isDeleted":false,"id":"m__w-3O2se0RxAF6xNKwY","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-247.33984593288878,"y":-208.55612529896217,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":21.455796767742868,"height":18.186031696330048,"seed":1934291802,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false},{"type":"text","version":306,"versionNonce":106434326,"isDeleted":false,"id":"wPFhmt8e","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-243.0240003139031,"y":-193.30186387976903,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10,"height":25,"seed":704523354,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u","rawText":"u","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u","lineHeight":1.25,"baseline":19},{"type":"line","version":416,"versionNonce":910464330,"isDeleted":false,"id":"WNfo4mPj7oBzBueDPxkis","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-225.2890922958844,"y":-198.92512739767741,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":65.96520665238668,"height":1.081396830366998,"seed":1300629062,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[65.96520665238668,-1.081396830366998]]},{"type":"ellipse","version":317,"versionNonce":770817110,"isDeleted":false,"id":"UodOMKIPxDMYplg-L6V_Z","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-157.80993008098395,"y":-208.44141950490697,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":16.869790553725124,"height":15.355834991211324,"seed":665602374,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false},{"type":"text","version":321,"versionNonce":811031562,"isDeleted":false,"id":"z2Ve39ME","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-153.70062212558938,"y":-195.03209880835624,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10,"height":25,"seed":2044071366,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"v","rawText":"v","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"v","lineHeight":1.25,"baseline":19},{"type":"text","version":307,"versionNonce":677626262,"isDeleted":false,"id":"1gb5sA8i","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-199.76812709922334,"y":-232.01587040690748,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":8.876953125,"height":25,"seed":337262534,"groupIds":["yT83nXoXPczJuJ79fJIJ9","AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e","rawText":"e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e","lineHeight":1.25,"baseline":19},{"type":"text","version":297,"versionNonce":1373850314,"isDeleted":false,"id":"XakQxQmC","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-238.0149927300738,"y":-272.5338671433383,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":82.1875,"height":25,"seed":1173685126,"groupIds":["AJ86x_kcttxh-PQo0oyQ-","K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"Incidentes","rawText":"Incidentes","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"Incidentes","lineHeight":1.25,"baseline":19},{"type":"text","version":356,"versionNonce":685973206,"isDeleted":false,"id":"wqqgdaki","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-291.84246602337583,"y":-146.29286551155366,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":160.498046875,"height":25,"seed":1009448646,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são incidentes a ","rawText":" e   são incidentes a ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são incidentes a ","lineHeight":1.25,"baseline":19},{"type":"text","version":466,"versionNonce":562258314,"isDeleted":false,"id":"ejGHugwA","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-302.84246602337583,"y":-146.29286551155366,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":133.876953125,"height":25,"seed":1377714074,"groupIds":["K8IfWTH6Uyxbgnnjf_qfw","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                  e","rawText":"u   v                  e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                  e","lineHeight":1.25,"baseline":19},{"type":"text","version":310,"versionNonce":872731670,"isDeleted":false,"id":"z08tEvt2","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-245.83764424603208,"y":-87.78836632744594,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":93.84765625,"height":25,"seed":1480202338,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"Adjacentes ","rawText":"Adjacentes ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"Adjacentes ","lineHeight":1.25,"baseline":19},{"type":"ellipse","version":454,"versionNonce":443719754,"isDeleted":false,"id":"oLidlY6Vd1eVHndOxSSCj","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-231.83764424603208,"y":-13.788366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":348109922,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false},{"type":"ellipse","version":581,"versionNonce":1941823830,"isDeleted":false,"id":"f1X5FWvk5hrRMXp7TT3yG","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-156.58764424603208,"y":2.7116336725540577,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":862545790,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false},{"type":"ellipse","version":555,"versionNonce":411830026,"isDeleted":false,"id":"EZID2798LPl6lebk8UFgq","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-161.08764424603208,"y":-46.78836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":18.5,"height":17,"seed":1768518178,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false},{"type":"line","version":345,"versionNonce":191055510,"isDeleted":false,"id":"PNMX0VbipxCgLGH4BKhZO","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-217.33764424603208,"y":-12.288366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":57.5,"height":24.5,"seed":1239108222,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[57.5,-24.5]]},{"type":"line","version":457,"versionNonce":1145738698,"isDeleted":false,"id":"m-2mjWmd0QFCYpKtEPvxk","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-211.8643547531148,"y":-0.9972315509402989,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":54.5,"height":12,"seed":744607074,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":{"type":2},"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"startBinding":null,"endBinding":null,"lastCommittedPoint":null,"startArrowhead":null,"endArrowhead":null,"points":[[0,0],[54.5,12]]},{"type":"text","version":330,"versionNonce":1806304214,"isDeleted":false,"id":"KCsn2p8b","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-195.83764424603208,"y":-55.78836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":15.537109375,"height":25,"seed":524773630,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e´","rawText":"e´","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e´","lineHeight":1.25,"baseline":19},{"type":"text","version":283,"versionNonce":2127121546,"isDeleted":false,"id":"9AKS8btf","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-191.33764424603208,"y":5.211633672554058,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":8.876953125,"height":25,"seed":147591102,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e","rawText":"e","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e","lineHeight":1.25,"baseline":19},{"type":"text","version":351,"versionNonce":648485142,"isDeleted":false,"id":"HxK9kOVq","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-249.33764424603208,"y":-9.788366327445942,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":10,"height":25,"seed":428905186,"groupIds":["hVJpEgGu7rjWCICz7HNzW","v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u","rawText":"u","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u","lineHeight":1.25,"baseline":19},{"type":"text","version":458,"versionNonce":1304636234,"isDeleted":false,"id":"eaLXljUF","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-293.3376442460321,"y":44.71163367255406,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":148.818359375,"height":25,"seed":1983866622,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"  e   são adjacentes","rawText":"  e   são adjacentes","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"  e   são adjacentes","lineHeight":1.25,"baseline":19},{"type":"text","version":373,"versionNonce":1137673814,"isDeleted":false,"id":"hd9ojiZj","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-292.8376442460321,"y":45.21163367255406,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":39.4140625,"height":25,"seed":1582856674,"groupIds":["v4VAWzy8oUKfev4y5uCaa","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"e   e´","rawText":"e   e´","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"e   e´","lineHeight":1.25,"baseline":19},{"type":"text","version":396,"versionNonce":1200828938,"isDeleted":false,"id":"lGDBrsO1","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-289.21746602337583,"y":-121.28836632744594,"strokeColor":"#2f9e44","backgroundColor":"transparent","width":115,"height":25,"seed":614997666,"groupIds":["jULvgpI_jw0I4GRtIO2Nb","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"u   v                ","rawText":"u   v                ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"u   v                ","lineHeight":1.25,"baseline":19},{"type":"text","version":512,"versionNonce":335039382,"isDeleted":false,"id":"G7BTDzJF","fillStyle":"solid","strokeWidth":2,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-280.5675026444696,"y":-122.28836632744594,"strokeColor":"#1e1e1e","backgroundColor":"transparent","width":148.818359375,"height":25,"seed":1045650494,"groupIds":["giOkxg_aoKh7L4yrSlfC3","luMVKdjQXm3fAU-IusPFa"],"frameId":null,"roundness":null,"boundElements":[],"updated":1711764633953,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":" e   são adjacentes ","rawText":" e   são adjacentes ","textAlign":"left","verticalAlign":"top","containerId":null,"originalText":" e   são adjacentes ","lineHeight":1.25,"baseline":19}],"appState":{"theme":"dark","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#2f9e44","currentItemBackgroundColor":"transparent","currentItemFillStyle":"solid","currentItemStrokeWidth":2,"currentItemStrokeStyle":"solid","currentItemRoughness":1,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","scrollX":486.59344258587583,"scrollY":340.2861167353921,"zoom":{"value":2},"currentItemRoundness":"round","gridSize":null,"gridColor":{"Bold":"#C9C9C9FF","Regular":"#EDEDEDFF"},"currentStrokeOptions":null,"previousGridSize":null,"frameRendering":{"enabled":true,"clip":true,"name":true,"outline":true}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Drawing_2024-03-17_1752.11.excalidraw.md1");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>

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
