# Relatório sobre tarefas de processamento de imagem - Allan Casado
## Introdução

De acordo com o artigo "What is Computer Vision and Machine Vision? A Guide for Beginners", da empresa Roboflow: "Visão computacional é a capacidade de um computador ver e entender o mundo físico. Com visão computacional, os computadores podem aprender a identificar, reconhecer e localizar a posição de objetos."

Assim, dentro desse grande campo, utilizam-se técnicas avançadas para processar e analisar imagens e vídeos, o que possibilita a execução de uma série de tarefas cruciais, como detecção de objetos, classificação de imagens, segmentação semântica, reconhecimento facial, rastreamento de objetos, reconstrução 3D, detecção de pontos-chave, análise de movimento, restauração de imagens e síntese de imagens. Cada uma dessas tarefas ajuda em aplicações variadas que vão desde a automação industrial até a segurança, saúde e entretenimento.

Este relatório se concentrará especificamente em duas dessas técnicas: detecção de objetos e detecção de pontos-chave, que serão exploradas em maior detalhe nas seções subsequentes. Além de descrever essas tarefas, também serão discutidas algumas de suas aplicações práticas e alguns produtos comerciais que as implementam, destacando como são empregadas no mundo real.

## Descrição das tarefas selecionadas e possíveis aplicações

### Detecção de Objetos

A detecção de objetos é uma técnica de visão computacional usada para localizar instâncias de objetos em imagens ou vídeos. Assim como os humanos, que podem localizar e reconhecer objetos em imagens rapidamente, o objetivo dessa tarefa é replicar essa capacidade em uma máquina. Repara-se que tratando-se de detecção de objetos, não basta apenas reconhecer que determinado objeto está presente em uma imagem ou vídeo, mas também ser capaz de apontar aonde que ele está localizado, o que é geralmente realizado desenhando uma caixa delimitadora ao redor de cada objeto detectado

Dentre alguns dos principais desafios para o uso preciso dessa técnica, pode-se citar:
* Diversidade e variação de classes: quando precisa-se reconhecer uma quantidade grande de diferentes objetos, tem-se como necessidade um conjunto de dados rotulados bem extenso e amplo, o que exige um grande trabalho humano, além da necessidade de utilizar algoritmos bem robustos para conseguir uma boa capacidade de generalização, o que é computacionalmente custoso.
* Variações de iluminação e condições ambientes: ao lidar com aplicações ao ar livre, como veículos autônomos, mudanças na iluminação, sombras e condições meteorológicas podem atrapalhar o modelo.
* Sobreposições: muitas vezes os objetos se sobrepõem ou são ocultados por outros, o que pode dificultar a identificação e a localização correta dos objetos de interesse.

As aplicações desse tipo de tarefa são  variadas e abrangentes. Algumas das principais incluem:
* Veículos autônomos: a detecção de objetos é essencial para o funcionamento desses veículos, pois eles precisam o tempo todo identificar pedestres, outros veículos, semáforos, árvores, animais e outros obstáculos.
* Sistemas de segurança inteligentes: nesses sistemas, utiliza-se a detecção de objetos para identificar pessoas, veículos ou outros atores de interesse, a fim de garantir um monitoramento eficaz de qualquer área, facilitando a identificação de atividades suspeitas.
* Análise de imagens médicas: na medicina, essa técnica é utilizada para identificar características específicas em imagens médicas, como tumores, fraturas ou outras anomalias. O artigo citado na introdução, da empresa Roboflow, apresenta um caso de uso específico desse contexto médico, em que faz-se uma avaliação do risco de câncer, por meio da detecção visual de células vermelhas do sangue, células brancas do sangue e plaquetas.


### Detecção de pontos chave

A detecção de pontos chave é uma tarefa de visão computacional que tem como essência a identificação e utilização de pontos específicos em imagens. A deteccção desses pontos mais importantes permite que os computadores não apenas "vejam", mas também compreendam as relações entre pontos em uma imagem ou vídeo.

Um "ponto chave" em uma imagem pode ser definido com base em três aspectos
* Unicidade: ele deve ser único e facilmente distinguível de outro ponto, seja pela cor, intensidade ou algum outro fator.
* Invariância: ele deve ser invariante em relação a rotações, mudanças na escala, iluminação...
* Repetibilidade: um ponto chave deve ser detectável de forma confiável em diferentes instâncias do mesmo objeto ou cena.

Dessa maneira, essa técnica pode ser aplicada em diferentes casos de uso, como por exemplo:
* Estimativa de pose humana: busca-se, com o uso dessa técnica, identificar "keypoints" associados a pessoas. Isso pode ser aplicado em um contexto de prática de exercício físico, para monitorar a postura e movimentos durante atividades físicas.
* Estimativa da pose da mão: esta abordagem foca em definir pontos-chave nas mãos humanas, o que pode ser utilizado, por exemplo, em interfaces de usuário onde o controle se dá através de gestos, como sistemas de realidade virtual ou dispositivos inteligentes.
* Keypoints de face: nesse caso de uso tem-se o objetivo de identificar "keypoints" de faces humanas, o que em um contexto de reconhecimento facial é essencial para identificar características individuais no rosto, facilitando o reconhecimento de identidade.

## Produtos comerciais relacionados e seus segmentos de mercado

###  Google Cloud Visual Inspection AI

O Visual Inspection AI é uma solução de inteligência artificial desenvolvida para automatizar e otimizar a inspeção visual em processos de produção, facilitando a inspeção de qualidade de produtos fabricados. Por meio da utilização de técnicas de detecção de objetos, essa ferramenta permite que as empresas identifiquem defeitos com precisão em diferentes tipos de itens fabricados em diferentes indústrias.

Esse produto é direcionado principalmente para o setor de manufatura industrial, abrangendo uma variedade de indústrias nesse setor, como a automotiva, eletrônicos e semicondutores. Os casos de uso incluem desde o inspecionamento de soldas em chassis de veículos até a análise de defeitos em placas de circuito impresso (PCBs) e wafers de silício.

Essa ferramenta permite que as empresas treinem e implantem rapidamente modelos de IA para inspeção visual sem exigir conhecimento técnico aprofundado e com poucas imagens rotuladas, a partir de uma interface do usuário simples e intuitiva.

Mais informações em https://cloud.google.com/solutions/visual-inspection-ai#all-features

### Tensorflow Pose Estimation

O Tensorflow Pose Estimation é um produto oferecido pelo Tensorflow que abrange a implementação de modelos de visão computacional que utilizam da técnica de detecção de pontos chave para estimar as posições das principais articulações do corpo humano em imagens ou vídeos.

Esses modelos podem ser utilizados em uma variedade de segmentos de mercado, os quais incluem:
* Fitness e Esportes: para análise e melhoria da técnica de exercícios e movimentos esportivos.
* Segurança e Vigilância: detecção de comportamentos ou atividades anômalas em ambientes monitorados.
* Saúde e Reabilitação: monitoramento de movimentos para fisioterapia e reabilitação.

O produto utiliza modelos como MoveNet e PoseNet para analisar imagens e vídeos, identificando pontos-chave do corpo humano, como cotovelos, joelhos e ombros. Como input o modelo recebs a entrada de imagem e produz uma saída tabular dos pontos-chave detectados, com suas respectivas pontuações de confiança, que indicam a precisão da detecção.

Desse modo, esse produto pode ser integrado em diferentes contextos e em diferentes plataformas, incluindo dispositivos móveis e aplicações web, por meio do Tensorflow Lite (uma versão otimizada do Tensorflow para dispositivos móveis) e do Tensorflow JS.


## Teste de um produto relacionado
