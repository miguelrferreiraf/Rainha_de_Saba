**Corrigindo problemas com o pip no Jupyter (múltiplas versões do Python)**

---

**Cenário do problema:**

O Jupyter estava acusando erro do tipo `ModuleNotFoundError`, mesmo após instalar corretamente o pacote com o comando `!pip install nome-do-pacote`. Isso ocorre quando o Jupyter está rodando em uma versão do Python diferente daquela onde o pip está instalando os pacotes.

---

**Passo-a-passo para diagnosticar e resolver:**

1. **Verifique onde o pip está instalado**
   
   No Jupyter, execute:

   ```python
   !where pip
   ```

   Isso mostra todas as localizações onde o executável `pip` está presente no sistema. Exemplo:

   ```
   C:\Users\progr\.pyenv\pyenv-win\shims\pip
   C:\Users\progr\.pyenv\pyenv-win\shims\pip.bat
   C:\Users\progr\AppData\Local\Microsoft\WindowsApps\pip.exe
   ```

2. **Descubra qual Python o Jupyter está usando**

   Execute:

   ```python
   import sys
   print(sys.executable)
   ```

   Isso mostra o caminho completo da versão do Python em uso pelo Jupyter. Exemplo:

   ```
   C:\Users\progr\AppData\Local\Programs\Python\Python312\python.exe
   ```

3. **Compare os caminhos**

   Se `pip` não estiver relacionado à pasta da versão de Python usada pelo Jupyter, os pacotes estão sendo instalados no lugar errado.

4. **Use pip corretamente para a versão do Jupyter**

   Para garantir que o pacote seja instalado exatamente na versão que o Jupyter está usando, use:

   ```python
   import sys
   !{sys.executable} -m pip install nome-do-pacote
   ```

   Exemplo:

   ```python
   import sys
   !{sys.executable} -m pip install statsmodels
   ```

5. **Teste novamente o import**

   Após a instalação, tente importar o pacote:

   ```python
   from statsmodels.tsa.seasonal import seasonal_decompose
   ```

   Se não houver erro, a instalação foi bem-sucedida e compatível com o kernel do Jupyter.

---

**Dica final:**

Sempre que estiver em ambientes com várias versões do Python, prefira usar:

```python
!{sys.executable} -m pip install pacote
```

Isso evita conflitos e garante que os pacotes sejam instalados no ambiente correto.

---

**Problema resolvido!**

Esse procedimento também ajuda a resolver outros erros recorrentes, como falhas no uso de bibliotecas financeiras (ex: `yfinance`, `statsmodels`, `ta`, etc) dentro do Jupyter.

