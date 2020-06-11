## Desafio SRE

### Problema
Você acaba de ser contratado pela Z-Tech para cuidar de um projeto de migração de uma plataforma Web. O projeto consiste em migrar todos os recursos (banco de dados, servidor de aplicação, sistemas de cache, conteúdos estáticos, DNS e outros) de um infra-estrutura terceira para a AWS. O principal motivo dessa migração se deve a nova quantidade de acesso esperados. A Z-Tech vem escalado fortemente suas operações nos últimos meses e por conta disso, é esperado uma aumento de tráfego de até 30x. Essa quantidade de acesso é infrequente, possuindo momentos de pico fortes e momentos onde o tráfego é menor.

Essa plataforma Web possui uma arquitetura muito simples. Um servidor de web, (Nginx) em conjunto com um interpretador de código (PHP) que é responsável por servir o conteúdo estático e dinâmico. Para armazenamento é utilizado um banco de dados relacional MySQL. Um dos problemas de performance que existe atualmente nessa solução é que todas as sessões são armazenadas em disco. Em momentos de pico, o disco fica muito utilizado degradando a performance do site. Além disso, essa infraestrutura não é escalável horizontalmente. Outro problema recorrente é quanto ao tempo de carregamento das imagens. A plataforma costuma servir imagens de até 1MB e como seus servidores ficam armazenados na Virginia, perde-se muito tempo com a latência/tempo de download dessas imagens.

### Sua Missão 
A nova conta AWS, em que os recursos serão alocados está totalmente vazia, sem nenhum recurso, ou seja, não existe infraestrutura básica para subir a aplicação. Lembre-se de requisitos básico  de segurança (ex: não deixar o banco de dados acessível via internet) ao modelar essa nova infraestrutura. 

Essa infraestrutura da plataforma deve ser elástica e escalável horizontalmente. Nessa aplicação uma das pastas (pasta com imagens de tamanho superior a 1MB) que é servida possui 30Gb.  Devido ao seu tamanho, essa pasta não pode ser copiada para as novas instâncias/pods quando a infraestrutura escalar. Além disso, lembre-se do problema que ocorria com as sessões armazenadas em disco.

### Entregáveis
Sua missão é propor uma arquitetura utilizando componentes da AWS que atendam os requisitos acima citados. Seus entregáveis devem ser:
1. Um diagrama AWS mostrando sua arquitetura. Recomendamos usar: https://cloudcraft.co/ 
2. Um ou mais templates (IaC - infrastructure as a code) da sua infra-estrutura feito em CloudFormation ou Terraform.



