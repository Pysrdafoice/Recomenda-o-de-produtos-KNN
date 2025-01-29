# Sistema de Recomendação de Produtos com ResNet50

Este projeto implementa um sistema de recomendação de produtos baseado em imagens, utilizando a arquitetura ResNet50 para extração de características e o algoritmo de vizinhos mais próximos (KNN) para encontrar itens similares.

## 📌 Requisitos
- Python 3.x
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn

## 📂 Estrutura do Projeto
```
📁 ecommerce-products
 ├── 📁 categoria1
 │   ├── imagem1.jpg
 │   ├── imagem2.jpg
 │   └── ...
 ├── 📁 categoria2
 │   ├── imagem1.jpg
 │   ├── imagem2.jpg
 │   └── ...
 ├── 📄 main.py
 ├── 📄 requirements.txt
 └── 📄 README.md
```

## 🚀 Como Funciona
1. **Carregamento do modelo**: Utiliza a ResNet50 pré-treinada sem a camada superior para extrair características das imagens.
2. **Extração de características**: Cada imagem é processada e convertida em um vetor de características.
3. **Armazenamento de dados**: As características extraídas de todas as imagens do dataset são armazenadas em um dicionário.
4. **Recomendação**: Dado uma nova imagem, o sistema busca as imagens mais semelhantes em diferentes categorias, retornando recomendações.

## 🛠️ Instalação
Clone o repositório e instale as dependências:
```bash
pip install -r requirements.txt
```

## 📌 Uso
Execute o script principal para gerar recomendações:
```bash
python main.py
```
O sistema irá processar as imagens no diretório `/content/ecommerce products` e exibir recomendações para um item específico.

## 📷 Exemplo de Saída
Para uma camisa como entrada, o sistema pode recomendar:
- 1 calça
- 1 bermuda
- 1 TV
- 1 jaqueta

  **uma observação o banco de dados usados não possuia nem TV e em calça**

As imagens recomendadas serão exibidas lado a lado para fácil visualização.

## 📜 Licença
Este projeto é distribuído sob a licença MIT. Sinta-se à vontade para contribuir e modificar conforme necessário!

## 🤝 Contribuições
Sinta-se livre para abrir issues e enviar pull requests para melhorias no código!

---
**Autor:** Anderson da cruz gomes




