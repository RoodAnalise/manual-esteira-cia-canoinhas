# Manual Técnico — Esteira de Alimentação de Carga CIA Canoinhas

**Código de fabricação: 28470**

Manual em HTML (mesmo modelo visual do Manual Linha Tornado 1,4).
Para abrir: duplo clique em `index.html`. Funciona offline, sem instalar nada.

## O que é o equipamento

Esteira de alimentação de carga **móvel sobre rodízios**, para carga de **pacotes de papel
higiênico**. Uma ponta fica no piso do pátio e a outra é conduzida para dentro do baú.
O operador externo alimenta a correia; o operador interno, dentro do baú, retira e empilha.

## Estrutura de seções

| Seção | Conteúdo |
|---|---|
| Capa | Identificação, correia, geometria, acionamento, mobilidade, segurança |
| 1. Aplicação e Operação | Finalidade, fluxo, correia, geometria, mobilidade, dimensões, componentes |
| 2. Posicionamento | Checklist antes/depois de posicionar no caminhão |
| 2.1 Segurança no Baú | Acesso, comunicação, parada de emergência, NR-35 |
| 2.2 Dispositivos de Segurança | Cordão Schmersal, fotocélula, tampas, checklist |
| 3. Manutenção e Ajustes | **Fusop M20**, correção de corredor, **base do motoredutor** |
| 3.4 Correia e Emenda | Especificação, **canais da guia**, manuseio, emenda |
| 3.5 Guia Central e Mesa | Estrutura, manutenção, diagnóstico rápido |
| 3.6 Rodízios e Estrutura | Cuidados, manutenção periódica, parafusos |
| 3.7 Motor, Redutor e Painel | Acionamento, motor WEG, redutor WCG01, painel |
| **3.8 Mancais e Rolamentos** | **5× F206 + 5× EX206**, engrenagens 1.50.18 / 1.50.35, **cálculo da corrente** |
| 4. Tabelas Técnicas | Dados de operação, **lista de 6 peças de reposição**, lubrificação |
| 5. Diagnóstico | 22 falhas com causa / verificação / ação |
| 6. Segurança | NR-12 + NR-35, LOTO, EPI |

## Dois tensionadores — não confunda

| | Ajusta | Onde | Como |
|---|---|---|---|
| **Fusop M20** | a **correia** | lado do esticador | Afrouxar a porca **interna**, apertar a **externa** |
| **Base oblonga** | a **corrente de tração** | lado do motoredutor | Afrouxar os **6 parafusos**, correr a base no oblongo até a corrente encaixar, **reapertar os 6** |

Correção de corredor da correia também é pelo fusop M20: **apertar mais o lado para o qual
a correia atravessa**.

## Dados já preenchidos (memória de cálculo)

```
C  = 11.760 mm   (distância entre centros, rolo de tração → esticador)
D  =   112 mm    (diâmetro do rolo de tração)
Comprimento total = 11.900 mm  ->  balanço de 70 mm em cada ponta
Largura total     =   940 mm  ->  70 mm de folga de cada lado da correia de 800 mm
Altura da mesa    =   830 mm  (rodízio 8" + pé)
Peso do conjunto  =   980 kg  ->  245 kg por rodízio (260 kg em aclive 3%)

L  ≈ 2C + πD = 2 × 11.760 + π × 112 = 23.871,9 mm   (teórico)
   + 140 mm curso do esticador  = 24.011,9 mm
   + folga de emenda            = a definir com o fornecedor da lona

Velocidade: 1750 rpm (4P) ÷ 20 (i=1:20) = 87,5 rpm no redutor
            corrente: 35/18 = 1,944:1  ->  rolo = 87,5 ÷ 1,944 = 45,0 rpm
            v = 45,0 × π × 0,112 = 15,8 m/min
            percurso (11,76 m) ≈ 45 s
            CONFIRMAR EM CAMPO: cronometrar um pacote entre duas marcas

Cadeia de tração: centro C = 285 mm | Z1 = 18 (rolo) | Z2 = 35 (redutor)
   L(p) = 2C/p + (Z1+Z2)/2 + ((Z2-Z1)/2pi)^2 × p/C
   9,525 mm  06B/ANSI35  -> 86,59 passes -> 88 elos ->  838,2 mm
  12,70  mm 08B/ANSI40  -> 71,71 passes -> 72 elos ->  914,4 mm
  15,875 mm 10B/ANSI50  -> 62,81 passes -> 64 elos -> 1.016,0 mm
  19,05  mm 12B/ANSI60  -> 56,91 passes -> 58 elos -> 1.104,9 mm

Entre eixos dos rodízios = 11.900 − 2.000 − 2.000 = 7.900 mm
```

**Os 2.000 mm dos rodízios não somam comprimento** — são medidos para dentro.
Conferência: 11.760 (C) + 70 + 70 = 11.900 mm.

**Falta o passo da corrente** para fechar o comprimento. A tabela acima cobre os quatro
passos usuais — identificar o da corrente instalada e usar a linha correspondente.
Corrente é vendida em **número par de elos**, sempre arredondado para cima.

**Atenção:** o comprimento comercial da correia é **fechado com o fabricante**, que soma a
folga de emenda. Na cotação, sempre passar a **medição real de campo**, não o valor teórico.

## Mancais e rolamentos

Par padronizado do equipamento — **cite sempre os dois juntos**:

| Item | Qtd. | Spec |
|---|---|---|
| Mancal | **5** | F206 (furo 30 mm) |
| Rolamento | **5** | EX206 (furo 30 mm) |

