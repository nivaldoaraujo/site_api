# Descrição
Um projeto com objetivo de estudos baseado em API rest. A comunicação é síncrona, ou seja, comunicam-se através de requisições HTTP.


# Análise técnica

### Comunicação
Para facilitar a comunicação entre os microserviços, usei diversas ferramentas. Entre elas estão: 
- <b>Servidor json</b> ➡️ É um formato de dados leve e de fácil leitura utilizado para troca de informações entre sistemas computacionais. 
- <b>Axios</b> ➡️ axios é que ele é um cliente HTTP baseado em promessas totalmente agnóstico, ou seja, que não depende de frameworks e bibliotecas. Ele é super maleável, podendo ser utilizado do lado do cliente (React, Vue, Svelte, etc) e do lado do backend (express, nest, etc). Então vamos mergulhar um pouco mais fundo e ver o que a gente consegue fazer com ele.
  
  O Eureka Server também se encarrega de realizar o <b>balanceamento de carga</b>, equilibrando o volume de requisições para aquele projeto que está instanciado mais de uma vez.

### Endpoints

Possui diversos endpoints que podem ser importados para o postman usando o arquivo JSON disponibilizado no repositório. Como o sistema usa <b>Eureka server</b>, todos os endpoints possuem o mesmo localhost (http://localhost:8765)

- <b>GET</b> (/ms-cart/cart) ➡️ Responsável por mostrar todos os itens dentro do carrinho, bem como o valor unitário e quantidade.
  
- <b>POST</b> (/ms-cart/cart) ➡️ Através do body, adiciona um item ao carrinho. Antes é feita a comunicação com o serviço de Produto para verificar a existencia do produto e se há estoque disponível.
  
- <b>GET</b> (/ms-cart/cart/total) ➡️ Responsável por somar o valor total que há no carrinho (quantidade * valor de cada item).
  
- <b>GET</b> (/ms-product/product) ➡️ Responsável por mostrar todos os produtos cadastrados, bem como o valor do produto e quantidade em estoque.

# Considerações finais

Graças a esse projeto, aprendi muito e pude desenvolver conhecimentos sobre a comunicação síncrona entre microserviços, uso do IntelliJ e Maven, POO, Java 8 (Streams, Lambda)

Vou ficar feliz em receber alguma mensagem com feedbacks sobre o projeto.
Se você perceber que errei em alguma coisa, que poderia melhorar em determinadas partes do código, por favor me manda uma mensagem, seria ótimo pro meu aprendizado!
