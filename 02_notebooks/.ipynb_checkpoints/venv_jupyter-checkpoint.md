**Como usar TensorFlow no Jupyter Notebook com Ambiente Virtual (passo-a-passo em PDF)**

---

# Instalar Python 3.10

1. Baixe o instalador do Python 3.10:
   - Link direto: https://www.python.org/ftp/python/3.10.13/python-3.10.13-amd64.exe
2. Instale normalmente.
   - IMPORTANTE: Marque a caixinha **"Add Python to PATH"** durante a instalacao.

# Criar um Ambiente Virtual (venv)

3. Abra o terminal (cmd ou PowerShell).
4. Navegue até a pasta onde você quer trabalhar:
   ```bash
   cd caminho/para/seu/projeto
   ```
5. Crie o ambiente virtual:
   ```bash
   python3.10 -m venv venv
   ```
6. Ative o ambiente:
   - Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - (Se pedir permissão de execução, aceite.)

# Instalar Bibliotecas

7. Instale TensorFlow e outras bibliotecas:
   ```bash
   pip install tensorflow scikit-learn pandas numpy jupyter ipykernel
   ```

# Adicionar o Ambiente Virtual como Kernel no Jupyter

8. Registre o ambiente no Jupyter:
   ```bash
   python -m ipykernel install --user --name=venv --display-name "Python (venv)"
   ```
   - `--name=venv`: nome interno.
   - `--display-name`: nome que vai aparecer no Jupyter.

# Usar no Jupyter Notebook

9. Abra o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
10. Na hora de abrir ou criar um Notebook novo, selecione o kernel "Python (venv)".


# Resumo Visual

- Instalar Python 3.10
- Criar e ativar venv
- Instalar bibliotecas (TensorFlow etc.)
- Adicionar o ambiente no Jupyter como kernel
- Selecionar o kernel "Python (venv)" no seu projeto

---

Assim você usa TensorFlow no Jupyter normalmente, sem precisar ficar trocando instalações ou complicando seu sistema! 🚀

Se quiser, posso também gerar uma versão com imagens passo-a-passo.

