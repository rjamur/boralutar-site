---
layout: post
title: "Guia Definitivo de Markdown e Mermaid"
subtitle: "O código-fonte da documentação tática"
author: "Rafa"
date: 2026-09-20
---

# Título Principal (H1)
Este é o título principal do documento. Use apenas um H1 por página.

## Subtítulo (H2)
Usado para dividir as seções principais da sua crônica.

### Subseção (H3)
Níveis menores de organização. Vai até o H6 (usando ######).

---

## 1. Formatação de Texto

O asfalto exige **negrito para dar peso**, *itálico para pensamentos* e ~~tachado para ideias que já morreram~~. 
Você também pode destacar `código inline` no meio da frase, ou usar HTML básico para <sub>subscrito</sub> e <sup>sobrescrito</sup>.

---

## 2. Citações e Blockquotes

> "O amor maduro não é uma colisão frontal. É emparelhar a velocidade da queda."
> 
> — *O Coelho*

Citações aninhadas para diálogos profundos:
> O Lobo-Guará olhou para o Rabbit:
>> "Essa batalha não é sua. Volte para a retaguarda."

---

## 3. Listas

### Lista Não Ordenada (Bullets)
* Sobrevivência na Ocupação:
  * Silêncio
  * Observação
    * Tática da Pedra Cinza
* Escuta ativa

### Lista Ordenada (Números)
1. Primeiro pensa.
2. Depois reage.
3. Hackeia o sistema.

### Lista de Tarefas (Checklists)
- [x] Atualizar o Índice Central
- [x] Escrever "O Contrato Invisível"
- [ ] Configurar o Jekyll no GitHub Pages
- [ ] Subir as fotos da Ocupação

---

## 4. Links e Imagens

**Links Padrão:**
Conheça o [Boralutar](https://seu-site.com).

**Links de Referência:**
Eu leio muito [Gabor Maté][1] e [Paulo Freire][2].
[1]: https://exemplo.com/gabor
[2]: https://exemplo.com/freire

**Imagens:**
![Logo da Ocupação](https://via.placeholder.com/800x200.png?text=Ocupacao+Francisco)

---

## 5. Tabelas

As tabelas alinham a lógica fria do Córtex:

| Personagem | Arquétipo Psicológico | Função no Asfalto |
| :--- | :---: | ---: |
| **Córtex** | Lobo-Guará Sábio | Razão, Planejamento, Flow |
| **Rabbit** | Amígdala Assustada | Hipervigilância, Trauma |
| **Rainha** | Alice | Base Segura, Empatia |

*(Nota: os `:` definem o alinhamento: esquerda, centro, direita).*

---

## 6. Blocos de Código (Syntax Highlighting)

O GitHub entende dezenas de linguagens. Veja um script Python:

```python
def hackear_sistema(farao_ativo):
    if farao_ativo:
        print("Ativando Cavalo de Troia...")
        iniciar_roda_de_conversa()
    else:
        print("Paz na Toca.")