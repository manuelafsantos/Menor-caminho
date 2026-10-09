# Menor-caminho
Esse projeto calcula a menor distância necessária para percorrer um grafo em que as arestas tem peso positivo utilizando o algoritmo de Dijkstra. Foi feito para pessoas que estão aprendendo teoria dos grafos e algoritmos de caminhos mínimos. Ele pode ser utilizado como exemplo para compreender o funcionamento do algoritmo de Dijkstra.

## Demonstração
![a imagem abaixo demonstra o funcionamento do programa](IMAGENS/IMG_0395.jpeg)

## Instalação e pré-requisitos
1. É necessário ter um compilador C++, como o g++. No GitHub Codespaces, abra o terminal e verifique se ele está instalado.
2. Na pasta que contém o arquivo main.cpp, execute "g++ main.cpp -o menor-caminho". Esse comando compila o código e gera o executável menor-caminho. Para iniciar o programa no Linux ou no GitHub Codespaces, execute "./menor-caminho".
3. digite os dados de entrada ou cole o exemplo do tópico "Exemplo de entrada".

## Uso e exemplos
O programa recebe:
* N: índice utilizado para definir o destino, que é o vértice N+1.
* M: quantidade de arestas.
* S e T: vértices conectados por uma aresta.
* B: peso da aresta.

O algoritmo começa no vértice 0 e calcula a menor distância até o vértice N+1. As arestas são adicionadas nos dois sentidos, portanto o grafo é não direcionado.

### Exemplo de entrada
- 2 5
- 0 1 1
- 0 2 3
- 0 3 9
- 1 3 2
- 2 3 2
- Saida: A menor distância do vértice 0 ao vértice 3 é igual a 3, pelo caminho 0-1-3.

## Estrutura do projeto
* README.md: documentação do projeto.
* LICENSE: arquivo com os termos de uso e distribuição.
* main.cpp: código-fonte do programa.
* IMAGENS: pasta com imagens utilizadas na documentação.

## Licença
Este projeto está licenciado sob a [Licença MIT](LICENSE).