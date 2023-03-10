# <h1> Cultura DevOps </h1>

<h5>Conceitos da cultura DevOps explicados de forma simples com as tecnologias que uso no dia a dia para consulta rápida.</h5>

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
<li>Healthcheck de readiness (negócio operacional): Valida a dependência de negócio, quando um microserviço depende de outro microserviço para funcionar cria-se uma rota de validação para verificar se o microserviço do qual se tem dependência está funcionando (em pé). Utilizado para abrir e fechar o tráfego de requisições, sendo que esse tráfego é aberto se o negócio estiver operacional e fechado caso não esteja.
</h5>