Um dos 5 mancais fica na **base do redutor**. Os outros 4 ficam nos rolos —
**confirmar no plano mecânico** se é um de cada lado do rolo de tração e do esticador.

**Trocar mancal e rolamento juntos.** Rolamento novo em mancal com pista desgastada falha cedo.

## Engrenagens da corrente de tração

| Peça | Código |
|---|---|
| Engrenagem no **rolo** de tração | **1.50.18** |
| Engrenagem no **redutor** | **1.50.35** |

Conferir o **número de dentes** das duas para fechar o cálculo da velocidade da correia.
Não assumir — a relação muda a vazão de carga.

## O que ainda precisa ser preenchido

### Capa
- CNPJ / IE → "Preencher"
- Endereço → hoje só "Canoinhas - SC, CEP 89460-000"

### Tabela 4.1 (Dados de Operação)
- **Tensão de alimentação** (`____ V`) — confirmar na placa do motor. Um motor de 2,2 kW
  em 220 V puxa corrente praticamente o dobro; ligar 380 V em motor de 220 V **queima o motor**.
- **Velocidade da correia** — corrigida para ≈ 15,8 m/min com a relação 1,944:1.
  Confirmar em campo: cronometrar um pacote entre duas marcas e fazer `distância ÷ tempo`.
- **Carga máxima por pacote** (`____ kg`)
- **Furação da platina** — a informar
- **Capacidade dos rodízios** — cada um recebe 245 kg (até 260 kg em aclive 3%).
  Conferir a capacidade nominal dos Colson 8" e dos traseiros.

### Lista de Peças de Reposição (4.2)

A tabela tem **6 itens** — redutor, correia, corrente, as duas engrenagens e os rolamentos.
Os códigos estão como `———`: a Zico tem os códigos internos, pedir a lista impressa.

Antes de cotar, confirmar:
- **Correia** — comprimento medido em campo (o ref. 24.012 mm é teórico)
- **Corrente** — **passo** (9,525 / 12,7 / 15,875 / 19,05 mm) e número par de elos
- **Engrenagens** — 1.50.18 (rolo) e 1.50.35 (redutor): conferir dentes e furo
- **Rolamento** — citar sempre o par **F206 + EX206** (furo 30 mm)

## Canais da guia central — item crítico de fabricação

A guia central entra em **canal usinado** em **três** componentes. Se qualquer um
não for usinado, a correia perde alinhamento e a tensão não é uniforme:

1. Rolo de tração
2. Rolo esticador
3. Mesa

## Imagens

Todas em `imagens/` são **placeholders**. Substitua cada arquivo mantendo o mesmo nome.
As 4 fotos estão marcadas como **prioritárias** — sem elas o manual perde a função de manual.

| Arquivo | Onde aparece | O que fotografar |
|---|---|---|
| `capa.jpg` | Capa (85% da largura) | **Foto de apresentação** — vista da esteira inteira no pátio, ao lado do caminhão, com a ponta externa no piso |
| `tensor.jpg` | 5.2.1 Tensionamento (70%) | **Tensionador de correia** — detalhe do fusop M20 com a porca interna e a porca externa visíveis, na cabeceira do esticador |
| `corrente_tracao.jpg` | 5.2.3 Tensionamento (80%) | **Tensionador de corrente + motor de tração** — motoredutor com a base de 6 parafusos, a corrente e a engrenagem 1.50.35 no redutor |
| `cabeceira_tracao.jpg` | 5.6 Mancais e Engrenagens (80%) | **Cabeceira de tração** — rolo de tração com o canal da guia central |
| `mancais_engrenagens.jpg` | 5.6 Mancais e Engrenagens (85%) | **Mancais F206 + engrenagens de tração** — mancal com o rolamento EX206 e, no mesmo conjunto, as engrenagens 1.50.18 (rolo) e 1.50.35 (redutor) |

### Como substituir

Arraste a foto para dentro da pasta `imagens` e, quando aparecer *"Este arquivo já existe"*,
clique em **Substituir**. Não precisa renomear nada.

Três erros que quebram a imagem:

- **Extensão diferente de `.jpg`** — `.jpeg`, `.png` e `.heic` (padrão do iPhone) não abrem
- **Extensão dupla** — `capa.jpg.png`. Para ver as extensões: *Exibir → Mostrar → Extensões de nome de arquivo*
- **Acento ou espaço no nome** — não use

Maiúsculas não são problema no Windows.

Todas as imagens abrem em tela cheia ao clicar (lightbox) e mostram "clique para ampliar"
ao passar o mouse. Para adicionar uma foto nova: coloque o arquivo em `imagens/` e copie
um bloco `<div class="img-wrapper">...</div>` existente, trocando o caminho do `src`.

## Botão "Cotar" (WhatsApp)

A lista de peças de reposição tem **6 botões** (redutor, correia, corrente, 2 engrenagens,
rolamento) que abrem o WhatsApp com o texto da peça já escrito e o **código de fabricação
28470** no início da mensagem. Para trocar o número, pesquise `wa.me/5547991865021` no
arquivo. Os textos das mensagens estão logo após `?text=`.

## Publicação

**PDF:** abra no navegador e use `Ctrl + P` → "Salvar como PDF".
O CSS já tem regras de impressão (imagens em 80%, sem menus, cores em preto).

**GitHub Pages:** subir a pasta inteira para um repositório e ativar Pages na branch
`main`, pasta `/ (root)`.
