<div align = center>
<h1> O que é flex-box: <h1>

<img height = "200px" src = "https://user-images.githubusercontent.com/100320094/229650304-6be97c63-c5b3-4923-9993-075df6d8e5c6.png">
</div>


* O flex-box é utilizado para um layout mais organizado e responsivo, sem causar problemas como no método antigo (margin).

---
<div align = center> 
<h2>Principais Comandos Para Flex-Box</h2>
  </div>
  
  * `display-flex:` é o elemento que define um container como flex-box;
  * `flex-direction:` permite alterar a direção dos itens, nele podem ser utilizados os elementos: <br>
  <br>
  
  **row:** alinha os itens da esquerda para direita; Exemplo Utilizando 2 divs: <br>
  <img height = "100px" src ="https://user-images.githubusercontent.com/100320094/229655581-51f865a5-a47e-4aca-8556-8c0f6e1affaa.png">
  
  
  
  **column:** alinha os itens em forma de coluna (verticalmente); Exemplo Utilizando 2 divs:<br>
  <img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229654591-7ea784e2-824a-4550-8b9a-7d81ca71fb15.png">
  
  **row-reverse:** alinha os itens da direita para esquerda; 
 Exemplo Utilizando 2 divs:  <br>
  <img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229655710-fccfdadd-8265-4221-b24c-cf4c652e830f.png">
  <br>
  **column-reverse:** alinha os itens debaixo para cima. Exemplo Utilizando 2 divs: <br> 
   <img height= "100px" src = "https://user-images.githubusercontent.com/100320094/229655290-95d74273-0589-4c21-874e-864256039b96.png"> 
  
  
* `justify-content:` Define a posição horizontal dos itens, nele podem ser utilizados os elementos: <br> 
<br> 

**flex-start:** alinha os elementos rente à borda esquerda do conteiner; Exemplo: <br>
<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229657206-d7647ea5-45d2-48c8-a25b-7897cd98bd95.png"> <br>

**center:** alinha os elementos ao centro; Exemplo: <br>
<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229657735-b6840ec1-8094-42c1-b8e4-929710b75709.png"> <br>

**space-between:** é utilizado para distribuir espaços livres horizontalmente, no caso a div 1 vai para esquerda e a div 2 irá para direita, deixando assim um espaço ao centro; Exemplo: <br>

<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229658087-0d81c7e7-fc69-43a1-bd2d-6214d7cda465.png"> <br>

**space-around:** ele é utilizado para distribuir o espaço em branco ao redor dos itens; Exemplo: <br> 
<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229658349-a98c39c5-ddbb-41a1-b22f-d7a5bceb0c96.png"> <br>

* `align-items:` Define a posição vertical dos itens, seus elementos são **flex-start**, **center**, que já citamos e: <br> 

**flex-end:** puxa os itens para baixo; Exemplo: <br> 
<img height = "100px;" src = "https://user-images.githubusercontent.com/100320094/229659095-1a6f5e4b-c25e-4e7f-b570-c1e9abb78ade.png"> <br>


**baseline**: utilizado para alinhar textos; Exemplos: <br> 
<img height = "150px" src= "https://user-images.githubusercontent.com/100320094/229659671-b1423896-a959-438b-a4cb-f101e61f02c7.png"> <br>

 **stretch**: podemos alinhar objetos deixando-os do mesmo tamanho e que respeitem o tamanho do container. A propriedade só funciona acompanhada da propriedade `flex-direction` que indica o fluxo do container (row ou column). Exemplos:
 
<img height ="100px" src = "https://user-images.githubusercontent.com/100320094/229935815-a38a4052-8f4e-4e46-a045-36fad87f28a3.png"><img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229936280-085d41f5-3bb8-464e-a2ea-e40b594b8bb7.png" ><br>


* Obs: Perceba que no exemplo 2 eu coloquei a child 1 com 500px de largura e a child 2 com 200px de largura, a função do stretch trás isso, conseguir colocar os elementos e eles respeitem até a borda do nosso container, assim como no exemplo 1, mas respeitando verticalmente. 

`flex-wrap:` permite serem postos em uma linha (nowrap) ou quebrar linhas (wrap).
<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229940216-fbc1a2a0-42d9-4c2f-860e-61f364326a9e.png"><img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229940330-a81a730f-fb35-4c63-8b42-25a1a9874edf.png"><br>

`align-content:` É usado para alinhas os itens verticalmente. Podem ser utilizados os seguintes elementos: **flex-start, flex-end, center, space-between, space-around e stretch.** 

* OBS: esta propriedade só funcionará se conter o flex-wrap definido. 

`flex-grow:` ele deixa os itens do mesmo tamanho ocupando o espaço disponível proporcionalmente. 
<img height = "100px" src= "https://user-images.githubusercontent.com/100320094/229942680-87b3501b-a4a9-4576-a940-ab9dd7e63129.png"> <br> 
* OBS: Neste caso, eu coloquei o valor do `flex-grow`da **child 1** como valor **1px** e a **child 2** com valor **0px**, assim podemos observar com clareza
que a child que vai ser maior é a que tiver maior valor.

`flex-shrink:` ao contrário do `flex-grow`, este elemento diminui os elementos para maior espaçamento na container. Exemplo: 
<img height = "100px" src= "https://user-images.githubusercontent.com/100320094/229943481-19ad0ef1-7935-4297-999b-528cb5f9bcf5.png"><img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229943957-e6c84e33-f4dc-475d-8755-5eab825917ec.png"><br> 
* OBS: O flex-shrink funciona junto ao flex-direction, então isso definirá se é row ou column. 


`flex-basis:` é possível definir o tamanho de um item antes dele crescer. Exemplo: **flex-basis: 25%;** 
<img height = "100px" src = "https://user-images.githubusercontent.com/100320094/229944501-1aac9267-8b96-4485-904f-5993f480c18d.png"><br>


`order:` define a ordem em que os itens devem aparecer no layout.













