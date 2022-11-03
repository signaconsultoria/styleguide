# Padrão de Pacotes Signa

## O que é um pacote?
Pacote é um diretório contendo arquivos para implantação no ambiente (sistema) do cliente, tanto para evoluções do sistema quanto para correção de problemas.

O pacote deve seguir a estrutura de diretórios abaixo, com os mesmos nomes:

![pacotes-estrutura](https://user-images.githubusercontent.com/5261655/199841242-c037268c-aec5-45d1-a35b-5c16b7d49fd1.png)


00_ROLLBACK
10_AD
20_SC
30_SP
40_DLL
ECARGO
INTEGRACAO
MANUAL
SERVICOS
VERSAO

_Obrigatoriamente, o pacote deve conter um script de VERSAO contendo o avanço de versão da função no SQL e um script de ROLLBACK contendo um comando para ser executado e gerado um backup dos updates a serem realizados no banco, tanto pela VERSAO quanto pela SC (caso possua)._

