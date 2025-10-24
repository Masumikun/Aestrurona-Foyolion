---
date created: Thursday, 23rd ✦ Oct┆2025 ➣ 08▫49▫27 
date modified: Thursday, 23rd ✦ Oct┆2025 ➣ 08▫49▫27 
tipo:
  - evento/loja
categoria:
  - comércio_misterioso
gatilho:
  - condições_de_aparecimento
risco:
  - baixo/médio/alto
tags:
  - loja_noturna
  - misterioso
  - risco
---
# 🏪 Loja Noturna - {{data_do_jogo}}

## 🎭 Vendedor Misterioso
**Aparência:** {{descrição_física_do_vendedor}}
**Comportamento:** {{padrão_de_comportamento}}
**Identidade Suspeita:** [ ] Humano [ ] Furry [ ] Anomalia [ ] Desconhecido

**Diálogo de Abertura:**
> "{{frase_característica_do_vendedor}}"

## 📦 Inventário Noturno

### 🛒 Itens Com Desconto (25% off)
| Item | Preço Original | Preço Noturno | Efeito | Estoque |
|------|----------------|---------------|--------|---------|
| [[{{item1}}]] | 🪙{{preço1}} | 🪙{{preço1*0.75}} | {{efeito1}} | {{quantidade1}} |
| [[{{item2}}]] | 🪙{{preço2}} | 🪙{{preço2*0.75}} | {{efeito2}} | {{quantidade2}} |

### 🎁 Itens Grátis Com **Mutação**
| Item | Mutação | Penalidade | Raridade |
|------|---------|------------|----------|
| [[{{item_gratis1}}]] | {{mutação1}} | {{penalidade1}} | {{raridade1}} |
| [[{{item_gratis2}}]] | {{mutação2}} | {{penalidade2}} | {{raridade2}} |

### ⚠️ Itens Ilícitos
| Item | Preço | Efeito | Consequência Moral |
|------|-------|--------|-------------------|
| [[{{item_ilícito1}}]] | 🪙{{preço_ilícito1}} | {{efeito_ilícito1}} | {{consequência1}} |
| [[{{item_ilícito2}}]] | 🪙{{preço_ilícito2}} | {{efeito_ilícito2}} | {{consequência2}} |

## ⚡ Mecânicas Especiais

### 🔮 Sistema De Mutação
```javascript
// Ao aceitar item grátis
function aplicarMutação(item) {
  ganhar: `[[${item.mutação}]]`,
  penalidade: `-${item.penalidade} em ${atributo}`,
  efeito_visual: `${mudança_ambiental}`
}
```


### 🎲 Tabela De Riscos
**Role 1d6 após compra:**
1. **Vendedor te segue** até casa
2. **Item sussurra** durante a noite
3. **Chama atenção** de anomalias
4. **Sonhos perturbadores**
5. **Memória corrompida**
6. **Seguro** (nada acontece)

### 💰 Economia Noturna
**Modificadores de Preço:**
- [ ] Chuva: +10% desconto
- [ ] Lua Cheia: +15% risco
- [ ] Energia ≤ 1⚡: +20% desconto
- [ ] Reputação com Furrys: ±5% por nível

## 🗣️ Diálogos Dinâmicos

### 💬 Baseado Na Sua Condição
**Se energia baixa:**
> "Você parece cansado... precisa de algo forte?"

**Se alta reputação com Furrys:**
> "Ouvi falar de você... tenho algo especial."

**Se já comprou antes:**
> "De volta por mais, meu cliente frequente?

### ❓ Investigação Do Vendedor
**Testes de Percepção:**
- [ ] **Olhar nos olhos:** {{dica_sobre_espécie}}
- [ ] **Observar mãos:** {{pista_física}}
- [ ] **Cheiro:** {{odor_característico}}
- [ ] **Voz:** {{padrão_de_fala_suspeito}}

## 📝 Registro Da Visita

### ✅ Itens Comprados
- [ ] `{{item}}` por 🪙`{{preço}}`
- [ ] `{{item_gratis}}` (MUTAÇÃO: `{{mutação}}`)

### ⚠️ Consequências Imediatas
- [ ] `{{mudança_ambiental}}`
- [ ] `{{efeito_mental}}`
- [ ] `{{alteração_física}}`

### 🔮 Efeitos De Longo Prazo
**Próximos Dias:**
- Dia 1: `{{efeito_imediato}}`
- Dia 2: `{{efeito_progressivo}}`
- Dia 3: `{{consequência_final}}`

## 🎯 Condições De Aparecimento
```yaml
gatilho:
  - energia_baixa: true
  - rejeicoes: 3
  - noite_especial: "lua_cheia"
  - reputação_minima: 2
  - evento_anterior: "sobreviveu_anomalia"

frequencia:
  - min_noites: 3
  - max_aparicoes: 2
  - cooldown: 5
```

---

**📋 Notas do Desenvolvedor:**
> *Esta loja aparece quando o jogador está mais vulnerável, oferecendo soluções arriscadas para problemas desesperados. Cada compra noturna deve sentir-se como um pacto faustiano.*
---