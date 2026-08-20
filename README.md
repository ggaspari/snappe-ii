# SNAPPE-II — Calculadora de Gravidade Neonatal

Calculadora client-side (HTML/JS puro, sem dependências de build) para o
score SNAPPE-II (Score for Neonatal Acute Physiology, Perinatal Extension II).

- Pontuação dos 9 itens conforme Richardson DK et al., J Pediatr. 2001;138:92–100.
- Mortalidade estimada por faixa de escore e peso ao nascer (<1500 g / ≥1500 g),
  reproduzida da tabela de calibração da coorte original (N=25.429), via
  calculadora da SFAR (sfar.org/scores2/snap22.php).
- Classificação de PIG (pequeno para idade gestacional) calculada automaticamente
  a partir do peso ao nascer e da idade gestacional informados, usando o percentil 3
  combinado de Alexander GR et al., Obstet Gynecol. 1996;87:163–168 — mesmos valores
  de corte reproduzidos pela calculadora da SFAR.
- Tema claro/escuro alternável (botão no cabeçalho), com preferência salva no navegador.

## Uso

Acesse **https://ggaspari.github.io/snappe-ii/**.

Alternativamente, baixe o `index.html` e abra localmente na sua instituição
para acesso off-line — não requer servidor nem instalação.

## Aviso

Ferramenta de apoio clínico. Não substitui julgamento médico nem validação
local. Não coleta, armazena ou transmite dados — todo cálculo ocorre
localmente no navegador.

## Licença

Distribuído sob a [licença MIT](LICENSE) — uso, cópia e modificação livres,
sem garantia de qualquer tipo (inclusive de adequação a uso clínico real).
