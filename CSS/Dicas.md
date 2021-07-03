Idealmente montar as páginas assim com includes nas páginas. Cada página recebe

require_once 'header.php';
require_once 'menu.php';
página: index.php, outra.php
require_once 'footer.php';

## Cor de bordas de inputs text
```css
input[type=text] {
  border: 2px solid red;
  border-radius: 4px;
}
```
## Design Responsivo

Viewport - O viewport é a área visível do user de uma web page, que definimos na tag <head>.
O viewport para o device celular será menor em um mobile phone do que em uma tela de computador.
https://pt.stackoverflow.com/questions/272210/o-que-%C3%A9-view-port

Usar este:
<meta name="viewport" content="width=device-width, initial-scale=1.0">


É muito importante atualmente criar sites responsivos, ou seja, que se ajustem automaticamente ao tamanho do dispositivo que acessa nosso site. Podemos ver isso redimensionando a janela do navegador. Sites responsivos se ajustam ao tamanho do dispositivo.

Como existem uma grande quantidade de usuários que atualmente acessa sites através de celulares, então se nosso site não for responsivo ele fica muito ruim de ser acessado através de um celular. 

Existem muitas boas informações sobre como criar sites responsivos
- https://www.hostinger.com.br/tutoriais/criar-site-responsivo-css 
- http://www.carloshps.com.br/blog/criar-site-responsivo-com-html5-e-css3-parte-1-de-3/ 
- https://marketingdeconteudo.com/como-criar-uma-pagina-web-responsiva/ 

Uma dica interessante é sobre imagens: quando usar imagens em site responsivo use o tamanho com % e não especifique a altura, mas somente a largura com porcentagem. Assim o navegador calculará automaticamente a altura proporcionalmente a largura.
- https://www.w3schools.com/css/css_rwd_intro.asp

Detalhes:
- http://blog.popupdesign.com.br/design-responsivo-i-o-que-e-e-por-que-usar/ 
- http://blog.popupdesign.com.br/desenvolvimento-responsivo-e-viewport/ 
- http://blog.popupdesign.com.br/palestra-design-e-desenvolvimento-responsivo/ 

Compatibilidade com navegadores

Praticamente cada um dos navegadores implementa as propriedades a sua maneira e quando criamos um CSS e setamos valores para propriedades e usamos nosso CSS numa página aparece diferente do que fizemos. Isso mostra duas coisas, que precisamos resetar os valores de propriedades dos navegadores logo no início do nosso CSS e mais ainda que deve ser indicativo de uso de bons frameworks como o BootStrap e o jQuery, pois estes já corrigem a compatibilidade com os navegadores.


Para organizar seu código CSS:

Você tem alguns arquivos:

reset.css
format.css
layout.css

Criar o 
master.css

E nele importar os demais:
@import url("reset.css");
@import url("format.css");
@import url("layout.css");

Na página html:
<style type="text/css" media="screen">@import url("master.css")</style>
