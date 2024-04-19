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
* Estimativa de pose humana: essa tecnologia é 


## Produtos comerciais relacionados e seus segmentos de mercado
## Teste de um produto relacionado
