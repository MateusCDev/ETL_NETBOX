# ETL NetBox

Projeto desenvolvido no Google Colab com apoio do Codex para processar informações de infraestrutura e apoiar a criação e interligação de cópias de POPs no NetBox.

## Organização

- [notebooks/ETL_NetBox_v6_3_1.ipynb](notebooks/ETL_NetBox_v6_3_1.ipynb): notebook autônomo do Colab, incluindo o código do processamento e o painel de execução.

## Fluxo

O notebook recebe planilhas e configurações, identifica e valida os dados de um POP e gera relatórios. Quando configurado para acessar o NetBox, pode criar uma cópia isolada e processar interligações confirmadas entre cópias. Os modos disponíveis incluem simulação, aplicação, retomada, interligação e previsão de limpeza. Consulte as instruções no próprio notebook para requisitos, revisão de pendências e limites de cada modo.

## Como usar

1. Abra o [notebook no Google Colab](https://colab.research.google.com/github/MateusCDev/ETL_NETBOX/blob/master/notebooks/ETL_NetBox_v6_3_1.ipynb) ou abra o arquivo pelo menu do Colab.
2. Execute a primeira etapa e forneça as planilhas e configurações solicitadas pelo painel.
3. Comece pelo modo **SIMULAR** e confira os relatórios e pendências antes de usar modos que alteram o NetBox.
4. Para acesso à API, informe a URL HTTPS e o token no ambiente de execução, conforme solicitado pelo notebook.

O notebook é autônomo: seus módulos são extraídos durante a execução. A movimentação para a pasta `notebooks/` não altera sua lógica.

## Dados e credenciais

Não inclua tokens, planilhas operacionais, relatórios ou arquivos de estado no repositório. Revise também saídas e metadados do notebook antes de compartilhá-lo, pois podem conter informações da infraestrutura.
