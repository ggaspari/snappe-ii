# Calculadoras Neonatais

Calculadoras client-side (HTML/JS puro, sem dependências de build) para escores
de gravidade e risco usados em UTIN. Cada uma é uma página independente.

- **[SNAPPE-II](https://ggaspari.github.io/snappe-ii/)** — Score for Neonatal
  Acute Physiology, Perinatal Extension II.
- **[CRIB-II](https://ggaspari.github.io/snappe-ii/crib-ii/)** — Clinical Risk
  Index for Babies II.

## SNAPPE-II

- Pontuação dos 9 itens conforme Richardson DK et al., J Pediatr. 2001;138:92–100.
- Mortalidade estimada por faixa de escore e peso ao nascer (<1500 g / ≥1500 g),
  reproduzida da tabela de calibração da coorte original (N=25.429), via
  calculadora da SFAR (sfar.org/scores2/snap22.php).
- Classificação de PIG (pequeno para idade gestacional) calculada automaticamente
  a partir do peso ao nascer e da idade gestacional informados, usando o percentil 3
  combinado de Alexander GR et al., Obstet Gynecol. 1996;87:163–168 — mesmos valores
  de corte reproduzidos pela calculadora da SFAR.

Acesse **https://ggaspari.github.io/snappe-ii/**, ou baixe `index.html` e abra
localmente na sua instituição para acesso off-line.

## CRIB-II

- Pontuação conforme Parry G, Tucker J, Tarnow-Mordi W; UK Neonatal Staffing
  Study Collaborative Group. Lancet. 2003;361(9371):1789–91.
- Escore = pontos da tabela peso × idade gestacional (específica por sexo) +
  temperatura à admissão + excesso de base, variando de 0 a 27.
- Mortalidade prevista pela fórmula logística original (Logit = −6,476 + 0,45 ×
  CRIB-II).
- A tabela peso × IG foi transcrita diretamente da tabela de referência estática
  da calculadora da SFAR (sfar.org/scores2/crib22.php) — **não** do JavaScript
  interativo daquela página, que tem um defeito: para diversas combinações de
  peso muito baixo com determinada idade gestacional (ex.: peso <751 g com
  IG=32 sem., <501 g com IG=29–31 sem.), nenhuma faixa de código é acionada e o
  campo de pontos permanece zerado por padrão, subestimando o escore. Esta
  calculadora sinaliza essas combinações como não calculáveis em vez de zerá-las.

Acesse **https://ggaspari.github.io/snappe-ii/crib-ii/**, ou baixe
`crib-ii/index.html` e abra localmente para acesso off-line.

## Recursos comuns às duas calculadoras

- Tema claro/escuro alternável (botão no cabeçalho), com preferência salva no
  navegador.
- Não coletam, armazenam ou transmitem dados — todo cálculo ocorre localmente
  no navegador.

## Aviso

Ferramentas de apoio clínico. Não substituem julgamento médico nem validação
local.

## Licença

Distribuído sob a [licença MIT](LICENSE) — uso, cópia e modificação livres,
sem garantia de qualquer tipo (inclusive de adequação a uso clínico real).
