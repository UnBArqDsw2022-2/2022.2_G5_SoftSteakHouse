## Visão de Implementação

A visão de implementação é responsável por descrever como os artefatos de desenvolvimento estão organizados no sistema de arquivos. Os elementos são arquivos e diretórios. Isto inclui os artefatos de desenvolvimento e os de implantação.

## Organização de pastas Front-End

Nossos artefatos estão organizados dentro da estrutura src que faz referencia a source. Esse diretório é dividido em quatro camadas que possuem sua propria resposabilidade, sendo elas: assets que é responsavel por guardar todas as imagens, svgs e componentes reutilizados, context tem como resposábilidade o gerenciamento de variáveis e funcões que precisam ser utilizadas em diversas paginas do sistema, já os hooks guarda as funções base de comunicação com o back-end, o diretório provider que exporta os componentes "pai" para que possamos utilizar de suas funções e por ultimo, o diretório pages que é onde as telas ficam, para cada tela existem um diretório com um arquivo tsx e um css correspondente. 

Os arquivos de configuração do projeto junto ao arquivo de rotas podem ser encontrados na raiz do projeto, no "guarda-chuva" do diretório src.

![Diagrama de implementação](../../assets/Diagrama_implementacao.png)   
 Figura 1: Diagrama de implementacao. Autor: Marcos Felipe


## Histórico de Versão
|Data| Versão | Descrição |Autor | Revisor|
|----|--------|-----------|------|--------|
|29/01/23| 1.0.0| Elaboração da visão de implementação | Marcos Felipe| -|