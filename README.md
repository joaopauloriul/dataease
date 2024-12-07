<p align="center"><a href="https://dataease.io"><img src="https://dataease.oss-cn-hangzhou.aliyuncs.com/img/dataease-logo.png" alt="DataEase" width="300" /></a></p>
<h3 align="center">人人可用的开源 BI 工具</h3>
<p align="center">
  <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/github/license/dataease/dataease?color=%231890FF" alt="License: GPL v3"></a>
  <a href="https://app.codacy.com/gh/dataease/dataease?utm_source=github.com&utm_medium=referral&utm_content=dataease/dataease&utm_campaign=Badge_Grade_Dashboard"><img src="https://app.codacy.com/project/badge/Grade/da67574fd82b473992781d1386b937ef" alt="Codacy"></a>
  <a href="https://github.com/dataease/dataease"><img src="https://img.shields.io/github/stars/dataease/dataease?color=%231890FF&style=flat-square" alt="GitHub Stars"></a>
  <a href="https://gitee.com/fit2cloud-feizhiyun/DataEase"><img src="https://gitee.com/fit2cloud-feizhiyun/DataEase/badge/star.svg?theme=gvp" alt="Gitee Stars"></a><br>
  [<a href="/README.md">中文(简体)</a>] | [<a href="/README_EN.md">English</a>]
</p>

------------------------------

## O que é o DataEase?  

O DataEase é uma ferramenta de BI open-source projetada para ajudar os usuários a analisar dados rapidamente e obter insights de negócios, permitindo melhorias e otimização de operações. Ele suporta uma ampla variedade de fontes de dados, permitindo a criação de gráficos com uma interface simples de arrastar e soltar e compartilhamento fácil.  

## Vantagens do DataEase:  

-   Open Source: Zero barreiras, aquisição e instalação rápidas, atualizações mensais.  
-   Fácil de Usar: Análises podem ser feitas com cliques do mouse e ações de arrastar e soltar.  
-   Versátil: Suporta instalação em múltiplas plataformas e opções diversificadas de incorporação.  
-   Compartilhamento Seguro: Oferece vários métodos de compartilhamento de dados com segurança.  

## Fontes de Dados Suportadas:  

-   Bancos de Dados OLTP: MySQL, Oracle, SQL Server, PostgreSQL, MariaDB, Db2, TiDB, MongoDB-BI, etc.  
-   Bancos de Dados OLAP: ClickHouse, Apache Doris, Apache Impala, StarRocks, etc.  
-   Armazéns/Dados em Lago: Amazon RedShift, etc.  
-   Arquivos de Dados: Excel, CSV, etc.  
-   APIs de Dados.  

---  

## Início Rápido  

bash  
# Prepare um servidor Linux com pelo menos 2 CPUs e 4GB de RAM, e execute o seguinte script de instalação como root:  

curl -sSL https://dataease.oss-cn-hangzhou.aliyuncs.com/quick_start_v2.sh | bash  

# Usuário: admin  
# Senha: DataEase@123456 

Você também pode implantar rapidamente o DataEase através da [loja de aplicativos do 1Panel](https://dataease.io/docs/v2/installation/1panel_installation/).

Se for para um ambiente de produção, recomendamos utilizar a [instalação offline](https://dataease.io/docs/v2/installation/offline_INSTL_and_UPG/).

Se tiver mais perguntas, você pode consultar a documentação online ou interagir conosco através do fórum.

- [Experiência Online](https://dataease.io/demo.html)
- [Documentação Online](https://dataease.io/docs/)
- [Fórum da Comunidade](https://bbs.fit2cloud.com/c/de/6)
- [Vídeo de Introdução](https://www.bilibili.com/video/BV1Z84y1X7eF/)
- [Mercado de Modelos](https://templates.dataease.cn/)

Exibição da Interface de Usuário (UI)

<table style="border-collapse: collapse; border: 1px solid black;">
  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/8dbed4e1-39f0-4392-aa8c-d1fd83ba42eb" alt="DataEase 工作台"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/7c54cb07-51ef-4bb6-a931-8a95c64c7e11" alt="DataEase 仪表板"   /></td>
  </tr>

  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/ffa79361-a7b3-4486-b14a-f3fd3a28f01a" alt="DataEase 数据源"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/bb28f4e4-636e-4ab0-85c5-1dfbd7a5397e" alt="DataEase 模板中心"   /></td>
  </tr>
</table>

## Tecnologias Utilizadas 

-   Frontend: [Vue.js](https://vuejs.org/), [Element](https://element.eleme.cn/)  
-   Biblioteca de Visualização: [AntV](https://antv.vision/zh)  
-   Backend: [Spring Boot](https://spring.io/projects/spring-boot)  
-   Banco de Dados: [MySQL](https://www.mysql.com/)  
-   Processamento de Dados: [Apache Calcite](https://github.com/apache/calcite/), [Apache SeaTunnel](https://github.com/apache/seatunnel)  
-   Infraestrutura: [Docker](https://www.docker.com/)  


## Outros projetos de destaque da Feizhiyun

- [1Panel](https://github.com/1panel-dev/1panel/) - Painel de gerenciamento de operações de servidores Linux moderno e de código aberto
- [MaxKB](https://github.com/1panel-dev/MaxKB/) - Sistema de perguntas e respostas de conhecimento baseado em LLM (Modelo de Linguagem Grande) e de código aberto
- [JumpServer](https://github.com/jumpserver/jumpserver/) - Bastion host de código aberto amplamente utilizado
- [Halo](https://github.com/halo-dev/halo/) - Ferramenta poderosa e fácil de usar para criação de sites, de código aberto
- [MeterSphere](https://github.com/metersphere/metersphere/) - Ferramenta de teste contínuo de nova geração, de código aberto

## Licença  

Copyright (c) 2014-2024 [FIT2CLOUD](https://fit2cloud.com/), Todos os direitos reservados.  

Licenciado sob a Licença GNU General Public License versão 3 (GPLv3). Você pode obter uma cópia da licença em:  
<https://www.gnu.org/licenses/gpl-3.0.html>  

A menos que exigido por lei aplicável ou acordado por escrito, o software distribuído sob a licença é fornecido "COMO ESTÁ", sem garantias de qualquer tipo. Consulte a licença para mais detalhes sobre direitos e limitações.
