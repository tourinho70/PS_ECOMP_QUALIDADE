## Relatório ##

### 1. Linux ###

Comecei assistindo ao [Tutorial deploy NGINX](https://www.youtube.com/watch?v=FBl1gZzcESY) , recomendado no documento da atividade.

Executei o passo a passo em uma máquina virtual do Ubuntu, baixando o nginx e executando os comandos mostrados no vídeo. Obtive o seguinte resultado:

![nginx welcome](https://hackmd.io/_uploads/SkderjI9xe.png)

Após isso fiquei um pouco perdido e assisti a um [vídeo rápido](https://www.youtube.com/watch?v=JKxlsvZXG7c) explicando o que é o nginx.

Depois, vi que não precisava fazer o trabalho no Linux e recomecei ele no sistema nativo (macos), usando o vídeo [INX Tutorial for Beginners](https://www.youtube.com/watch?v=9t9Mp0BGnyI&t=1534s) para prosseguir na tarefa.

---

### 2. Fazendo a Atividade ###


Primeiramente, baixei o nginx com `brew install nginx` e "iniciei" ele com `nginx`:

| ![terminal](https://hackmd.io/_uploads/S14muiLcll.png) | ![welcome to ngix](https://hackmd.io/_uploads/SyY_KjLcxg.png)|
| -------- | -------- |

Depois, abri a pasta do jogo no vscode e aprendi o básico acerca do arquivo nginx.config:

|   ![Screenshot 2025-09-04 at 02.00.45](https://hackmd.io/_uploads/S1GcqsUqgx.png)   |
| ---- |

Em seguida, apaguei o conteúdo dele e segui o tutorial para adicionar o código que coloca a pasta do jogo como CAMINHO PARA A SAÍDA. Depois, recarreguei o nginx com `nginx -s reload`

| ![ALTERA NGINX COM RELOAD](https://hackmd.io/_uploads/HkhhosUqxl.png) | ![Screenshot 2025-09-04 at 02.10.47](https://hackmd.io/_uploads/ryvajo8clx.png) | 
| -------- | -------- | 

Só o HTML do site estava aparecendo. Outros tipos de arquivos, como os .css, estavam aparecendo com o `content-type`  definido como `text/plain`:



| ![CSS com text:plain](https://hackmd.io/_uploads/BJil13Uqle.png) |
| -------- |

Aprendi que isso aconteceu porque faltava incluir a diretiva "types". Essa diretiva deve conter os MIME types seguidos das extensões que vão usar o tipo (1ª imagem).

Aprendi também que é possível no nginx.config incluir o arquivo mime.types, que tem diversos MIME types seguidos das extensões que o usam (2ª imagem). Isso torna o processo mais prático, por isso optei por fazer dessa maneira.

|![Screenshot 2025-09-04 at 02.20.34](https://hackmd.io/_uploads/ryOel2Icll.png)|![Screenshot 2025-09-04 at 03.24.30](https://hackmd.io/_uploads/Sy4nlh89xl.png)|
| --- | ------------------------------------------------------------------------------- |


Assim, finalizei a atividade:


|   ![Screenshot 2025-09-04 at 02.22.02](https://hackmd.io/_uploads/BydRghUqle.png)   |
| ---- |

---

### 3. Desafios ###

Para mim, a parte mais desafiadora foi saber para onde ir após terminar de ver o 1º tutorial (do Linux). Cheguei a ler algumas páginas da web sobre o assunto, porém elas não estavam me ajudando muito. Foi somente após ver o vídeo rápido sobre nginx que entendi melhor o que procurar aprender.

### 4. Conclusões ###

No geral, a atividade foi divertida e achei o assunto bastante curioso, inclusive, assisti ao último tutorial mencionado um pouco além do necessário, justamente por essa curiosidade.

Consegui aprender o básico de nginx e fiquei satisfeito com a minha execução e com a minha entrega.





