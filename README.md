# Estudando Efeitos de Borda em Métricas de Redes Viárias

Este repositório contém os dados e o código associados ao Trabalho de Conclusão de Curso (TCC) de Brenddon Érick Andrade de Oliveira, apresentado ao Departamento de Física da Universidade Federal Fluminense (UFF) como requisito parcial para a obtenção do grau de Bacharel em Física.

## Resumo

Diferentes trabalhos aplicam a teoria de redes complexas em redes viárias, utilizando-a como fundamentação para gestão de instalações, planejamento de serviços e engenharia de transporte. As métricas de centralidade têm como objetivo mensurar o impacto que um nó exerce sobre o funcionamento da rede. Este trabalho investiga o comportamento das métricas de redes quando submetidas ao efeito de borda, visando compreender e mensurar perdas de informação ao realizar um recorte na rede espacial.

Os recortes espaciais das redes viárias deste estudo são feitos utilizando a ferramenta OSMnx. Após a extração, aplicamos as medidas investigadas e realizamos incrementos de distância, implementando uma vizinhança cujo tamanho varia com as distâncias incrementadas. A comparação dos dados obtidos das medidas antes e após as implementações de vizinhança são produzidas através do RMSE e por diferenças diretas, expondo o quanto a rede integral está sendo afetada e quais conexões estão sofrendo maior influência desta vizinhança.

## Cidades Analisadas

Este método foi aplicado em seis cidades:
- São Paulo, Brasil
- São José dos Campos, Brasil
- Rio de Janeiro, Brasil
- Brasília, Brasil
- Barcelona, Espanha
- Nova Iorque, EUA

## Resultados

Os resultados obtidos do RMSE demonstram que métricas que independem dos menores caminhos, como grau, comunicabilidade e centralidade de subgrafo, exibem um comportamento estável ao alcançar e manter um limite superior, apresentando variação relativamente baixa com o aumento do tamanho do recorte da rede. Por outro lado, as medidas de eficiência global, vulnerabilidade, closeness e betweenness mostram variações significativas em relação ao tamanho da rede.

## Estrutura do Repositório

- `data/`: Contém os dados brutos utilizados nas análises.
- `scripts/`: Contém os scripts utilizados para a extração e análise dos dados.
- `results/`: Contém os resultados das análises, incluindo gráficos e tabelas.
- `figures/`: Contém as figuras geradas para a apresentação dos resultados.

## Ferramentas Utilizadas

- **Python**: Linguagem de programação utilizada para a análise dos dados.
- **OSMnx**: Ferramenta utilizada para a extração das redes viárias.
- **RMSE (Root Mean Square Error)**: Método utilizado para comparar os dados antes e depois das implementações de vizinhança.

## Como Reproduzir as Análises

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu_usuario/seu_repositorio.git
    cd seu_repositorio
    ```

2. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

3. Execute os scripts de análise:
    ```bash
    python scripts/analyze_networks.py
    ```

## Autores

- **Brenddon Érick Andrade de Oliveira** - [brenddonandrade@gmail.com](mailto:brenddonandrade@gmail.com)

## Orientadores

- **Prof. Thadeu Josino Pereira Penna, D.Sc.**
- **Prof. Leonardo Bacelar Lima Santos, D.Sc.**
- **Pesq. Giovanni Guarnieri Soares, M.Sc.**

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Agradecimentos

Gostaria de expressar minha profunda gratidão a todas as pessoas e instituições que contribuíram para a realização deste trabalho. Agradecimentos especiais ao meu orientador, coorientadores, minha família, minha noiva Pâmela, e aos meus cachorros por todo o apoio durante este projeto.

