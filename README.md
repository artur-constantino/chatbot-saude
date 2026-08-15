# 🩺 Bússola da Saúde — Chatbot de Especialidades Médicas

Chatbot simples que ajuda o usuário a descobrir qual especialidade médica procurar
com base nos sintomas descritos. Feito com **HTML, CSS e JavaScript puro**, sem
nenhuma API externa ou back-end — roda inteiramente no navegador.

## 🔗 Acesso
👉 https://artur-constantino.github.io/chatbot-saude/

## 💡 Como funciona
O usuário digita um sintoma (ex: "dor no peito", "dor de cabeça") ou clica em um
dos botões de sugestão. O chatbot compara o texto com uma base de palavras-chave
e indica a especialidade médica mais provável (Cardiologia, Dermatologia,
Ortopedia, Pediatria, Ginecologia, Urologia, Psiquiatria, Oftalmologia,
Otorrinolaringologia, Gastroenterologia, Neurologia, Endocrinologia ou
Pneumologia).

Depois de identificar a especialidade, o chatbot faz uma chamada assíncrona
(`fetch`) para a **API pública da Wikipédia**
([REST API](https://pt.wikipedia.org/api/rest_v1/)) e busca um resumo real
sobre aquela especialidade médica, exibindo o resultado na conversa. Enquanto
a requisição acontece, uma bolha de "Buscando mais informações..." é exibida
para indicar o carregamento assíncrono.

## 🛠️ Tecnologias
- HTML5
- CSS3
- JavaScript (vanilla, sem frameworks)
- Consumo de API externa via `fetch()` — [Wikipedia REST API](https://pt.wikipedia.org/api/rest_v1/) (pública, gratuita, sem necessidade de chave)

## 🚀 Como rodar localmente
Basta abrir o arquivo `index.html` no navegador. Não precisa instalar nada.

## ⚠️ Aviso
Este projeto tem fins **educacionais e de portfólio**. Ele não substitui uma
consulta médica real nem oferece diagnóstico. Os resumos exibidos vêm
diretamente da Wikipédia e não são revisados por profissionais de saúde.

## 📌 Próximos passos (ideias de melhoria)
- Adicionar mais especialidades e sintomas
- Salvar histórico da conversa
- Tornar o chatbot mais "inteligente" com correspondência aproximada de texto
