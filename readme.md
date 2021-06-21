### Desafio de performance Sicredi
---

## Em refinamento com o time e área de negócio, foi informado que a aplicação terá um pico de 
utilização no quinto dia útil do mês. São esperados 1000 acessos por hora no período da manhã 
e esse pico é atingido em 30 minutos, mantendo-se estável até o final da manhã e reduzindo 
até o final do dia. 
Também foi informado que a aplicação possui duas operações: uma que consulta pelo código 
do CEP e outra que busca pelo endereço. A consulta por CEP terá 60% da volumetria de uso, 
enquanto a consulta por endereço terá 40%.
A documentação e exemplos de utilização da API podem ser obtidas em: https://viacep.com.br

Neste desafio o objetivo é criar um projeto de performance com as seguintes configurações e 
<sub><b> requisitos mínimos:</b></sub>
1. Ramp up de 30 minutos;
2. Steady State de 60 minutos;
3. Think time randômico entre os requests, variando de 100ms a 1000ms;
4. Pacing de 1000 requests por hora durante o período de steady state;
5. Utilizando datapools ou outra forma de geração de dados para uma massa de dados variável 
durante a execução do teste de performance;