# <h1> DevOps </h1>

<h5>DevOps é a automação dos processos de desenvolvimento e infraestrutura. DevSecOps é a prática de integrar testes de segurança em todas as etapas do processo de desenvolvimento de software, denominada assim quando a segurança é prioridade. A cultura DevOps utiliza várias tecnologia e ferramentas que ajudam a operar e desenvolver aplicativos de modo rápido e confiável. DevSecOps traz uma transformação cultural que torna a segurança uma responsabilidade compartilhada por todos que estão construindo o software. <br> </h5>
<h5>Em uma cultura DevOps, experimentamos, encontramos problemas, avisamos a tempo e ajustamos, logo, crie-se uma cultura de experimentação, colaboração e autoatendimento, construindo times autossuficientes e autônomos. Com isso, trabalhamos para errar rápido e corrigir rápido.</h5>


<h1>Conceitos da cultura DevOps</h1>
<h5>Explicação de forma simples com as tecnologias que uso no dia a dia para consulta rápida.</h5>

<img src="https://miro.medium.com/max/1400/1*O76HIkmAb_ackQ94hUHMPw.png"> </img>

<h2>Etapas:</h2>
<h5>
<li>Plan:  Metodologias Ágeis/Jira;
<br><li>Code: Codificação;
<br><li>Build/Test: CI (Continuous Integration);
<br><li>Release: Gitflow;
<br><li>Deploy: CD (Continuous Delivery e Continuous Deployment, onde Continuous Delivery requer aprovação para Deploy e Continuous Deployment é automático);
<br><li>Operate: Produção/Usuário Final.
</h5>


<h2>Conceitos:</h2>
<h3>CI/CD:</h3> 
<h5> Build, Test e Deploy da aplicação, sendo Docker para Build e Test, e Kubernetes para Deploy.
<br><li>Pipeline - Passos:
<br>1. Build da aplicação;
<br>2. Teste da aplicação;
<br>3. Build da imagem da aplicação com Docker;
<br>4. Upload da imagem da aplicação com Docker;
<br>5. Deploy da aplicação no Kubernetes com Helm.
</h5>
<img align="center" alt="Java" height="300" width="700" src="https://media.licdn.com/dms/image/C5112AQGN4vNFRhAZIA/article-cover_image-shrink_600_2000/0/1561044324742?e=2147483647&v=beta&t=6ZXnwkmoNcroRad2lHMtWNyt43vQnV2aL42xcfJpFZI"> </img> <br>


<h3>Manifestos do Kubernetes:</h3>
<h5>
Um arquivo de manifesto, ou especificação de pod, do Kubernetes compreende instruções em um arquivo yaml ou json que especificam como implantar um aplicativo em um cluster do Kubernetes. As instruções incluem informações sobre a implantação do Kubernetes, o serviço Kubernetes e outros objetos do Kubernetes a serem criados no cluster.
</h5>

<h3>Liveness e Readiness do Kubernetes:</h3>
<h5>
Todo o ecossistema onde a aplicação é executada precisa receber informações constantes sobre a saúde e a disponibilidade de seus serviços. Essas informações permitem ações como a reposição de um pod com a aplicação comprometida (sem funcionamento de algum dos seus serviços) e a liberação do tráfego de requisições para essa aplicação. <br>
<li>Healthcheck de liveness (aplicação saudável): Valida a infraestrutura do microserviço, cria-se uma rota de validação para verificar se todos os serviços que compoem a infraestrutura do microserviço estão funcionando adequadamente. Utilizado para pedir reposição ao orquestrador caso a infraestrutura da aplicação esteja comprometida.<br>
<li>Healthcheck de readiness (negócio operacional): Valida a dependência de negócio, quando um microserviço depende de outro microserviço para funcionar cria-se uma rota de validação para verificar se o microserviço do qual se tem dependência está funcionando (em pé). Utilizado para o orquestrador saber quando abrir e fechar o tráfego de requisições, sendo que esse tráfego é aberto se o negócio estiver operacional e fechado caso não esteja.
</h5>

<h2>Transformação Cloud Native: </h2>
<h5> Desenvolver/tornar aplicações compatíveis com conceitos cloud native, através de processos e mecanismos integrados ao orquestrador e à ferramentas de observabilidade.</h5> <br> 
</h3> Cloud computing x Cloud Native  </h3>
<h5> Cloud computing é a entrega sob demanda de infraestrutura (hardware/servidores), armazenamento, bancos de dados e todos os tipos de serviços de aplicativos via Internet. Freqüentemente, eles são fornecidos por uma plataforma de serviços em nuvem como Amazon Web Services, Google Cloud ou Microsoft Azure, com preços medidos para que você pague apenas pelos recursos que realmente consome. <br>
Cloud Native é uma arquitetura para montar todos os componentes baseados em nuvem de uma forma otimizada para o ambiente de nuvem. Não é sobre os servidores, mas os serviços. Portanto, Cloud Native também é um destino organizacional: o objetivo atual para empresas que procuram modernizar sua infraestrutura e processo, e até cultura organizacional, escolhendo cuidadosamente as tecnologias de nuvem que melhor se adaptam ao seu caso específico.
<br> Referência: Livro - Cloud Native Transformation
</h5>
