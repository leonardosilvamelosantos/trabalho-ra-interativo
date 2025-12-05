Aplicação de Realidade Aumentada (RA) com AR.js e A-Frame
Descrição do Projeto

Este projeto implementa uma aplicação de Realidade Aumentada (RA) utilizando tecnologias web acessíveis diretamente pelo celular, sem necessidade de instalar aplicativos adicionais.
A partir da leitura do marcador Hiro, a aplicação exibe um modelo 3D da Arena Corinthians, permitindo que o usuário visualize o estádio por cima, pelas laterais ou caminhando ao redor, como se estivesse observando uma maquete física.

O objetivo da atividade era implementar uma aplicação baseada em uma tecnologia de referência e propor alguma alteração de interatividade.
O projeto demonstra como desenvolvedores, empresas e vendedores podem utilizar RA Web para visualizar produtos, casas, carros, estruturas e outros objetos tridimensionais de maneira simples, rápida e funcional.

Tecnologias Utilizadas

A-Frame
Framework para criação de cenas 3D e experiências VR/AR em HTML, facilitando a manipulação de modelos e animações.

AR.js
Implementação utilizada como referência.
Fornece reconhecimento de marcadores, rastreamento e suporte completo a RA via navegador mobile.

Modelo 3D (GLB)
Arquivo utilizado: arena_corinthians_itaquera.glb
Representa a Arena Corinthians em três dimensões.

HTML e JavaScript
Responsáveis pela estrutura da página, botões interativos e controle de rotação do modelo.

Implementação de Referência e Alterações Realizadas

A aplicação foi baseada no exemplo padrão de AR.js que utiliza um cubo simples sobre o marcador Hiro.
A partir desse modelo básico, foram feitas as seguintes modificações:

Alteração 1 – Substituição do objeto 3D
O cubo padrão foi substituído pelo modelo da Arena Corinthians (arena_corinthians_itaquera.glb).

Alteração 2 – Interatividade (botões de rotação)
Foram criados dois botões:
▶ Girar — inicia rotação do modelo
⏹ Parar — interrompe a rotação
A rotação foi corrigida para ocorrer apenas no eixo Y, garantindo comportamento natural e sem deformações.

Alteração 3 – Modo AR otimizado para uso no celular
A aplicação foi ajustada para funcionar no navegador mobile simulando a experiência de se movimentar em torno de um objeto físico, como se fosse observado por óculos de RA.

Dificuldades Encontradas

Controle da rotação inicial
Modelos importados em GLB geralmente vêm com rotações internas diferentes.
Foi necessário ajustar o modelo dentro de um container para corrigir o eixo Y e evitar que o objeto inclinasse.

Ajuste de escala
O modelo original estava grande demais.
Foi aplicada uma escala compatível com o tamanho desejado no marcador.

Comportamento da câmera
Em AR.js a posição da câmera se move em relação ao marcador.
Ajustar para que vistas superior e laterais fossem naturais exigiu testes reais com o celular.

Arquivos Inclusos no Projeto

index.html
arena_corinthians_itaquera.glb
print_da_aplicacao.png
README.md
Vídeo de demonstração (link)

Demonstração em Vídeo

https://youtu.be/DdV4fQzbXBI?si=-70l4frq7T7lPxXr

Teste Online da Aplicação

O projeto pode ser testado diretamente pelo navegador:
https://leonardosilvamelosantos.github.io/trabalho-ra-interativo/

Instruções de Uso

Abra o link ou execute o arquivo index.html em um servidor local.

Aponte a câmera para o marcador Hiro.

O modelo 3D da Arena Corinthians será carregado.

Utilize os botões de controle:
▶ Girar — inicia rotação do modelo
⏹ Parar — interrompe a rotação
