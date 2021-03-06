## **Metodologia da análise de dados da reportagem ["Eleições 2020: candidatos têm mais de R$ 175 milhões em multas ambientais"](https://apublica.org/2020/11/eleicoes-2020-candidatos-tem-mais-de-r-175-milhoes-em-multas-ambientais)**

### 1) Download e limpeza dos dados de multas aplicadas pelo Ibama

* Foram exportadas, no dia 19 de outubro, as planilhas com a relação de multas aplicadas pelo Ibama em todas as unidades federativas (UF);
* Unimos as planilhas de multas das 27 UFs e filtramos as entradas de multas aplicadas no período de janeiro de 2011 a outubro de 2020;
* Retiramos da lista as multas com os status débito: “Baixado – Defesa deferida”; “Baixado – Recurso de ofício indeferido”; “Baixado – Recurso deferido”; “Baixado c/base na Lei 9.873/99 (Prescrito)”; “Baixado por determinação judicial”; “Baixado por prescrição intercorrente durante anál. Jurídica”; “Cancelado; Cancelado na homologação (AI sem defesa)”; “Substituição de multa por advertência”; “Substituído na homologação por outro”.
* Excluímos os registros duplicados;
* A relação final contou com 138.835 multas, que podem ser vistas na [planilha 1](https://github.com/apublica/candidatos-multados/blob/main/Planilha%201%20-%20Multas%20filtradas%20(19-10)%20-%20MULTAS.zip).

### 2) Download e limpeza dos dados de candidatos

* No dia 9 de novembro, baixamos a relação de candidatos nas eleições municipais de 2020 do Repositório de Dados Eleitorais;
* Na planilha de candidatos, filtramos as candidaturas com a situação “apto” e, em seguida, aquelas com detalhamento da situação “deferido” ou “deferido com recurso”. A relação final considerou 525.148 candidaturas ([planilha 2](https://github.com/apublica/candidatos-multados/blob/main/Planilha%202-%20candidaturas%20analisadas.zip)). 

### 3) Cruzamento entre os dados de multas e de candidaturas para identificar os candidatos multados

* Verificamos os CPFs de candidatos que aparecem nas multas ambientais. Filtramos esses valores e retiramos as multas vinculadas aos CPFs e CNPJs que não estão na planilha dos candidatos;
* Os nomes levantados e as multas vinculadas aos seus CPFs podem ser vistos na [planilha 3](https://github.com/apublica/candidatos-multados/blob/main/Planilha%203%20-%20candidatos%20multados.xlsx).
