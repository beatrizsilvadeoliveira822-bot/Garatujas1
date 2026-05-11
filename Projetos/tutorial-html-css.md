[fonte]https://github.com/drachehavoc/ia26-webdesign

tutorial-html-css.md
# html e css (teoria)
html: uma linguagem de marcação, podemos imaginar assim..

-> html é um "ajudante" seu, ele vai te dizer o que é cada coisa e onde ela fica.

é basicamente isso que ele faz com o navegador.

no html, temos as "tags", que diz o que é cada coisa, um exemplo de tag: < main >, ele diz para o navegador que tal coisa é o conteudo principal.

toda tag começa aberta < > e precisa ser fechada </ >
nas tag. O HTML também permite a inclusão de atributos nas tags para fornecer informações adicionais sobre os elementos, como class, id, src, etc.

-> já o css, ele **especifica** melhor o que o html diz.
Ele permite que você defina regras de estilo para os elementos HTML, como cores, fontes, margens, espaçamento, entre outros. O CSS é separado do HTML, o que significa que você pode manter a estrutura do conteúdo (HTML) separada da apresentação visual (CSS). O CSS é composto por seletores e declarações. Os seletores são usados para selecionar os elementos HTML aos quais as regras de estilo serão aplicadas, enquanto as declarações definem as propriedades de estilo e seus valores.

# html estrutura básica
< !DOCTYPE html >

< html lang="pt-BR" >

< head >
 
< meta charset="UTF-8" >
 
< title >Título da Página</ title >

< head >

< body >

< /body >

< /html >

- explicação

< !DOCTYPE html >
afirma para o navegador que o site é em html

< head > 
-->é a seção do documento onde são incluídas informações sobre a página, como o título, links para arquivos CSS, scripts JavaScript, meta tags (metainformações), entre outros. não é exibido diretamente na página, mas é essencial para o funcionamento e a aparência da página web.

< body >
-->  é a seção do documento onde o conteúdo visível da página é colocado. É aqui que você adiciona os elementos HTML que compõem a estrutura e o conteúdo da página, como títulos, parágrafos, imagens, links etc. O conteúdo do < body > é o que os usuários veem quando acessam a página web.

**importante**
-->todo conteudo deve ser escrito dentro da tag < html >, que é a base de tudo. 
temos outros atributos como: **lang="pt-BR"** indica que o idioma principal do conteúdo da página é o português do Brasil, o que é importante para a acessibilidade e para os mecanismos de busca entenderem o idioma da página. O elemento **< meta charset="UTF-8" >** define a codificação de caracteres do documento como UTF-8, garantindo que caracteres acentuados e outros símbolos sejam exibidos corretamente. O elemento **< title >** define o título da página, que é exibido na aba do navegador e nos resultados de busca.

**Atributos HTML**
Os atributos HTML são usados para fornecer informações adicionais sobre os elementos HTML. Eles são escritos dentro da tag de abertura de um elemento e consistem em um nome e um valor, separados por um sinal de igual "=".

# CSS exemplo
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: #333333;
  text-align: center;
}

p {
  color: #666666;
  font-size: 18px;
  margin: 20px;
}


No exemplo acima, o CSS é aplicado ao HTML, pois o arquivo styles.css está vinculado ao documento HTML usando a tag < link > no < head >. O CSS define o estilo para o elemento < body >, o título < h1 > e o parágrafo < p >, controlando a aparência da página web.

# CSS sintaxe
A sintaxe do css é basicamente a parte onde especifiamos o que queremos no html, snedo composto por *regras de estilos*, onde cada regra é formada por um **seletor** que seleciona os elementos em html para serem modificados, enquanto o **bloco de declarações** define as propriedades de estilo e seus valores.

# Seletores CSS
 A lógica dos seletores é baseada na estrutura do documento HTML seguindo a hierarquia de elementos. eles permitem que você aplique estilos a elementos específicos ou a grupos de elementos com base em suas características, como tipo, classe, ID, atributos, entre outros.

**explicação do seletores**
​Os seletores mais simples são os de **Tipo**, que buscam pela tag HTML (como todos os parágrafos ou todos os títulos), e os de **Classe**, que são extremamente versáteis por permitirem agrupar elementos diferentes sob um mesmo estilo usando um ponto antes do nome. Já o seletor de **ID**, marcado pelo símbolo de sustenido (#), é o mais específico e deve ser usado para identificar um elemento único e exclusivo na página. Para um refinamento maior, existem os seletores de **Atributo**, que filtram elementos por propriedades internas (como um link que aponta para um destino específico), e as **Pseudo-classes**, que aplicam estilos baseados no estado do elemento, como quando o usuário passa o mouse por cima dele.
​Quando entramos na estrutura da página, utilizamos os **Combinadores** para definir relações de parentesco. O seletor de **Descendente** é o mais comum, usando apenas um espaço para encontrar qualquer elemento dentro de outro. Se precisarmos de mais precisão, o seletor de **Filho Direto** (>) ignora netos ou bisnetos, focando apenas no nível imediato abaixo. Para elementos que estão no mesmo nível de hierarquia, usamos os seletores de **Irmãos***: **o Adjacente** (+) seleciona apenas o próximo elemento imediato, enquanto o **Irmão Geral** (~) seleciona todos os irmãos que aparecem na sequência, independentemente da distância entre eles.