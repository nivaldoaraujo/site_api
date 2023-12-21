# Descrição
Um projeto com objetivo de estudos baseado em API rest. A comunicação é síncrona, ou seja, comunicam-se através de requisições HTTP.


# Análise técnica

### Comunicação
Para facilitar a comunicação HTTP Utilizei vários elementos. Entre elas estão: 
- <b>Servidor json</b> ➡️ É um formato de dados leve e de fácil leitura utilizado para troca de informações entre sistemas computacionais. 
- <b>Axios</b> ➡️ axios é que ele é um cliente HTTP baseado em promessas totalmente agnóstico, ou seja, que não depende de frameworks e bibliotecas. Ele é super maleável, podendo ser utilizado do lado do cliente (React, Vue, Svelte, etc) e do lado do backend (express, nest, etc). Então vamos mergulhar um pouco mais fundo e ver o que a gente consegue fazer com ele.
- <b>Git e GitHub</b> ➡️ GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.
- <b>Site Render</b> ➡️ O Render é um novo provedor de hospedagem web e de aplicativos, descrito pelo seu CEO como "o melhor dos dois mundos" comparando fornecedores em nuvem de larga escala, como a AWS, e provedores PaaS (Plataforma como Serviço)
 

### Endpoints

Possui diversos endpoints que podem ser importados para o postman usando o arquivo JSON disponibilizado no repositório. Como o sistema usa <b>Eureka server</b>, todos os endpoints possuem o mesmo localhost (http://localhost:5173)

- <b>GET</b> (/ms-cart/cart) ➡️ Responsável por mostrar todos os itens dentro do carrinho, bem como o valor unitário e quantidade.
  
- <b>POST</b> (/ms-cart/cart) ➡️ Através do body, adiciona um item ao carrinho. Antes é feita a comunicação com o serviço de Produto para verificar a existencia do produto e se há estoque disponível.
  
- <b>GET</b> (/ms-cart/cart/total) ➡️ Responsável por somar o valor total que há no carrinho (quantidade * valor de cada item).
  
- <b>GET</b> (/ms-product/product) ➡️ Responsável por mostrar todos os produtos cadastrados, bem como o valor do produto e quantidade em estoque.

# Considerações finais

Projeto desenvido para auxiliar nos conceitos de API rest e requisições HTTP
