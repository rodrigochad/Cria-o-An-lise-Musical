# Criador/Analista Dos Seus Hits Musicais

Este projeto usa aprendizado de máquina para prever o sucesso de uma música com base em seus atributos musicais. Ele também usa o Gemini para interpretar a descrição de uma música fornecida pelo usuário, gerando uma música modelo, e traduzi-la em atributos musicais

## Pré-requisitos

* Python 3.7 ou superior
* Pandas
* Scikit-learn
* Google Generative AI SDK
* Uma conta do Google Cloud com o Gemini habilitado

## Instalação

1. Clone este repositório: `git clone https://github.com/seu_usuario/music-success-predictor.git`
2. Instale as dependências: `pip install -r requirements.txt`
3. Configure sua chave de API do Google Cloud:
    * Crie uma variável de ambiente chamada `SECRET_KEY` com sua chave de API.
    * Ou, você pode substituir `userdata.get("SECRET_KEY")` pelo valor da sua chave de API no código.

## Uso

1. Execute o script: `python music_predictor.py`
2. O script pedirá que você descreva a música que deseja criar.
3. O script usará o Gemini para interpretar sua descrição e gerar valores para os atributos musicais da música.
4. O script usará um modelo de regressão linear para prever o número de streams que a música receberá.
5. O script imprimirá os streams previstos e uma pontuação de sucesso (0-10).

## Dados

O script usa um conjunto de dados de músicas do Spotify para treinar o modelo de regressão linear. O conjunto de dados está localizado no arquivo `new_withC_spotfiy-2023.csv`.

## Modelo

O script usa um modelo de regressão linear para prever o número de streams que uma música receberá. O modelo é treinado nos atributos musicais da música, como BPM, dança, energia, etc.

## Gemini

O script usa o Gemini para interpretar a descrição de uma música fornecida pelo usuário e traduzi-la em atributos musicais. O Gemini é um modelo de linguagem grande que é capaz de entender e gerar linguagem natural.

## Exemplos
Use code with caution.
Markdown
Descreva a música que você deseja criar: música para programadores com acordes nos versos
Use code with caution.
Informações da Música
Característica	Valor	Tradução
bpm	100	Batidas por minuto
mode	Minor	Modo
danceability_%	60	Dançabilidade
valence_%	40	Valência
energy_%	90	Energia
acousticness_%	20	Acusticidade
instrumentalness_%	45	Instrumentalidade
liveness_%	10	Vitalidade
speechiness_%	65	Fala
key	G	Tonalidade
Exemplo de musica
[Intro]
Dm7 Gm7 C7 Fmaj7
Dm7 Gm7 C7 Fmaj7
[Verso 1]
Am7 Dm7
Eu digito linhas sem parar
G7 Cmaj7
Para criar mundos cheios de luz
Fmaj7 Gm7
Meu código, um reflexo da alma
Dm7 Am7
Que anseia por soluções
...
Streams previstos: 0 de views
Pontuação de sucesso (0-10): 0
## Limitações

* O modelo de regressão linear é apenas uma aproximação de como o sucesso de uma música é determinado.
* O Gemini pode não interpretar as descrições dos usuários perfeitamente.
* O conjunto de dados usado para treinar o modelo é limitado.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas ou enviar solicitações pull.

## Licença

Este projeto é licenciado sob a licença MIT.
