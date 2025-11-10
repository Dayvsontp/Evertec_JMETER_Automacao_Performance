![poster](https://github.com/Dayvsontp/newman_serverest/blob/master/Postman/jmeter-tutorial.png)

## 🤘 Sobre

Repositório do projeto de testes automatizados de performance, realizado no site "https://www.blazedemo.com", construído com Jmeter! O Jmeter é uma ferramenta poderosa que realiza alguns tipos de testes voltado a performance, este projeto foi realizado uma automação de testes de carga e de pico em sistema web/api.

## 💻 Tecnologias e Requisitos
- API Rest
- Jmeter


## 🤖 Qual a estrutura?

```
1. Plano de Teste
2. Servidor HTTP Proxy
3. Thread Group (Cenário de Teste)
  - Requisição GET index.php
  - Requisição POST reserve.php-141
  - Requisição POST purchase.php-154
  - Requisição POST confirmation.php-161
4. Record and Play
  - Controlador de Gravação     //este projeto foi realizado via gravação/navegação.
5. Listeners
  - jp@gc - Throughput Shaping Timer
  - Aggregate Report
```

## 🤖 Como executar

1. Clonar o repositório ou fork do projeto
```
Após instalação do apache-jmeter, quando importar o projeto, parametrizar usuarios e Ramp-up, clicar no play
```

2. Executar testes em Carga ou Pico
```
Plugin jp@gc - Throughput Shaping Timer deve ser instalado, para controlar as requisições pelo Start RPS/ End RPS / Duration, sec
Foi criada linhas para picos e para cargas, exemplo:  Start RPS = 250, End RPS = 500, Duration = 10s para um teste de pico
```

3. Executar e ver o relatório dos testes
```
Execução via CLI
ex:
C:\Teste_JMETER>C:\apache-jmeter-5.6.3\bin\jmeter.bat -n -t consulta_cep.jmx -l resultado.jtl -e -o myDashboard
Relatorio e arquivo .jtl na pasta "myDashboard"
```

<hr>
