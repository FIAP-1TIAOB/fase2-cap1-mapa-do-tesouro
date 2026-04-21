# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# FarmTech Solutions - Sistema de Irrigação Inteligente (Fase 2)

## Grupo 33

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/company/inova-fusca">Milton Akira Fukuhara</a>
- <a href="https://www.linkedin.com/company/inova-fusca">Samyr de Souza Pereira</a>
- <a href="https://www.linkedin.com/company/inova-fusca">ANTONIO FILIPE DE SOUZA BRANCO</a> 
- <a href="https://www.linkedin.com/company/inova-fusca">Albert Oliveira Ribeiro</a> 
- <a href="https://www.linkedin.com/in/vinicius-adati/">Vinicius Seiti Adati</a>

## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://www.linkedin.com/company/inova-fusca">Sabrina Otoni</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/company/inova-fusca">André Godoi Chiovato</a>
## 📜 Descrição

Este projeto de automação agrícola foi desenvolvido para a Startup **FarmTech Solutions**, visando otimizar o uso de recursos hídricos através do monitoramento em tempo real de sensores e atuadores acoplados a um microcontrolador ESP32.

O sistema monitora a umidade do solo (simulada via sensor DHT22), o pH da terra (simulado via LDR) e a presença de nutrientes essenciais NPK (Nitrogênio, Fósforo e Potássio, simulados via push buttons verdes). A inteligência do sistema garante a **Fertirrigação Inteligente** para a cultura da Soja: a bomba d'água (representada por um Módulo Relé) só é ativada se o solo estiver seco (umidade inferior a 40%), se o pH for adequado para a planta (5.5 a 7.5) ou se houver adição de adubo para ser dissolvido e corrigir o solo.

**Programa Ir Além (Opcional 1):** Adicionalmente, desenvolvemos a integração com uma API meteorológica (Python) simulada via Monitor Serial. Caso o sistema receba o caractere 'C' (Chuva), a irrigação é suspensa preventivamente para evitar desperdícios. Ao receber 'S' (Seco), o funcionamento normal é retomado.

**Demonstração em Vídeo:** [Insira o Link do seu Vídeo do YouTube Aqui]

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>.github</b>: Nesta pasta ficarão os arquivos de configuração específicos do GitHub que ajudam a gerenciar e automatizar processos no repositório.
- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens (ex: `circuito.png`).
- <b>config</b>: Posicione aqui arquivos de configuração que são usados para definir parâmetros e ajustes do projeto.
- <b>document</b>: aqui estão todos os documentos do projeto que as atividades poderão pedir. Na subpasta "other", adicione documentos complementares e menos importantes.
- <b>scripts</b>: Posicione aqui scripts auxiliares para tarefas específicas do seu projeto. Exemplo: deploy, migrações de banco de dados, backups.
- <b>src</b>: Todo o código fonte criado para o desenvolvimento do projeto ao longo das 7 fases (ex: `sketch.ino` e `diagram.json`).
- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🔧 Como executar o código

Este projeto foi desenvolvido utilizando o simulador Wokwi para dispositivos IoT (ESP32). Siga os passos abaixo para testar a solução em sua máquina:

1. Acesse a plataforma [Wokwi](https://wokwi.com/).
2. Crie um novo projeto em branco para o microcontrolador **ESP32**.
3. Acesse a pasta `src` deste repositório no GitHub.
4. Copie todo o conteúdo do arquivo `sketch.ino` e cole na aba de código principal do simulador.
5. Substitua o conteúdo do arquivo `diagram.json` do Wokwi pelo nosso arquivo `diagram.json` (isso montará o circuito e conectará os sensores automaticamente).
6. Clique no botão verde de Play para iniciar a simulação.
7. **Para testar a Previsão do Tempo (Ir Além):** Clique na aba do Monitor Serial do Wokwi, digite `C` e aperte Enter para simular chuva (a bomba bloqueia), ou digite `S` e aperte Enter para tempo seco (a bomba é liberada).

## 🗃 Histórico de lançamentos

* 0.1.0 - 20/04/2026
    * Lançamento da Fase 2: Circuito ESP32, Lógica NPK de Fertirrigação e Integração Serial (Ir Além).

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
