# Entre Faixas — by Onlion | Edição 2

Uma coleção pessoal de 32 faixas: 29 gravações e três demos instrumentais. Interface em português do Brasil. Nenhuma conta, assinatura, biblioteca externa, fonte remota ou servidor é necessário para abrir a coleção em um navegador de computador que permita arquivos locais.

## Como abrir

1. Extraia o ZIP inteiro. Mantenha `index.html`, `app.js`, `style.css`, `catalog.js` e as pastas `music`, `artwork`, `lyrics` juntos.
2. Abra `index.html` no Safari, Chrome, Firefox ou Edge. Não abra o arquivo diretamente dentro do ZIP.
3. Clique em Reproduzir. O navegador exige uma interação antes de iniciar o áudio.

No celular, especialmente iPhone/iPad, o app Arquivos pode abrir HTML apenas como prévia e impedir scripts ou acesso às outras pastas. Isso depende do sistema/navegador. Se ocorrer, use a mesma coleção em uma hospedagem estática HTTPS (como GitHub Pages), ou abra no computador. Não há backend. O funcionamento sem servidor em iOS não é garantido.

## Sua biblioteca

- **Editar nome e letra:** clique nos três pontos de qualquer faixa. O painel de letras também tem o botão Editar.
- **Organizar:** clique em Organizar. Arraste as faixas no computador ou use as setas para cima/baixo, inclusive em telas de toque. Clique em Concluir. A ordem da biblioteca e a de cada playlist são independentes.
- **Playlists:** Nova playlist → escolha um nome → marque as músicas. Use Opções para editar, organizar ou excluir. Os três pontos da faixa permitem adicioná-la a uma playlist. Excluir uma playlist não remove a música da biblioteca.
- **Favoritas:** toque no coração. A seção Favoritas reúne as faixas selecionadas.
- **Player:** reproduzir/pausar, anterior/próxima, aleatório, repetir fila ou faixa, volume (computador), mute, barra de progresso em forma de onda, painel de letras. A fila acompanha a seleção que estava aberta quando uma faixa foi escolhida. A barra de ondas usa amplitudes reais pré-calculadas. Algumas plataformas móveis controlam o volume pelo sistema.
- **Busca e visualização:** filtre pelo nome, inclusive sem acentos, e alterne lista/grade.

## Salvar e compartilhar

As alterações ficam automaticamente no armazenamento local do navegador quando disponível. Isso não modifica diretamente `songs.json` nem os arquivos de áudio. O armazenamento de páginas locais pode variar conforme o navegador, a pasta e as configurações de privacidade. Exporte backups regularmente.

Em **Gerenciar biblioteca**:
- **Exportar backup**: gera um JSON com nomes, letras editadas, ordem, favoritas e playlists. Importe em outro navegador para recuperar essas escolhas.
- **Importar backup**: restaura as configurações e substitui as alterações atuais após confirmação.
- **Exportar versão para compartilhar**: gera um `catalog.js` com as músicas e suas configurações. Faça uma cópia da pasta do projeto, substitua o `catalog.js` dessa cópia pelo arquivo exportado e compacte a pasta inteira. Envie o novo ZIP aos amigos. Eles receberão a ordem, títulos, letras editadas e playlists escolhidas. Se preferir, envie apenas o backup para alguém que já tem esta mesma versão da coleção.
- **Restaurar biblioteca original**: volta às configurações padrão desta cópia do projeto, sem tocar nos arquivos de áudio.

Links para faixas individuais funcionam quando a coleção é publicada na web; um caminho local não é um link que outra pessoa pode abrir. A publicação deve conter todos os arquivos de reprodução e respeitar os direitos das gravações e imagens. Se as letras incluírem informações pessoais, considere quem terá acesso antes de publicar.

## Conteúdo e compatibilidade

- 32 faixas mantidas, inclusive demos e versões alternativas. Nenhuma gravação original foi descartada.
- 28 arquivos de letras em texto foram limpos: marcações de produção, indicações de instrumentos, acordes isolados e etiquetas de seção removidos. As palavras, repetições e vocais de apoio foram preservados quando identificáveis. Três letras de demonstração em JSON foram mantidas com seus tempos e traduções.
- **Eles tentam me derrubar** não tinha um arquivo de letra nem metadados com letra no material recebido; use Editar para incluí-la. Não foi inventada uma letra. As outras letras sem timestamps aparecem completas, não como sincronização artificial.
- Dez arquivos M4A continham áudio Opus. Para melhorar a compatibilidade com Safari/iOS, foram criadas cópias AAC em `music/playback/`; os originais continuam no local original. O AAC é uma conversão com perdas, não uma substituição do master.
- Todas as capas fornecidas foram mantidas. O plano de fundo e a paleta são derivados da capa da música ativa.
- `catalog.js` é o catálogo ativo e contém metadados, letras, durações e ondas calculadas. `songs.json` e a pasta `lyrics/` são arquivos de referência para manutenção; para edições normais, use a interface e exporte o catálogo ou backup.

## Hospedagem opcional

O projeto é estático. Se quiser publicar em GitHub Pages, envie a pasta inteira para um repositório apropriado, mantendo as subpastas, e ative Pages para a branch desejada. Os arquivos originais de áudio convertidos podem ser omitidos de uma cópia hospedada para economizar espaço, desde que todos os caminhos de reprodução em `catalog.js` estejam presentes. O app não depende de conexão com serviços de música.
