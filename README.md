# Bloco Site Info (`block_site_info`)

O **Site Info** é um bloco customizado para o Moodle, desenvolvido como parte da suíte de temas **suap-moodletheme-suite** do IFRN (Instituto Federal do Rio Grande do Norte). Ele permite exibir informações institucionais, estatísticas gerais ("O Moodle em números") ou qualquer conteúdo HTML personalizado nas páginas principais do Moodle.

---

## 📌 Funcionalidades

- **Conteúdo HTML Customizável**: O administrador ou gerente da página pode configurar o conteúdo livremente através do editor de texto nativo do Moodle.
- **Visual Padrão**: Apresenta por padrão uma seção moderna com estatísticas do IFRN (anos de história, quantidade de cursos, quantidade de alunos e certificados emitidos).
- **Design Responsivo**: Adaptado para telas menores (responsividade em dispositivos móveis), ajustando as colunas de informações.
- **Integração com Temas**: Desenvolvido sob medida para herdar variáveis de cores e fontes do tema SUAP.

---

## ⚙️ Requisitos

- **Moodle**: Versão `4.1` ou superior (requer Moodle versão `2022112800` ou posterior).

---

## 🚀 Instalação

1. Baixe ou clone este repositório para o diretório de blocos do seu Moodle:
   ```bash
   git clone https://codelab.ifrn.edu.br/dead-zl/ava/lms/block_site_info.git blocks/site_info
   ```
   *Nota: Certifique-se de que o nome da pasta de destino seja estritamente `site_info`.*

2. Acesse a área de administração do seu Moodle (ou execute via CLI) para atualizar o banco de dados e concluir a instalação:
   ```bash
   php admin/cli/upgrade.php
   ```

---

## 🛠️ Configuração e Uso

1. Entre no Moodle como administrador ou com permissão de edição.
2. Ative o **Modo de Edição** no topo da página.
3. Adicione o bloco **Site Info** nas páginas onde ele é permitido (por padrão, Página Inicial/Site Index e Painel/Dashboard).
4. Para alterar os dados exibidos:
   - Clique na engrenagem de configuração do bloco e selecione **Configurar bloco Site Info**.
   - Altere o HTML na **Caixa de texto** conforme necessário.
   - Salve as mudanças.

---

## 🎨 Estilização e Personalização

Os estilos específicos deste bloco estão localizados em [styles.css](file:///C:/Users/2080882/projetos/IFRN/suap-moodletheme-suite/block_site_info/styles.css). O bloco utiliza variáveis CSS personalizadas (ex: `--font-heading7`, `--font-heading2`, `--font-heading4`, `--general-white`), garantindo consistência visual quando utilizado em conjunto com o tema da suíte.

O template de exibição utiliza o Moodle Mustache Template, localizado em [templates/site_info.mustache](file:///C:/Users/2080882/projetos/IFRN/suap-moodletheme-suite/block_site_info/templates/site_info.mustache).

---

## 📄 Licença

Este plugin é um software livre distribuído sob os termos da licença GNU General Public License v3 ou posterior. Consulte o arquivo [LICENSE.md](file:///C:/Users/2080882/projetos/IFRN/suap-moodletheme-suite/block_site_info/LICENSE.md) para obter mais detalhes.
