# **Phishing para Captura de Senhas do Facebook no Kali Linux**

Este documento fornece um guia passo a passo sobre como utilizar a ferramenta SET (Social-Engineer Toolkit) no Kali Linux para criar um ataque de phishing direcionado à captura de credenciais do Facebook.  

> **Nota:** Este procedimento foi realizado dentro de um laboratório seguro e controlado com o objetivo de compreender técnicas de ataque e melhorar práticas de segurança.  

## **Requisitos**
- Um ambiente controlado com Kali Linux instalado.
- Permissões de root no sistema.
- O Social-Engineer Toolkit (SET), que vem pré-instalado no Kali Linux.

---

## **Passo a Passo**

1. **Iniciar o SEToolkit**  
   Abra o terminal e execute o seguinte comando para iniciar o SET:  
   ```bash
   sudo setoolkit
   ```

2. **Selecionar o tipo de ataque**  
   Escolha a opção para realizar um ataque de engenharia social:  
   ```  
   1) Social-Engineering Attacks  
   ```

3. **Selecionar o vetor de ataque**  
   Escolha a opção para realizar um ataque baseado em sites:  
   ```  
   2) Website Attack Vectors  
   ```

4. **Escolher o método de ataque**  
   Escolha a opção "Credential Harvester Attack Method":  
   ```  
   3) Credential Harvester Attack Method  
   ```

5. **Escolher a técnica de ataque**  
   Escolha a opção "Site Cloner" para clonar um site legítimo:  
   ```  
   2) Site Cloner  
   ```

6. **Configurar o endereço do site clonado**  
   Quando solicitado, insira o endereço da URL do site que deseja clonar, neste caso:  
   ```
   http://www.facebook.com
   ```

7. **Configurar o endereço IP para o servidor**  
   O SET solicitará o endereço IP que será usado para hospedar o site clonado. Insira o endereço IP local ou público da máquina Kali Linux.

---

## **Execução**
- Após seguir os passos acima, o SET criará um clone do site do Facebook e o hospeda no endereço IP fornecido.  
- Quando um usuário acessa o site clonado e insere suas credenciais, essas informações serão registradas no terminal ou no arquivo de logs do SET.

---

## **Mitigação**
- Certifique-se de sempre verificar URLs antes de inserir credenciais.
- Use autenticação de dois fatores (2FA) para maior segurança.
- Eduque usuários sobre práticas seguras de navegação e phishing.

