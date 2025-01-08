# 🛡️ **Demonstração de Phishing com Kali Linux**

⚠️ **Aviso Legal**:  
Este projeto foi criado exclusivamente para **fins educacionais** e conscientização sobre segurança cibernética. O uso indevido das informações aqui contidas pode ser considerado crime. **Nunca utilize este conteúdo para atividades maliciosas.**

---

## 📋 **Visão Geral**
Este projeto demonstra como configurar uma página de phishing usando o Kali Linux e o SEToolkit para educar sobre ataques de phishing e como se proteger contra eles.

---

## 🛠️ **Ferramentas Utilizadas**
- **Kali Linux**: Distribuição Linux focada em testes de penetração.
- **SEToolkit**: Ferramenta para simulação de ataques de engenharia social.

---

## ⚙️ **Passo a Passo Detalhado**

### 1. **Obtenha acesso root:**
   - Execute o seguinte comando no terminal:
     ```bash
     sudo su
     ```
   - Este comando eleva os privilégios do usuário atual para o nível de administrador (root). Isso é necessário porque o SEToolkit e outros processos de rede no Kali Linux geralmente requerem permissões administrativas.

### 2. **Inicie o SEToolkit:**
   - Execute o comando:
     ```bash
     setoolkit
     ```
   - Inicia o Social-Engineer Toolkit (SEToolkit), uma ferramenta poderosa para realizar testes de engenharia social, incluindo ataques de phishing.

### 3. **Selecione o tipo de ataque:**
   - Navegue pelas opções do menu interativo:
     ```
     Social-Engineering Attacks > Web Site Attack Vectors > Credential Harvester Attack Method > Site Cloner
     ```
   - **Social-Engineering Attacks:** Abre o menu de ataques baseados em engenharia social.
   - **Web Site Attack Vectors:** Define o vetor de ataque como uma página web maliciosa.
   - **Credential Harvester Attack Method:** Configura o ataque para capturar credenciais (usuário e senha) inseridas pelos alvos.
   - **Site Cloner:** Permite clonar um site legítimo para enganar os usuários e coletar suas informações.

### 4. **Obtendo o endereço IP da máquina:**
   - Execute o comando:
     ```bash
     ifconfig
     ```
   - Este comando exibe as configurações de rede da máquina. O endereço IP exibido (por exemplo, `192.168.1.14`) será usado para hospedar a página de phishing e deve ser acessível pela vítima.

### 5. **Definindo o site alvo:**
   - Durante o processo de configuração, o SEToolkit solicitará uma URL para ser clonada. Neste caso:
     ```
     http://www.facebook.com
     ```
   - Este URL é o site que será copiado pelo SEToolkit para criar a página de phishing. O clone terá a aparência exata do Facebook original.

### 6. **Captura de credenciais:**
   - Uma vez configurado, o SEToolkit cria um servidor local que hospeda a página clonada. Quando a vítima acessa o IP da máquina e insere credenciais, o SEToolkit captura essas informações e as exibe no terminal.

---

## 🔒 **Prevenção e Conscientização**
1. **Verifique URLs** antes de inserir credenciais.
2. **Ative a autenticação em dois fatores (2FA)** sempre que possível.
3. **Mantenha softwares de segurança atualizados** e evite acessar links desconhecidos.

---

## 📜 **Licença**
Este projeto é licenciado sob os termos da [Licença MIT](LICENSE).

---

## 🤝 **Contribuições**
Contribuições para melhorar este projeto são bem-vindas. Sinta-se à vontade para abrir um pull request ou relatar problemas.

---

## 🌐 **Descrição Adicional**

### **O que cada comando faz:**

1. **`sudo su`:** Eleva privilégios para root, permitindo executar ferramentas avançadas.
2. **`setoolkit`:** Inicia o Social-Engineer Toolkit.
3. **Menu interativo do SEToolkit:**
   - Escolha do ataque e métodos usados para configurar o phishing.
4. **`ifconfig`:** Obtém o endereço IP local da máquina.
5. **Clone do site:** Define o alvo como o Facebook, criando uma réplica do site original.
6. **Captura de dados:** Exibe os dados capturados no terminal do SEToolkit.

---

# 🛡️ **Phishing Demonstration with Kali Linux**

⚠️ **Legal Disclaimer**:  
This project was created exclusively for **educational purposes** and to raise awareness about cybersecurity. Misusing the information contained here may be considered a crime. **Never use this content for malicious activities.**

---

## 📋 **Overview**
This project demonstrates how to set up a phishing page using Kali Linux and the SEToolkit to educate about phishing attacks and how to defend against them.

---

## 🛠️ **Tools Used**
- **Kali Linux**: A Linux distribution focused on penetration testing.
- **SEToolkit**: A tool for simulating social engineering attacks.

---

## ⚙️ **Step-by-Step Guide**

### 1. **Gain root access:**
   - Run the following command in the terminal:
     ```bash
     sudo su
     ```
   - This command elevates the current user privileges to administrator (root). This is necessary because SEToolkit and other networking processes in Kali Linux typically require administrative permissions.

### 2. **Start SEToolkit:**
   - Run the command:
     ```bash
     setoolkit
     ```
   - Launches the Social-Engineer Toolkit (SEToolkit), a powerful tool for conducting social engineering tests, including phishing attacks.

### 3. **Select the type of attack:**
   - Navigate through the interactive menu options:
     ```
     Social-Engineering Attacks > Web Site Attack Vectors > Credential Harvester Attack Method > Site Cloner
     ```
   - **Social-Engineering Attacks:** Opens the menu for social engineering-based attacks.
   - **Web Site Attack Vectors:** Sets the attack vector to a malicious web page.
   - **Credential Harvester Attack Method:** Configures the attack to capture credentials (username and password) entered by targets.
   - **Site Cloner:** Allows cloning a legitimate site to deceive users and collect their information.

### 4. **Obtain the machine's IP address:**
   - Run the command:
     ```bash
     ifconfig
     ```
   - This command displays the machine's network configurations. The displayed IP address (e.g., `192.168.1.14`) will be used to host the phishing page and must be accessible to the victim.

### 5. **Set the target site:**
   - During the setup process, SEToolkit will prompt for a URL to be cloned. In this case:
     ```
     http://www.facebook.com
     ```
   - This URL is the site that will be copied by SEToolkit to create the phishing page. The clone will look exactly like the original Facebook site.

### 6. **Capture credentials:**
   - Once configured, SEToolkit creates a local server hosting the cloned page. When the victim accesses the machine's IP and enters credentials, SEToolkit captures this information and displays it in the terminal.

---

## 🔒 **Prevention and Awareness**
1. **Check URLs** before entering credentials.
2. **Enable two-factor authentication (2FA)** whenever possible.
3. **Keep security software updated** and avoid clicking on unknown links.

---

## 📜 **License**
This project is licensed under the terms of the [MIT License](LICENSE).

---

## 🤝 **Contributions**
Contributions to improve this project are welcome. Feel free to open a pull request or report issues.

---

## 🌐 **Additional Description**

### **What each command does:**

1. **`sudo su`:** Elevates privileges to root, allowing advanced tools to run.
2. **`setoolkit`:** Launches the Social-Engineer Toolkit.
3. **SEToolkit interactive menu:**
   - Attack selection and methods used to configure phishing.
4. **`ifconfig`:** Retrieves the local machine's IP address.
5. **Site cloning:** Sets the target as Facebook, creating a replica of the original site.
6. **Data capture:** Displays the captured credentials in the SEToolkit terminal.

