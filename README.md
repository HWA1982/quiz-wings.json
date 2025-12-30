# Wings Motorcycle Course - Quiz Database

Este repositório contém a base de dados oficial de questões para o aplicativo **Wings Motorcycle Course**. O objetivo é fornecer um banco de dados estruturado para auxiliar motociclistas no aprendizado de técnicas de pilotagem, manutenção, segurança e legislação.

## 📊 Estrutura dos Dados

O arquivo principal `quiz-wings.json` contém 300 questões no formato JSON. Cada objeto segue a estrutura abaixo:

- **id**: Identificador único da questão.
- **question**: Enunciado da pergunta.
- **options**: Array com 4 alternativas de resposta.
- **correct**: Índice da resposta correta (0 a 3).
- **category**: Categoria do conhecimento (Manutenção, Pilotagem, Segurança, etc).
- **level**: Nível de dificuldade (Iniciante, Intermediário, Avançado).
- **explanation**: Breve explicação pedagógica sobre a resposta correta.

## 🗂️ Categorias Incluídas

O banco de dados cobre os seguintes temas:
* **Pilotagem**: Técnicas de curvas, frenagem e condução urbana/estrada.
* **Segurança**: Uso de EPIs, direção defensiva e primeiros socorros.
* **Manutenção**: Cuidados preventivos e mecânica de emergência.
* **Legislação**: Regras de trânsito e sinalização.
* **Tecnologia**: Sistemas como ABS, Controle de Tração e IMU.
* **Curiosidades**: História e cultura do motociclismo.

## 🚀 Como utilizar

Para consumir estes dados em um projeto JavaScript/React, você pode importar o arquivo diretamente:

```javascript
import quizData from './quiz-wings.json';

// Exemplo de acesso
console.log(quizData[0].question);
